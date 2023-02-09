# 動作テスト
LHP14LiteはQMK firmwareという、キーボード用のオープンソースファームウェアで動作します。  
私はwindows10でQMK MSYSとQMK Toolboxを使っておりますので、こちらを使った手順で説明します。
<br>
<br>
<br>

### １．QMK-MSYSのセットアップ

・[公式サイト](https://msys.qmk.fm/)からLatest versionのQMK_MSYS.exeをダウンロードします。

![](./images/alert1.png)

![](./images/alert2.png)

![](./images/alert3.png)

ダウンロード時、警告のメッセージが出ますが、赤丸部分をクリックしてダウンロードします。
<br>
<br>
<br>
・ダウンロードしたQMK_MSYS.exeを実行します。

![](./images/alert4.png)

![](./images/alert5.png)

警告が出ますが、インストールを進めていきます。
<br>
<br>
<br>

・QMK MSYSを起動します。   
　黒い画面が開き、＄が出たら、qmk setupと打ち込み、エンターを押します。

・設問が出ますが全てy(es)で答えます。

・cloning into...　と出てファイルのアップデートが始まりますが、終わるまで待ちます。

・QMK is ready to goと出て、＄の横にカーソルが出てきたらQMK MSYSセットアップ完了です！
<br>
<br>
<br>

### ２．QMK Toolboxのインストール

・[公式サイト](https://github.com/qmk/qmk_toolbox/releases)からqmk_toolbox_install.exeをダウンロードし実行します。  
同じように警告が出ますが、インストールを進めていきます。
<br>
<br>
<br>
### ３．テストファームの書き込み

・[LHP14ファームウェア置き場](https://github.com/LHPbackup/LHP14-firmware)からLHP14Liteのファームウェアをダウンロードします。  
　Codeと書いた緑のボタンを押し、Zipファイルをダウンロード、解凍します。

・C:\Users\ユーザー名\qmk_firmware\keyboards\に、lhp14liteフォルダをフォルダごとコピーしてください。

・QMK Toolboxを起動します。

・右上にあるAuto-Flashをチェックします。

![](./images/QMK_toolbox_lite.png)

<br>
<br>

・lhp1414liteフォルダ内のlhp14lite_test.hexをQMK Toolboxにドラッグ＆ドロップします。

![](./images/QMK_toolbox2_lite.png)

<br>
<br>

・PCにLHP14Liteをつなぎ、LHP14Liteのリセットボタンを押すとファームウェアが書き込まれます。

![](./images/reset_sw_lite.jpg)

<br>
<br>
<br>

### 4．動作テスト

・テストファームを書き込むとOLEDが光り、LEDが赤く光ります。

・OLEDの表示が「KEY TEST」になっていることを確認します。 キーを押して、文字が出てくれば正常。

・レイヤー変更キー（4行1列目）を押し、RGB LED TESTに切り替えてください。RGB変更（2行1列目）を押すとLEDの発光パターンが切り替わっていきます。LEDリセット（2行2列目）でLEDをリセットして全て赤に変わります。

![](./images/LED_TEST_lite.jpg)

・各キーの詳しい割り当ては\LHP14Lite\keymaps\Test\のkeymap.cを参照してください。

<br>
<br>
<br>

### 5．ジョイスティックの調整

・コントロールパネルのハードウェアとサウンドを左クリックします。

![](./images/calibration1.png)
<br>
<br>
<br>
・デバイスとプリンターを左クリックします。

![](./images/calibration2.png)
<br>
<br>
<br>
・LHP14Liteを**右クリック**します。

![](./images/calibration3.png)
<br>
<br>
<br>
・ゲームコントローラーの設定を左クリックします。

![](./images/calibration4.png)
<br>
<br>
<br>
・LHP14Liteを選択し、プロパティを左クリックします。

![](./images/calibration5.png)
<br>
<br>
<br>
・設定タブを選択して、調整を左クリックします。

![](./images/calibration6.png)
<br>
<br>
<br>
・次へを左クリックします。

![](./images/calibration7.png)
<br>
<br>
<br>
・次へを左クリックします。

![](./images/calibration8.png)
<br>
<br>
<br>
・あまり力を加えずに外周をなぞるようにスティックを軽く回します。
カーソルが安定したら次へを左クリックします。

![](./images/calibration9.png)
<br>
<br>
<br>
・次へを左クリックします。

![](./images/calibration10.png)
<br>
<br>
<br>
・完了を左クリックします。

![](./images/calibration11.png)
<br>
<br>
<br>
・ジョイスティックを動かし、カーソルが追従しているかチェックします。

ジョイスティック押し込みでボタン1が反応するかチェックします。

動作に問題なければOKを左クリックします。

![](./images/calibration12.png)
<br>
<br>
<br>

### お疲れ様でした。上手く動きましたか？？　

<br>
<br>


[ ＞＞キーマップを作る](./LHP14Lite_make_layer.md/) 

