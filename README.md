# FUTABA_CANServo_Updater  

本アプリケーションでは、DroneCAN対応サーボ（BLAシリーズ：BLA21-**U、BLA15-**U等）のファームウェアアップデートを行うことが可能です。   
アプリケーションを使用する際は、実行ファイル(FUTABA_CANServo_Updater_V1.0.4.exe)をダウンロードして実行してください。  
アプリケーションの使用方法およびファームウェアアップデートの手順は以下のマニュアルをご確認ください。  
This application allows you to update the firmware for DroneCAN-compatible servos (BLA series: BLA21-**U, BLA15-**U, etc.).  
To use the application, download and run the executable file (FUTABA_CANServo_Updater_V1.0.4.exe).  
Please refer to the following manual for instructions on how to use the application and firmware updates.  
<br>
* [FUTABA_CANServo_Updater_マニュアル_Rev1.00.pdf](https://github.com/FutabaCorp/FUTABA_CANServo_Updater/blob/main/FUTABA_CANServo_Updater_%E3%83%9E%E3%83%8B%E3%83%A5%E3%82%A2%E3%83%AB.pdf)　（Japanese）
* [FUTABA_CANServo_Updater_Manual_Rev1.00.pdf](https://github.com/FutabaCorp/FUTABA_CANServo_Updater/blob/main/FUTABA_CANServo_Updater_Manual.pdf)　（English）
<br>

アップデートに使用するbinファイルは以下のフォルダに保存されています。  
アップデート対象の機種名が記載されたフォルダ内のbinファイルをご利用ください。  
The bin file used for the update is saved in the following folder.  
Please use the bin file in the folder containing the name of the model to be updated.  
<br>
[update_bin_files](https://github.com/FutabaCorp/FUTABA_CANServo_Updater/tree/main/update_bin_files)
<br>
<br>
DroneCAN対応サーボとPCの接続にはスターターキット（DroneCAN対応サーボ用）をご利用ください。  
Please use the Starter Kit (for DroneCAN-compatible servos) to connect a DroneCAN-compatible servo to a PC.  
https://www.futaba.co.jp/product/industrial_servo/servo/lineup/starter-kit
<br>
<br>

### サーボファームウェアバージョン管理表

| Ver | 機種(期間) | 変更内容 |
| :---: | :--- | :--- |
| 1.010 | ・BLA21-\*\*U-A0* (2021/1\~2023/12)<br>・BLA15-06U-A01 (2021/5\~2023/12) | ・新規ファームウェア |
| 1.100 | ・BLA21-\*\*U-AB2 (2021/10~2022/4) | ・速度/トルク制御 ON/OFF機能実装 [0x25]<br> デフォルトは速度/トルク制御はOFF（速度/トルク制御不可）<br>・過電流保護機能実装 [0x2A]<br>・PWM入力設定機能実装 [0x34]\~[0x37]<br>(PWM入力対応機種のみ) |
| 1.200 | ・BLA21-\*\*U-AB2 (2022/5\~2023/12)<br>・BLA15-12U-A01 (2022/9\~2023/12) | ・[0x2F] 角度制御　ブースト機能実装 |
| 1.300 | ・BLA21-\*\*U-A**<br>・BLA15-**U-A01<br> (2024/1\~) | ・動作改善 |
| 1.400 | ・BLA21-\*\*U-A**<br>・BLA15-**U-A01<br> (2024/6\~) | ・低速動作時にサーボがストールする不具合を修正 |

### Servo firmware version management table

| Ver | Model (Period) | Changes |
| :---: | :--- | :--- |
| 1.010 | ・BLA21-\*\*U-A0* (1/2021\~12/2023)<br>・BLA15-06U-A01 (5/2021\~12/2023) | ・New firmware |
| 1.100 | ・BLA21-\*\*U-AB2 (10/2021~4/2022) | ・Implementation Speed/Torque Control ON/OFF [0x25].<br> Speed/Torque Control is OFF by default.<br>・Implementation Overcurrent protection [0x2A].<br>・implementation PWM input setting [0x34] to [0x37].<br>(Only for models that support PWM input) |
| 1.200 | ・BLA21-\*\*U-AB2 (5/2022\~12/2023)<br>・BLA15-12U-A01 (9/2022\~12/2023) | ・Implementation Angle control Boost [0x2F]. |
| 1.300 | ・BLA21-\*\*U-A**<br>・BLA15-**U-A01<br> (1/2024\~) | ・Improved behavior |
| 1.400 | ・BLA21-\*\*U-A**<br>・BLA15-**U-A01<br> (6/2024\~) | ・Fixed a bug that caused the servo to stall during low speed operation. |

### アプリケーションバージョン管理表

| Ver | 変更内容 |
| :---: | :--- |
| 1.0.4 | ・新規アプリケーション |
| 1.0.5 | ・BLA15-**Uシリーズにて、アップデート時に一部パラメータの初期値が変わる不具合を修正 |

### Application version management table

| Ver | Changes |
| :---: | :--- |
| 1.0.4 | ・New applications |
| 1.0.5 | ・Fixed an issue where the initial values ​​of some parameters in the BLA15-**U series changed when updating. |
