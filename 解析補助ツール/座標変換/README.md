# 座標変換計算シート
空間中の座標変換を計算するExcel  

## 理論
座標変換について - [wikipedia](https://ja.wikipedia.org/wiki/%E5%9B%9E%E8%BB%A2%E8%A1%8C%E5%88%97)  

## Cradleでの利用方法
Cradleでタイヤを回転させて解析したいとき、  
必要なパラメータは「回転軸座標」と「回転軸」の２種類。  
このそれぞれは下図のようなイメージで捉えることができる。

![fig_geometry](https://github.com/KIT-formula/Cradle/blob/image/fig_geometry.JPG)

ここで、タイヤに舵角がついていた場合は次のように処理すれば良い。  

1. タイヤの回転中心座標（x,y,z）をCradleに入力する。
2. タイヤの傾きをゼロとしたときの回転軸（x,y,z）を0 or 1で入力する。
3. 傾き角（pitch, roll, yaw）を入力する。
4. 出力された変換後座標を舵角が付いたときの回転軸(x,y,z)としてCradleに入力する。

解析結果
![fig_cradle](https://github.com/KIT-formula/Cradle-notes/blob/image/fig_cradle.jpg)
