# IMS (国際化マルチシフト)キーボード

[readme_ENGLISH](https://github.com/pinekz/qmk_firmware/blob/IMS-module/keyboards/ymdk/ymd40/air40/keymaps/via_ims_air40/readme_IMS_en.md)  

ver. 2.6 :2026/10/18 親指キー押しっぱなしでの連続シフト機能の導入 
ver. 2.5 :2026/10/10 主要部の state machine 化とプロセスの整理  
ver. 2.0 :2026/07/26 QMK 0.33.0  
ver. 1.0 :2026/06/26 QMK 0.27.0  

<img width="1920" height="1440" alt="Aatreus" src="https://github.com/user-attachments/assets/1b391ce7-3524-44e8-8ec8-26d49f49ba2e" />

これは、QMKとViaを基本とした日本語かな入力用のモジュールです。
自然な日本語入力のための「親指シフト」入力環境を発展させて、via利用での自由な文字配置を実現します。
同時に、入力レイヤを拡張するためのシフトキーを自由に選択・追加することで、「親指シフト」に限定されない独自のシフト入力を提供します。

## 機能

1. このモジュールを使って英語・各国語キーボードに参照用言語レイヤーを追加し、固有の言語文字を自由に配置することができます。
   (viaにカスタムキーコードをインポート)
2. 日本語レイアウト(JP layout)でも、英語キーボードの記号を見たままに入力可能です。
3. 英字とモディファイアキーを併用するショートカットキー操作や、英数・記号レイヤへの移動は、仮想言語レイヤー使用中にも自由に可能です。
4. 固有の言語が日本語である場合、IME(Input Method Editor)で使用する操作キーを透過する為、QMKキーボードでかな(表音)文字入力、PC側のIMEでかな漢字(表意文字)変換という分担操作が自然に実現され、既存のIMEと自由に連携することが可能です。
5. IME_monitorをPC側で動作させることで、モードずれのないストレスフリーな運用が可能です。

## 特徴

1. viaのWeb操作画面を利用して、既存のキー配置に限定されない個々人用の文字キー配置が可能です。
   (独自のかな配列開発ができます)
2. 同時押しキーを自由に配置することで、事故で親指を欠損した場合でも他の指で代替することが可能です。
   (親指シフトに限定されない日本語入力システムを構築可能です)
3. 固有言語部分を `language.c` と header に独立させて、開発の効率化を図っています。

## 実装済み キーボード

[YMDK Air40](https://github.com/pinekz/qmk_firmware/tree/IMS-module/keyboards/ymdk/ymd40/air40/keymaps/via_ims_air40)  
[Keyboardio Atreus](https://github.com/pinekz/qmk_firmware/tree/IMS-module/keyboards/keyboardio/atreus/keymaps/via_ims_Atreus)  
