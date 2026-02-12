## Convert Python Script to App(.exe)
pythonのスクリプトをexe化する手順

## pyinstallerのインストール
pip install pyinstaller
※もしプロキシーエラーが出た場合はこちらを参照
https://github.com/yubun241/python_venv

## exeファイル化の実施
① コマンドプロンプトを開き
② python環境に入る
③ exe化するscriptが格納されているディレクトリをカレントディレクトに設定する
④ 以下のコマンドを実行
　pyinstaller your_script.py --onefile
⑤ 同フォルダいくつかフォルダが生成される
  distフォルダの中に.exeが作成される
 ※Pathの都合上distフォルダから出す必要がある

 ## 注意事項
 こちらは環境ごとまるまるアプリ化をするのでpython環境のないPCや環境でも動作するが
 読み込んだ環境が激重だった場合は起動するまで時間が掛かることがよくある。
 また、途中でtimeOutEroorになることもある。
 exe化するときは必要最低限のライブラリの入った環境で行うことをお勧めします。
 一部streamlitなどのサーバーを起動させるようなwebアプリ関連ではexe化がうまく動かなかったことがありました。
 その際はpythonフォルダの環境ごと移植することをお勧めします。
 
