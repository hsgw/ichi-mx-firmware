# ichi MX ファームウェア

ichi MXキーボード用のカスタムファームウェアです。   
CH55xduinoを使用し、QMK VIAプロトコルと互換性があります。

## 特徴

- CH552eマイコン対応
- QMK VIAプロトコル互換
- キーマップのカスタマイズ可能
  - レイヤー機能やマクロ機能は使えません。単純なキーマップ書き換えだけが使用可能

## キーマップのカスタマイズ

VIAを使用してキーマップをカスタマイズできます。デフォルトのキーマップはEnterキーに設定されています。

Remapを使用してキーマップをカスタマイズするには、以下の手順を参考してください。

1. ichi MXをUSBケーブルで接続する
2. Remapを開いて`ichi MX`を開く
3. jsonファイルを読み込ませる   
   [ichi_mx.json](ichi_mx.json)
4. キーマップを変更する
   - 変更できるレイアウトは単純なキーへの書き換えのみです
   - レイヤー・ホールドタップ・マクロ機能などには対応していません


## ビルド環境のセットアップ

以下のページを参照してch55xduinoの環境をセットアップします
- https://github.com/DeqingSun/ch55xduino
- https://qiita.com/akita11/items/d7baed4ca3c06e292637

## 書き込み

ichi MXをブートローダーモード(書き込みモード)にする必要があります。   
USBケーブルを抜いて、BOOTのパッドをショートさせながらUSBケーブルを指し直します。


## ライセンス

(c) 2025, Takuya Urakawa, 5z6p Instruments

GNU Lesser General Public License v2.1   
https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html

## クレジット

Based on the HID Keyboard & Mouse implementation for CH55xduino by Deqing Sun.

https://github.com/DeqingSun/ch55xduino