# joboji_campus

テーマ:画像処理

## 4/28
githubの設定  
clone,commit,pushできたことを確認  

## 5/12
選択回数 : 16パズルなら2回  
受け取りフォーマット : 配列?

## 並べ替え案
1. 
<div align="center"><img src="image/案1.jpg" width="300"></div>

2. 
<div align="center"><img src="image/案2.jpg" width="300"></div>

~~こっちの方がいい気がする~~


3. 
<div align="center"><img src="image/案3.jpg" width="300"></div>

これ!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!  

## restore.ipynb
~~4x4の配列で座標を所得するだけ~~  
~~選択した値を座標移動させたい値の上まで移動させる(途中)~~  
選択した値(16)を上下左右に動かす関数  
最後の2行値を除く、動かしたい値が下端にあるとき以外の移動はできた  

* 移動方法
<div align="center"><img src="image/移動方法1.jpg" width="300"></div>
<div align="center"><img src="image/移動方法2.jpg" width="300"></div>

### to do
* up, down, right, leftの関数が 4x4 にしか対応してない
* 変数名のリファクタリング
* txtの行数、列数を反映させる

## slide_puzzle.ipynb
新しいファイルで作り直す  

### 使用変数
* puzzle_board → パズル盤面
* column → 列
* row → 行
* select_cost → 選択コスト
* select_times → 選択回数
* exchange_operation → 交換操作
* fixed_value → 並び替え済みの値
<br>

* selection_value → 選択値
* selection_coord → 選択値の座標
* selection_position → 選択値の初期座標
* target_value → 動かしたい値
* target_coord → 動かしたい値の座標
* x, y → coord[1], coord[0]


### 変数名変更
* (パズル盤面)split_list → puzzle_board
* (列)row → column
* (行)columns → row
* (交換回数)exchange_num → exchange_times
* (選択値)choice_num → selection_value
* (選択値の座標)choice_pos → selection_coordinate
* (動かしたい値)target_num → target_value
* (動かしたい値の座標)target_pos → target_coordinate
* (targetを置きたい座標)pos → coord


