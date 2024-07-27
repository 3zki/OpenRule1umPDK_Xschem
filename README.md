# OpenRule1umPDK_Xschem

## これは何
* OpenRule1umPDK (PTS06) の回路図作成およびシミュレーションをXschem上で行うためのPDKです。
* 秋田先生による diode.lib, mos.lib を使ってngspice上でのシミュレーションが可能です。
** https://github.com/MakeLSI/Measure の 16PTSを参照
* WとLを入れるだけで抵抗/容量が設定できるようにR+Cモデル(passive.lib)を追加しています。
** 未完成です。 TODO: diff_cap のモデル改良
* スタンダードセルもネットリストがあるのでngspice上でシミュレーションが可能です。
** 一応klayoutでのLVSを意識したつくりにしてあります。

## 内容物
* xschemrc : xschemrcのサンプル
* title_PTS06.sch : 表紙
* lib : シミュレーションモデルとスタンダードセルのネットリスト
* symbols/OR1 : プリミティブ(FET, R, C, diode)シンボルとスタンダードセルシンボル
* klayout : xschemのLVS回路図を使ってLVSをするための変換マクロ。.klayout/macroに配置。Linux環境用。

## Author
Junichi Akita (@akita11), Mizuki Mori (@3zki), ISHI-kai (@ishi-kai)