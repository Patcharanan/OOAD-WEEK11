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
Picture -l-> [*] : Send
@enduml
```

![](http://www.plantuml.com/plantuml/img/HP3D2eCm48JlUOgS2ta13wKzMB5WAsXFjOTK5msD6qbMwEDt_UrbORwPMTWz1TAUnjuACcH1oWAmaHc4e5iGpyDBAg-ECdDlmsua7sXT_Lcrs76H5PkOywoPtWT0UHu6QsfDng5OS0bVgZ0tDOqUAenxjvkguVBaSon60Y-9XLX9sMd3UMoj2Tq2bUN2keeJAGRmj07nD_9RKk4rvv6abvtFxUd8QBvRd7XCl_W1)
