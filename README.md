#นายพชรนันท์ จันทร์รักษ์ 57030198
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

* รูปที่ 3 สั่งสินค้าออนไลน์
```
@startuml
title  Online Shopping
[*] -r-> Website : Open Website
Website : URL
Website -r-> Home : EnterSite
Home :  Product\nPrice\nPicture
Home -r-> Profile : Login
Profile : Username\nPicture\nAddress
Profile -d-> Cart : Add Product to Cart
Cart : Product\namount\nBill
Cart -l-> Payment : Pay
Payment : Cash\nCard
Payment -l-> WaitForProduct : Wait
WaitForProduct : Waiting for delivery
WaitForProduct -l-> [*] : receive
@enduml
```

![](http://www.plantuml.com/plantuml/img/RP5DQyCm38Rl_XKw3_87SXZToiOEXPQLqaEpWnUhhS2HWwmCykzhU_c0iPFG-pxwiBo9QaM7pXibzGYmPq-CSBo7lYU-cSlJ5rHIFSCPloCfGWtx7dbEpIgVFdTBLYe-GfVrDrQKOsOd0GuItD1gmmUX5bEWLWUP_5AQY2lv3E_2ZTYi-IcYiEtMgePVd1ECSO4gbpfiqxCIdhnv76WegfciPGlRXO5JV2NlVytAvntis24NqevcpROstXjEd5l4mfyjwNkGULfT1FElcWuBro3WqDCFolYNAltovMiGR34nPeFiyZSz0000)

* รูปที่ 4 เติมเงิน
```
@startuml
title  Top-Up
[*] -r-> MachineTopUp : Go to Machine TopUp
MachineTopUp : Menu
MachineTopUp -r-> PressMenu : Enter Menu
PressMenu : Select callnumber\namount
PressMenu -d-> Money : Insert Money
Money : Coin\nBill
Money -l-> Confirm : Press OK
Confirm : Check Money\nCheck call number
Confirm -l-> [*] : End
@enduml
```

![](http://www.plantuml.com/plantuml/img/NP3D2i9038Jl-nGv2_i27gHOH4IAWlPaFQnjf8lRRDcc1z_U_R5QFURBP9XCDh1oF7P6i6Q306VRox8NbyKLf9ChA5JTQaAFonwMiBN0Te8GgVYJ54ZZBuj6HuV347PUiY56buHpV4A3DKEjZA6nkw6hI7Ls99wfP1D2MSAdFzZHW8xJA2QOMqqLhRKnRoIDFyajtRNh_3vwmM4llYXliNuacuhI4490Il4HHgFGJFYW4HbI4vfx0G00)

* รูปที่ 5 Login Facebook
```
@startuml
title  Login Facebook
[*] -r-> Website : Open Website
Website : URL\nNew tab
Website -r-> Facebook : Enter Facebook
Facebook : Username\nPassword\nE-mail\nCall number
Facebook -d-> Identify : Enter security code
Identify : security code 6 Digit
Identify-l-> HomeFeed : If SuccessFul
HomeFeed : News\nActivity
HomeFeed -l-> [*] : Successful
@enduml
```

![](http://www.plantuml.com/plantuml/img/LP3DIaCn44RtUOfP2zcww48gsek5OejIN1WNkSdS4amcafbO-lQcXVlZSkPytu6PDOijKbDK4YGYm2wV0a5d7VOvVwlFko_GHJ_01_OS1645-n-aSLJp-lYsC_IAPn3RJ-jRTPIrq8O4osnVa2DZ8PlGqC4odtFnXZOwsH0DFTaOWMhgiSmLxPjwwv4a39T9pUXg2N81bpsg1Vu7u1wUmod85D2noLvomWxHj_HsWFVg739tDQe5Q0UoeKSduRV9Pd8JN9-r6ej3AwwH_FMtVm00)


## Activity Diagram

* รูปที่ 1 สัญญาณไฟจราจร
```
@startuml
title Traffic Light
(*) --> "Queue"

if "If Traffic Light has Change" then
  -->[Green] "Pass"
    -r-> [End](*)
else
  ->[Red] "Stop"
  -->[End] (*)
endif
@enduml
```

![](http://www.plantuml.com/plantuml/img/LSvD2W8n30NWVKuHib9XhZ0CY8ZWmhzTcKMnwRHGEzAczpSLDwu2Z-yzCbMnHTehWKH9Z8zYlOzFFCSb26nsMno64UdQk341H8zqylyAWwsu3pOlJ2Y1Cs0lcMDXpZFInTPAccbQTCiSifjr63XLxdGqDtRgxhA-wTVj1hyek-W19htwv0S0)

* รูปที่ 2 เปลี่ยนอุณหภูมิ
```
@startuml
title Air temperature
(*) --> "Remote"
if "Press Remote\n for change temperature" then
  -->[increase] "Rooms heat up"
    -r-> [End](*)
else
  ->[decrease] "Temperature down"
  -->[End] (*)
endif
@enduml
```

![](http://www.plantuml.com/plantuml/img/JOyn3i8m34LtdyBA14YzGbK6TeJOIeUe-QMHcgHo775zKa30PCd-xtsvosf5IrX8lIxWenTMX1LYjGXeTzXpqxHiBWX9OOZynEOio9dVgrlaAGcFiurt_BE6TKOatlZUnr5WCuPgIYbadc6LoshglIQaLlIdw8RQHrWoDgpj7RxKzITcbnxHVCGRn2ygEZyHTNNMTvu0)

* รูปที่ 3 ปลดล็อค iPhone
```
@startuml
title Unlock iPhone
(*) --> "iPhone and Finger"

if "Put your finger on the scanner" then
  -->[straight] "Unlock iPhone"
    -r-> [End](*)
else
  -r->[not straight] "Try Again"
  -->[End] (*)
endif
@enduml
```

![](http://www.plantuml.com/plantuml/img/LK-x3i8m3Dpz5QTCWCGle3B0t06cgaFKfgr5SAJ47Vhtk2q3JDQTxw6hYlgiypkIiiQ0fyJKlS3rb2JGuNJ4-No1sp6yzBYpZ24x8XxWwbcnf3bZs5WaWKu1fVCY9bg14DQCfcZsF4xQmlsLEFkR8bjDSvE-jKuAiGJQoKQIuiVxo0kkesTntzpLWyqaFGz4bLtRym40)

* รูปที่ 4 บุรุษไปรษณีย์ ส่งของ
```
@startuml
title Delivery 
(*) --> "Postman"
Postman -d-> delivery 

if "  postman come delivery\nand recipient...." then
  -d->[stay at home] "Send success"
  -d->[End] (*)  
    
else
  -r->[Not at home] "Resend"
  Resend -u-> delivery
endif
@enduml
```

![](http://www.plantuml.com/plantuml/img/JK_D2i8m3BxtAJvwKg4-WkoWLn4zwWwbpLYXwqQR2NjxCvrZEIJX-ybFLTXc7hkeE70ad2c6D-K9QdVOmvWJzAqltDcarTB0U87zAbIXWGQ6XNLzHolxIZPvP79X29JuAA71BIM5xvYdh9zW6QsuQkW7YRoCpb4f-g-v95zZFWU2IA9OQEQoSDUUD_Ox5Ham6tyTpBWvLGaI6bL9aOS_)

* รูปที่ 5 เลือกซื้อสินค้าใน shop
```
@startuml
title Buy Product 
(*) --> "Customer"
Customer -d-> Shop 

if "  Select Product" then
  -d->[Pleased] "Buy"
  -d-> Pay
  -d->[End] (*)  
    
else
  -r->[displeased] "Choose Again"
  "Choose Again" -u-> Shop 
endif
@enduml
```

![](http://www.plantuml.com/plantuml/img/LKyx2iCm3DrrYeUdjk0hbBIXUo1ZwM1gfJ4uTl1doEshb2JGHHBleoSrkPXKwkIfkE8PzxgWIz7MTm6TBcTeVOLgQovnugHedw2j4FqOPn2v0GhesREuDhT26JaGVi9dvzbajYye2L0RYiuik-0HX5pp88WKzfbNBWbdNPuFVpl6c1ctZt5XNVGFGDVZB0xM3TH8a_U-)
#นายพชรนันท์ จันทร์รักษ์ 57030198
