# es6-study-4-13-29
JavaScript 学習コース IV > クラスの継承 > オーバーライド（1）

### オーバーライド
親クラスと同じ名前のメソッドを子クラスに定義すると、子クラスのメソッドが優先して使用される。
これは、子クラスのメソッドが親クラスのメソッドを上書きしていることから、オーバーライドと呼ばれる。
```
class Ahoge {
  info() {
  *******
  }
}

class Bhoge extends Ahoge {
  info() {
  *******
  }
}

const bhoge = new Bhoge("*******", "*******");
dog.info();

```
▲ 子クラスBhogeのinfoメソッドが呼び出される（オーバーライド）

## コーディングトレーニング
「ハウスM21」のレイアウト構造をレスポンシブで写経する。

#### サイト構造
- header > logo - nav/toggle
- main > section（p-index__mainVisual） - section（p-index__event） - section（p-index__news） - section（p-index__brand） - section（p-index__voice） - section（footer__own__wrap） - section（p-index__exhibition） - section（p-index__works）
- footer
- aside(※smartphoneのみ)

#### ブレイクポイント
- desktop（1200px ↑）
- tablet（1199px ↓）
- smartDevice（1023px ↓）

## チャレンジ
- ハンバーガーメニューに画像やSVGを使わずcssで描画する
- ヘッダーを上部固定にする
- スマホビューの時だけasideを表示し、ページ下部に固定する
