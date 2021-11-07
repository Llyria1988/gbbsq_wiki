# アノテーションのためのソフトウェア環境セットアップ 

### Squidle+について
**Squidle+** を利用することで、**生物学的な画像記録データに対し様々なワークフローやモードでアノテーションすることが可能になります。**　例）フレーム全体、ポイント、ポリゴン、バウンディングボックス、アノテーションごとにタグ付けやコメントなどを複数ラベル付与すること。

### Squidle+ と SquidvidPRO
北極データセットのアノーテーションには **Squidle+** と **SquidvidPRO** の両方を使用します. **Squidle+** は、画像へのアノテーションやタグ付けに特化したソフトウェアです。 **SquidvidPRO** はビデオキャプター機能を持ったビデオプレーヤーで、キャプチャー画像を **Squidle+** に送る機能なども備えています。

### Set up Annotation

Let's start setting up your annotation environment!

#### 1. Logging into Squidle+: 
   1. Click the Squidle+ icon and open the app
   ![Squidle+](../images/4_SquidleApp_1.png)

   1. Click **Log in >>**
   ![Log in](../images/5_SquidleApp_2.png)

   1. Log in in with your **username**
   Your username is already prepared in advance.
   Ask it from the representatives in GODAC or decide which username you should use in the annotation group.
   ***Each annotator has to have their own username.**
   **Example)**
   `Email or usename: GodacOne`
   `Password: godac`
   ![User account](../images/6_Login_1.png)

   1. Open **Frameplay GUI**
   Now you are logging in. Open **Frameplay GUI** next
   ![FrameplayGUI1](../images/7_FrameplayGUI_1.png)
   You can see the window below and now you are ready for the next step
   ![FrameplayGUI2](../images/8_FrameplayGUI_2.png)
   
#### 2. Open SquidvidPRO
   1. Shrink the window size of the **Frameplay GUI** as below
   ![FrameplayGUI3](../images/9_FrameplayGUI_3.png)

   1. Open **SquidvidPRO**
   ![SquidvidPRO](../images/10_SquidvidPROApp_1.png)
   Then a line **SquidvidPRO** & **Frameplay GUI** windows as below
   ![SquidvidPRO and Frameplay GUI](../images/11_SquidvidPROApp_and_FrameplayGUI_1.png)

#### 3. Getting API TOKEN and SquidvidPRO SETUP
   1. Get **API TOKEN**
   Click the **Key** icon just next to your username on **Frameplay GUI**
   ![API TOKEN](../images/12_SquidvidPROApp_and_FrameplayGUI_2.png)

   1. Copy **API TOKEN** to **SQ+ API Key:** on SquidvidPRO SETUP
   ![SquidvidPRO API TOKEN](../images/13_SquidvidPROApp_and_FrameplayGUI_3.png)
   
   1. Load log file
   Loading Arctic ROV dive logfile from your HDD into **Logfile path:**
   In this case the file name is **HLY1601_full_NO_altitude.gbb.csv**
   ![SquidvidPRO_setup_1](../images/14_SquidvidPRO_setup_1.gif)
   
   1. Load video file 
   Loading a video file from your HDD into **Video path:**
   ![SquidvidPRO_setup_2](../images/15_SquidvidPRO_setup_2.PNG)

   1. Fill out **Video start time:** and **Camera code:** from **Video path:**
      1. For the **Video start time:**, refer to the characters just before `.mov`. You can find numbers and characters as **`2016xxxTxxxxxx.xxxxZ`**. Copy the numbers **just before Z** and paste them to **Video start time:**.
      2. For the **Camera code:**, refer to the `camera_type-camera_angle-camera_resolution` in the video file name (e.g. 4K-pantilt-4K30p). Copy the characters to **Camera code:**.
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
