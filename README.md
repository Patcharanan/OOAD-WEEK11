# OOAD-WEEK11
State Diagram
* รูปที่ 1 ส่ง SMS
```
@startuml
title  Send Message
[*] -r-> Mobile : Unlock Mobile
Mobile : SMS
Mobile -r-> SMS : Open Application
SMS : Text\nPicture\nEmotion
SMS -d-> Text : Enter text
Text : Thai\nEnglish
Text -l-> Picture : Insert Picture
Picture : PNG\nJPG\nGIF
Picture -l-> Recipient : Enter Call number
Recipient : Call number
Recipient -l-> [*] : Send
@enduml

```

![](http://www.plantuml.com/plantuml/img/RP312i9034Jl-nKv2_s17aIHAWhLOlLaFQmrQ72RbjqK_7pJMgi7Bu5vCqbWPa6ibxPoHaWS0kJ8LqWn17j3SvgS8VBH5DBwGkh6S6HNbuz1cn7dQVuHVLwrqbs33FEcSLHQePhD6n_mAGLdL4hhiU2agaSpkkfovsiiOK4Fei8Cv72tf7c-EGhtDuoSBWodDB7cW5u-m7oDRBigU9FfMAsN8--tzrXIGyZVdmlh771RNT2RN_S_xuzqJSLzUMQceolq1G00)

* รูปที่ 2 โอนเงิน
```
@startuml
title  Transfer Money
[*] -r-> Mobile : Unlock Mobile
Mobile : Application
Mobile -r-> MobileBanking : Open Application
MobileBanking : textbox :Username\ntextbox :Password
MobileBanking -d-> transferWindow : Enter Application
transferWindow : account number\naccount name\nBank account
transferWindow -l-> MoneyType : Enter Money
MoneyType : Baht\nDollas\nYen\n
MoneyType -l-> [*] : Press OK 
@enduml
```
![](http://www.plantuml.com/plantuml/img/RL51Ri8m4Bpd5Nkkb0_aK544fwg20wX2c8EJR5iBPnojDm9-ZvD2cj8UPtPcPpsUHRMYNUCpTUgPQ2CMyOE5tWBuaksV3fHB_fnWwTAye2ryg8utd8tqIzjwLrbr0NToufjR71q-asxLCluH_mYKprg6CnNRo0BRiC58hMsCfo3rWoclKv3U3dztgCCfBLecd_oA-YEnLHKwAA5hIXQ34G-n_VgxvD6R--5jgQBDfUKnxRkqAJ-tNsgm2DxRQB1Z64pcmvg-uuBMmZ7IwfMo6QFkV-GA)
