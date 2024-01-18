# FUTABA_CANServo_Updater  

本アプリケーションでは、DroneCAN対応サーボ（BLAシリーズ：BLA21-**U、BLA15-**U等）のファームウェアアップデートを行うことが可能です。   
アプリケーションの使用方法およびファームウェアアップデートの手順は以下のマニュアルをご確認ください。
<br>
* [FUTABA_CANServo_Updater_マニュアル_Rev1.00.pdf](https://github.com/FutabaCorp/FUTABA_CANServo_Updater/blob/main/FUTABA_CANServo_Updater_%E3%83%9E%E3%83%8B%E3%83%A5%E3%82%A2%E3%83%AB_Rev1.00.pdf)　（Japanese）
* [FUTABA_CANServo_Updater_Manual_Rev1.00.pdf](https://github.com/FutabaCorp/FUTABA_CANServo_Updater/blob/main/FUTABA_CANServo_Updater_Manual_Rev1.00.pdf)　（English）
<br>

アップデートに使用するbinファイルは以下のフォルダに保存されています。  
アップデート対象の機種名が記載されたフォルダ内のbinファイルをご利用ください。
<br>
[bin](https://github.com/FutabaCorp/FUTABA_CANServo_Updater/tree/main/bin)
<br>

### ファームウェアバージョン管理表

| Ver | 機種(期間) | 変更内容 |
| :---: | :--- | :--- |
| 1.010 | ・BLA21-\*\*U-A0* (2021/1\~2023/12)<br>・BLA15-06U-A01 (2021/5\~2023/12) | ・新規ファームウェア |
| 1.100 | ・BLA21-\*\*U-AB2 (2021/10~2022/4) | ・速度/トルク制御 ON/OFF機能実装 [0x25]<br> デフォルトは速度/トルク制御はOFF（速度/トルク制御不可）<br>・過電流保護機能実装 [0x2A]<br>・PWM入力設定機能実装 [0x34]\~[0x37]<br>(PWM入力対応機種のみ) |
| 1.200 | ・BLA21-\*\*U-AB2 (2022/5\~2023/12)<br>・BLA15-12U-A01 (2022/9\~2023/12) | ・[0x2F] 角度制御　ブースト機能実装 |
| 1.300 | 全機種 (2024/1\~) | ・動作改善 |

### Firmware version management table

| Ver | 機種(期間) | 変更内容 |
| :---: | :--- | :--- |
| 1.010 | ・BLA21-\*\*U-A0* (1/2021\~12/2023)<br>・BLA15-06U-A01 (5/2021\~12/2023) | ・New firmware |
| 1.100 | ・BLA21-\*\*U-AB2 (10/2021~4/2022) | ・Implementation Speed/Torque Control ON/OFF [0x25].<br> Speed/Torque Control is OFF by default.<br>・Implementation Overcurrent protection [0x2A].<br>・implementation PWM input setting [0x34] to [0x37].<br>(Only for models that support PWM input) |
| 1.200 | ・BLA21-\*\*U-AB2 (5/2022\~12/2023)<br>・BLA15-12U-A01 (9/2022\~12/2023) | ・Implementation Angle control Boost [0x2F]. |
| 1.300 | All models (1/2024\~) | ・Improved behavior |
