# gsi-dem-slice
国土地理院標高タイルを使った valhalla elevation service API の部分実装とデモ

## Demo

<http://frogcat.github.io/gsi-dem-slice/>

* 画面下部に二点間の標高変化が折れ線表示される
* マーカードラッグで更新


## Note

* 緯度経度群から標高配列を求めるための elevation 関数を定義している
* <https://github.com/valhalla/valhalla-docs/blob/master/elevation-service.md> の部分実装
* 内部では 10mメッシュ [標高データ・国土地理院](http://maps.gsi.go.jp/development/demtile.html) を XHR で取得
* ブラウザ純正 Promise を使っているので、IE 系は動作対象外 <http://caniuse.com/#search=promise>



