# GNN_Introduction
GNNの勉強の取っ掛かりとしておすすめの資料をまとめました。

## 論文
[A comprehensive survey on graph neural networks](https://arxiv.org/abs/1901.00596)
Zonghan Wu, Shirui Pan, Fengwen Chen, Guodong Long, Chengqi Zhang, and Philip S. Yu, IEEE transactions on neural networks and learning systems (2020).
通常のGNNモデルだけでなく、グラフを生成するGraph Autoencoderや時系列データを扱うSTGNNなどを含めて、GNNの各手法を幅広く網羅しているサーベイ論文。
GNNの応用についても詳しく述べられている。

[Neural message passing for quantum chemistry](https://arxiv.org/abs/1704.01212)
Justin Gilmer, Samuel S. Schoenholz, Patrick F. Riley, Oriol Vinyals, and George E. Dahl, ICML 2017.
GNNの各手法を統一的に説明するMessage Passingというフレームワークを提案。
まず各ノードが隣接ノードの情報を集め（Message function）、次に集めた情報を利用して各ノードの特徴量をアップデートし（Update function）、それをT回繰り返して各ノードの高次の特徴量を得る。
グラフごとに値を出力するタスクの場合は、Readout functionを用いて各ノードの特徴量ベクトルからグラフ全体を表す特徴量ベクトルを計算する。

[Semi-supervised classification with graph convolutional networks](https://arxiv.org/abs/1609.02907)
Thomas N. Kipf and Max Welling, ICLR 2017.
現在最も広く利用されているGNNモデルであるGCNを提案。
2章"FAST APPROXIMATE CONVOLUTIONS ON GRAPHS"では、従来のスペクトルベースのGNNモデルからGCNモデルを導出しているが、いきなり理解するのは難しいので最初は飛すことをおすすめする。

## ライブラリ
[PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/)
PyTorchベースのGNNライブラリ。様々なGNNモデルの実装が提供されている。
公式の[Introduction](https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html)から始めるのがおすすめ。


