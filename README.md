# Creator's Analog Clock

https://user-images.githubusercontent.com/67828511/184906888-cf0eaa7c-5e67-4d69-b9fc-3b16e8aae22d.mp4

## ◇ ダウンロード
- [CreatorsAnalogClock.zip](https://github.com/into-vision/AnalogClock/raw/main/archive/analog_clock1_0_0.zip)

## ◇ 目指したもの

- OBS上に簡単に設置可能  
- 奥行きのある壁にもフィットさせられる  
- **文字盤 および 時計の針 の画像をTwitterで募集できるように想定**  

## ◇ 画像の作り方

- 文字盤 および 時計の針 の画像はそれぞれ 512x512px を想定しています。
- ガイドライン画像に沿ったパーツ配置なら解像度は自由ですが、Twitter投稿する際は 512x512px にしたほうが良いです(後述)
- もちろん高解像度で作っておいて利用する際は 512x512px に縮小しても大丈夫です。
- 作った画像はサンプルページにて画像をドラッグアンドドロップすることで即座にチェックできます。
  - サンプルページ：http://intovision.sakura.ne.jp/public/analog_clock/
- 後段のTIPSも先に見ておくことをおすすめします。

## ◇ Twitterで画像を投稿する場合

- Twitterに投稿する際は透過pngで投稿することになりますが、その際に条件を満たさないと不透明jpgに変換されてしまいます。
- 詳細は「twitter 透過 フローチャート」などで検索していただくのが良いです。
- とりあえず 512x512px の解像度で作っておけば大抵の場合うまくいくはずです。
  - ちなみにDMで送る場合は常に不透明jpgに変換されてしまうようです。  
プライベートでやり取りする場合にご注意下さい。

## ◇ OBS上での使い方

https://user-images.githubusercontent.com/67828511/184910012-e9bc9ce2-6501-4f25-84ab-28aca5e32b34.mp4

1. 以下のファイルをダウンロード
   - [CreatorsAnalogClock.zip](https://github.com/into-vision/AnalogClock/raw/main/archive/analog_clock1_0_0.zip)
2. お使いの配信素材フォルダに解凍
3. OBSの下らへんにあるソース/+(追加)/ブラウザを選択
4. 「ローカルファイル」をチェック
5. 「参照」から解凍したファイルのindex.htmlを選択
6. 幅 1024 / 高さ 512 を指定
7. Altキーを押しながら右の赤点を動かして右半分を切り取る
8. AnalogClockを右クリックし「対話」を選択して角度などを調整

## ◇ TIPS

- Q.針や文字盤の縁に変な色が出る/黒っぽい縁が出る
  - A.画像の縁は時計の傾きや大きさによって周囲のピクセルを混ぜるようにして縮小されます。  
ピクセルのRGBAが(255,255,255,255)、隣接する透明部分が(0,0,0,0)だと半透明グレーになります。  
イラストソフトによってはRGBAのAlpha値が0の場合、RGB値を勝手に変更する場合があります。  
それによって意図しない色や黒っぽい縁が出てしまう場合があります。  
その場合はGIMPなどのカラーチャンネルを分解できるイラストソフトを利用して  
Alpha値が0の部分のRGBを書き換えることで抑制できます。  
- Q.動く振り子を付けたい
  - A.ループ再生する振り子の動画を作ってその上にこのツールを載せるのが良いです。
- Q.シーンごとに別の画像を使いたい
  - A.AnalogClockを複製してそれぞれ画像を変えて置いておくのが良いです。  
その際、フォルダ名を変えることで設定をそれぞれ保持することができます。  
参考として以下のようなフォルダ構成を想定しています。  
    - 配信素材フォルダ
      - AnalogClock_Aさん作
        - index.html
        - dial.png
        - hand.png
      - AnalogClock_Bさん作
        - index.html
        - dial.png
        - hand.png
- Q.配信画面に設置するとジャギが出る
  - 配信で使用する場合は場合によっては非常に小さいサイズで利用される場合があります。  
例えば背景にある小物の時計に当てはめる場合などです。  
小さいかつ斜めに配置とかだとさらにジャギが出やすいです。  
![2022y08m15d_152932732](https://user-images.githubusercontent.com/67828511/184659735-5bc20c13-d237-4a53-bda8-37420c68140d.png)
![2022y08m15d_154835832](https://user-images.githubusercontent.com/67828511/184659814-e0644242-7a44-4627-83f5-c4974b06a366.png)  
※1枚目の画像は長針と秒針が削れている  
その想定で利用される場合は画像作成時に時計の針や意匠を少し太めにしておくと良いです。  
それか予め斜めにした状態で文字盤等を背景に描き込んでおいて、時計の針だけあとからはめ込むというのも手です。

## ◇ 注意事項

- 個人/企業/Youtuber/Vtuber 問わず配信者ならどなたでも無償でご利用いただけます。
- 利用に際しましては本ツールの製作者(バイザン)を明記する必要はありません。
- 画像自体の著作権は画像の作成者/著作権者に帰属します。  
各配信者向けに作られたファンメイドの画像を勝手に利用しないように！  
それでも利用したい場合はその画像の著作権者に許可を取って下さい。  
  - サンプルで同梱しているdial.pngとhand.pngはそのまま配信でご利用いただいても構いません。
- 使用に際してこのツールの改造などはご自由に行っていただけます。  
  - ただし再配布は禁止とさせていただきます(グループ内や閉鎖空間での共有はその限りではありません)
- 作成者を騙ったり、公序良俗に反する使い方などは禁止します。
- 利用に際して発生した問題に関して、このツールの作成者は一切の責任を負いかねます。
- **実際に配信で使用されるかどうかは配信者の裁量になります。**
  - 使われなくても「そういう時もあるさ」の精神でいましょう。

## ◇ 更新履歴
- 2022/08/26 注意事項をもう少し詳しく追記
- 2022/08/26 v1.0.0 初版公開

## ◇ クレジット

- 製作者：バイザン🐈([@into_vision](https://twitter.com/into_vision))
  - なにか欲しい機能やバグ報告とか有ったらリプしてね！
