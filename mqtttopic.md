## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301023/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
2. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301023/model-01/sn-001
    - payload
        - {"temperature": "29.2"}
        - {"Pressure Sensors": "55"}
        - {"Load Sensors": "5"}
        - {"weight_cloth": "4"}
        - {"rotation": "20"}
        - {"้huminity": "50"}
        - {"Water Level Sensors": "3"}
        - {""inbalance": "8.5""}
        - {"Heat Pump": "40"}
        

 3. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/6310301023/model-01/sn-001
    - payload
        - {"current": "155"}
        - {"Hall Effect Sensors": "14"}
        - {"vibration": "0.9"}
        - {"radar": "5"}
        - {"Vibration Sensors": "0.2"}
        - {"air_pressure": "110"}
        - {"touch_open/close": "0"}

