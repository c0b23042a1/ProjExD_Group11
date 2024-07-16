# GTC(Grand Theft Cash)

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
現金輸送車が落としていった現金を集めつつ、警察に捕まらないように、周囲の乗用車を避けるゲーム。

## ゲームの遊び方
* 十字キーで加減速、上下移動をする。
* 乗用車にぶつかればゲームオーバー。
* 現金にぶつかればスコアアップ。

## ゲームの実装
### 共通基本機能
* 背景画像と主人公キャラクターの描画が同じ速度で横に移動する
* 十字キーの上下で上下に移動し、左右で加減速する

### 担当追加機能
* 敵にぶつかった時に残機が減り、一定時間無敵になってエフェクトが出る(武田)
仮で不動の敵を出現させ、ぶつかった時に残機が減り、500フレーム無敵状態になり、無敵中は半透明になるようにした
仮のため、ぶつかった時に敵は消えないため、マージの後手動で変更する
* スコアを表示する
* BGMと現金を取った時のSEを出す　（馬場）
* 背景と自キャラを変える。　（馬場）
* 現金毎にスコアを変える(川嶋)
* 敵とアイテムがランダムで出現する(川嶋)
* ゲームオーバー画面の表示(武田)
仮で600フレーム後にゲームオーバー画面を表示するコードを作成した
仮のため、本実装ではゲームオーバーになった時にこのコードをコピペする


### ToDo
--各自担当の追加機能を作成する

### メモ
* クラス内の変数は，すべて，「get_変数名」という名前のメソッドを介してアクセスするように設計してある
* 変数の表記方法は初期状態の変数名を参考に決定する
