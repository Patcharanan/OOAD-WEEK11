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
