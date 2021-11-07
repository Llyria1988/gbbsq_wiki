# アノテーションのためのソフトウェア環境セットアップ 

### Squidle+について
**Squidle+** を利用することで、**生物学的な画像記録データに対し様々なワークフローやモードでアノテーションすることが可能になります。** <br>
例）フレーム全体、ポイント、ポリゴン、バウンディングボックス、アノテーションごとにタグ付けやコメントなどを複数ラベル付与するこ

### Squidle+ と SquidvidPRO
北極データセットのアノーテーションには **Squidle+** と **SquidvidPRO** の両方を使用します。**Squidle+** は、画像へのアノテーションやタグ付けに特化したソフトウェアです。 **SquidvidPRO** はビデオキャプター機能を持ったビデオプレーヤーで、キャプチャー画像を **Squidle+** に送る機能なども備えています。

### アノーテーション環境をセットアップする

アノテーション環境のセットアップを始めましょう!

#### 1. Squidle+にログインする: 
   1. Squidle+ アイコンをクリックしアプリを起動します。<br>  
   ![Squidle+](../images/4_SquidleApp_1.png)

   1. **Log in >>** をクリックしてください<br>  
   ![Log in](../images/5_SquidleApp_2.png)

   1. **username** でログインする<br>
   あなたの username はすでに準備されてます。
   GODACの担当者に問い合わせるか、アノテーションチームの中で誰がどのusernameを使用するかを決めてください。  
   ***それぞれのアノテーターは個別のユーザーネームを使用してください。***
   ***例)***
   `Email or usename: GodacOne`
   `Password: godac`<br>
   ![User account](../images/6_Login_1.png)

   1. **Frameplay GUI** を開く
   現在あなたはログインしています。次に **Frameplay GUI** を開きましょう。<br>
   ![FrameplayGUI1](../images/7_FrameplayGUI_1.png)
   下のようなウィンドウが見えていたら次へのステップへ進みます。<br>
   ![FrameplayGUI2](../images/8_FrameplayGUI_2.png)
   
#### 2. SquidvidPRO を開く
   1. 下のように **Frameplay GUI** のウィンドウを小さくします<br>
   ![FrameplayGUI3](../images/9_FrameplayGUI_3.png)

   1. **SquidvidPRO** を開きます<br>
   ![SquidvidPRO](../images/10_SquidvidPROApp_1.png)
   **SquidvidPRO** と **Frameplay GUI** のウィンドウを以下のように並べます<br>
   ![SquidvidPRO and Frameplay GUI](../images/11_SquidvidPROApp_and_FrameplayGUI_1.png)

#### 3. API TOKEN を取得し SquidvidPRO をセットアップする
   1. **API TOKEN**を取得
   **Frameplay GUI** のウィンドウの、ユーザー名のすぐ隣にある**Key** アイコンをクリックします。<br>
   ![API TOKEN](../images/12_SquidvidPROApp_and_FrameplayGUI_2.png)

   1. **API TOKEN** をSquidvidPRO SETUP の **SQ+ API Key:** にコピーします。（選択項目のドラッグ＆ドロップでもコピーペースト可能です。）<br>  
   ![SquidvidPRO API TOKEN](../images/13_SquidvidPROApp_and_FrameplayGUI_3.png)
   
   1. ログファイルのロード
   ハードディスクから **Logfile path:** へログファイルをろロードします。
   今回のアノテーションでは、ログファイル名はすべて **HLY1601_full_NO_altitude.gbb.csv**　になります。<br>
   ![SquidvidPRO_setup_1](../images/14_SquidvidPRO_setup_1.gif)
   
   1. ビデオファイルをロードする
   ハードディスクから **Video path:** へビデオファイルをロードします。<br>
   ![SquidvidPRO_setup_2](../images/15_SquidvidPRO_setup_2.png)

   1. **Video start time:** と **Camera code:** を **Video path:** から取得
      1. **Video start time:** は、ファイル名の末尾にある`.mov`の直前の項目を引用します。 それらは **`2016xxxTxxxxxx.xxxxZ`** のよう記述されています。**Zの直前までの** の文字列を **Video start time:** の項目にコピーペーストして下さい。（選択項目のドラッグ＆ドロップでもコピーペースト可能です。）
      1. **Camera code:** は、ファイル名の `camera_type-camera_angle-camera_resolution` (例： 4K-pantilt-4K30p) の項目を引用します。 これらを **Camera code:**　にコピーペーストして下さい。（選択項目のドラッグ＆ドロップでもコピーペースト可能です。）<br>
      ![SquidvidPRO_setup_3](../images/16_SquidvidPRO_setup_3.gif)

   1. Fill out **Platform** and **Campaign** from **Deployment**
      You can usually pick them by the pull-down menu.
      1. The **Platform** is always ought to be set as **GlobalExplorer** in this Arctic annotation task. 
      2. **Campaign** is also always ought to be set as **HLY1601**. 
      3. Only **Deployment** will be changed depending on which movie file you picked. Check the head of the file name.
      ![SquidvidPRO_setup_4](../images/17_SquidvidPRO_setup_4.png)  

   1. Now you are all set on SquidvidPRO and press **OK**
      Once you press **OK**, the **Deployment** will be loaded.
      Then you click **â–¶ï¸Ž** mark of SquidvidPRO the video will be played. 
      ![SquidvidPRO_setup_5](../images/18_SquidvidPRO_setup_4.gif)
   
   1. **Media collection** and **Annotation set**
   Select the **Media collection** and **Annotation set** on Frameplay GUI.
   Now you are ready for Annotation!!
   ![Frameplay_setup_1](../images/19_Frameplay_setup_1.png)
