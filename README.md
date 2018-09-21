# OpenAI Gym original environments
OpenAI Gymの自前環境の作成方法[参照](https://qiita.com/ohtaman/items/edcb3b0a2ff9d48a7def)

## 環境づくりの基本
1. gym.Envを継承し, 必要な関数を実装する
2. gym.envs.registration .register関数を使ってgymに登録する


## gym.Envを継承したクラスを実装する
gym.Envのクラスは以下のメソッドとプロパティを実装する必要がある

|メソッド|解説|
|:--|--:|
|_setp(self, action)|actionを実行し、結果を返す|
|_reset(self)|状態を初期化し、初期の観測値を返す|
|_render(self, mode='human', close=False)|環境を可視化する|
|_close(self)|環境を閉じて後処理をする|
|_seed(self, seed=none)|ランダムシードを固定する|
