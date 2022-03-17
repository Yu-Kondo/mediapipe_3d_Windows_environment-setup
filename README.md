# mediapipe_3d_Windows_environment-setup_Using_analysis
※コマンドプロンプトで１つずつ入力


※anacondaをインスト―ルしていない場合は，下記URLを参考にanacondaをダウンロード及びインストール
  https://www.javadrive.jp/python/install/index5.html
 （「Add Anaconda 3 to the system PATH environment variable」は，チェックを入れる）

## 準備
### 1) anaconda仮想環境作成（python3.10）
     conda create -n 3dpose python

### 2) 仮想環境をアクティベート
     activate 3dpose

### 3) mediapipeのインストール
     pip install mediapipe

### 4) opencvのインストール
     conda install -c conda-forge opencv

### 5) matplotlibのインストール
     conda install -c conda-forge matplotlib

### 6) mediapipe-python-sample-main.zip をデスクトップにダウンロードおよび解凍

## 実行
### 1) 仮想環境が 3dpose であることを確認
     conda info -e
   ※仮想環境が 3dpose でない場合は，【準備】の #2 コマンドを入力
   
### 2) ファイルのある階層までコマンドで進む
     cd desktop/mediapipe-python-sample-main

### 3 plot_world_landmark オプション（3D描画）付きで実行（pose/holistic のみ）
     python sample_holistic.py --plot_world_landmark
     （python ファイル名 第一引数）

### 4 終了方法
     plot_world_landmark
オプションを利用している場合は、3D描画のウィンドウを×ボタン押下で閉じる

その後コマンドプロンプトで [ctrl] + [c]

mp4 ファイルを読み込んでいる場合は，mp4 ファイルが終了すると同時に終了する
