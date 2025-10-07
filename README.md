# DEIMv2-ONNX-Sample
[Intellindust-AI-Lab/DEIMv2](https://github.com/Intellindust-AI-Lab/DEIMv2)のPythonでのONNX推論サンプルです。<br>
変換自体を試したい方は、Google Colaboratory上で[Convert2ONNX.ipynb](Convert2ONNX.ipynb)を使用ください。<br><br>

![image](https://github.com/user-attachments/assets/7e1fa0d3-5baa-43c3-9b5f-5c2fefee3956)

# Requirement 
* OpenCV 4.5.3.56 or later
* onnxruntime 1.11.0 or later

# Convert
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kazuhito00/DEIMv2-ONNX-Sample/blob/main/Convert2ONNX.ipynb)<br>
Colaboratoryでノートブックを開き、上から順に実行してください。<br>

# Demo
デモの実行方法は以下です。
```bash
python sample_onnx.py
```
* --device<br>
カメラデバイス番号の指定<br>
デフォルト：0
* --movie<br>
動画ファイルの指定 ※指定時はカメラデバイスより優先<br>
デフォルト：指定なし
* --image<br>
画像ファイルの指定 ※指定時はカメラデバイスより優先<br>
デフォルト：指定なし
* --model<br>
ロードするモデルの格納パス<br>
デフォルト：model/deim_dfine_hgnetv2_s_coco_120e.onnx
* --score_th<br>
検出閾値<br>
デフォルト：0.6
* --unuse_gpu<br>
GPU推論なし（CPU推論）<br>
デフォルト：指定なし

# Reference
* [Intellindust-AI-Lab/DEIMv2](https://github.com/Intellindust-AI-Lab/DEIMv2)

# Author
高橋かずひと(https://twitter.com/KzhtTkhs)
 
# License 
DEIMv2-ONNX-Sample is under [Apache 2.0 License](LICENSE).

# Note
サンプルの画像は[ぱくたそ](https://www.pakutaso.com/)様の「[ものすごい数のバイクの列（ベトナムホーチミン）](https://www.pakutaso.com/20170628178post-12228.html)」を使用しています。
