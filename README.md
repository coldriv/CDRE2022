# 🚀 CDRE2022
_Change Detection dataset specialized for Riverbank Erosion 2022_  

河岸侵食に特化した**教師なし変状検知・異常検知**のための河川CCTVカメラ画像のデータセットです。  
実際の河岸侵食の画像セットはまだ少ないですが、大規模なデータセットとして蓄積されていくきっかけになることを期待して公開するものです。  

![Badge Status](https://img.shields.io/github/license/coldriv/CDRE2022)
![Badge Status](https://img.shields.io/github/issues/coldriv/CDRE2022)
![Badge Status](https://img.shields.io/github/stars/coldriv/CDRE2022)

***
## 🌐 Downloads
[Gドライブ](https://drive.google.com/drive/folders/19umRFXrMD4XkN_EzdHu3Vn1FoGj8bLk8?usp=sharing)
で共有しています。

> フォルダ構成 
>> 640_512_0（学習用：河岸侵食なし）  
>> 640_512_1（学習用：河岸侵食なし）  
>> 640_512_2（検証用：河岸侵食あり）  

tar.gzで圧縮されているので、ダウンロード後に解凍してください。

    $# Linuxの場合は以下のコマンドで解凍できます。
    $tar -zxvf *.tar.gz


***
## 👀 データセットの内容
学習用のデータセット（「640_512_0」「640_512_1」）は同じ画角の様々な地点の画像が同一のフォルダに格納されています。  
検証用のデータセット（「640_512_2」）は今のところ2画角のみです。
河岸侵食なし（「t0」）と河岸侵食あり（「t1」）にフォルダが分かれており「t1」には侵食箇所のマスク画像も格納されています。
画像はすべて512×640ピクセルに成形してあります。  

- 「640_512_0」の例：
![png](https://github.com/coldriv/CDRE2022/blob/main/img/sample_640_512_0.png)

- 「640_512_1」の例：
![png](https://github.com/coldriv/CDRE2022/blob/main/img/sample_640_512_1.png)

- 「640_512_0」「640_512_1」の整理状況：
![png](https://github.com/coldriv/CDRE2022/blob/main/img/count.png)

学習用のデータセット（「640_512_0」「640_512_1」）は322画角で合計86,862枚の画像が格納されています。
※同じCCTVカメラでも画角が著しくことなる場合は別カテゴリとしています。

- 「640_512_2」の例：
![png](https://github.com/coldriv/CDRE2022/blob/main/img/sample_640_512_2.png)
枚数構成は以下の通りです（T0：侵食なし、T1：侵食あり）。  
  |  | T0 | T1 |
  |:---:|:---:|:---:|
  | obihiro | 43 | 80 |
  | otofuke | 1 | 214 |

***
## 🔨 ToDo
- [ ] 英語版レポジトリの整備  
- [ ] 河岸侵食画像の追加（随時） 
- [ ] 自動でデータセットを追加できる機能の整備   
- [ ] Webスクレイパー公開  
- [ ] 教師なし変状検知モデルの公開（別レポジトリを想定）  

***
## 💬 Author
- [国立研究開発法人　土木研究所　寒地土木研究所](https://www.ceri.go.jp/)
- [いであ株式会社](https://ideacon.jp/)

***
## 🌏 License
MIT License
