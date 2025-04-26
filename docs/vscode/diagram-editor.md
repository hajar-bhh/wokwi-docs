{
  "version": 1,
  "author": "",
  "editor": "wokwi",
  "parts": [
    {
      "type": "wokwi-dht22",
      "id": "p1",
      "cirkitDesignerTypeID": "76bd66c7-e24d-e1e2-c5b0-259aaba19349",
      "cirkitDesignerInstanceID": "f55713fc-9130-4a72-8589-d6ef8f779482",
      "top": 138.22190400000025,
      "left": 441.1893255000001,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "wokwi-arduino-uno",
      "id": "u2",
      "cirkitDesignerTypeID": "23db5403-7550-740c-a02b-8b3755757442",
      "cirkitDesignerInstanceID": "c925210e-16b8-4620-8159-455d52d47893",
      "top": 483.2218200000002,
      "left": 388.68932700000005,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "board-ds18b20",
      "id": "p3",
      "cirkitDesignerTypeID": "e2f44d25-4e0a-0597-8a3e-c96edfa06f32",
      "cirkitDesignerInstanceID": "9a598761-026d-47b8-b008-93a11d459531",
      "top": 247.72181700000021,
      "left": 18.18932700000005,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "wokwi-photoresistor-sensor",
      "id": "p4",
      "cirkitDesignerTypeID": "0f2918f0-bc39-436d-ab03-71a55044e559",
      "cirkitDesignerInstanceID": "2b20df3e-3cd7-45c0-9e93-5d44930a7193",
      "top": 475.6111380000001,
      "left": 147.34738800000002,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "board-ssd1306",
      "id": "p5",
      "cirkitDesignerTypeID": "02eba015-74c5-41e4-b72e-a44004e25461",
      "cirkitDesignerInstanceID": "f195cb5b-9975-44e9-b1f4-84bf0d177218",
      "top": 0,
      "left": 721.4708729999999,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "wokwi-servo",
      "id": "p6",
      "cirkitDesignerTypeID": "233f901c-5ffd-44a2-b253-527a22a136ca",
      "cirkitDesignerInstanceID": "b8a4d597-b710-407d-8d46-81efa7708446",
      "top": 860.7489435000002,
      "left": 0,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "wokwi-relay-module",
      "id": "p7",
      "cirkitDesignerTypeID": "d1472a6f-c54b-4f66-856e-dec6c99df000",
      "cirkitDesignerInstanceID": "1e1781d5-726f-4375-a39c-b59c05a8d3e7",
      "top": 1044.2320425000003,
      "left": 980.988813,
      "rotate": 0,
      "attrs": {}
    },
    {
      "type": "wokwi-rgb-led",
      "id": "p8",
      "cirkitDesignerTypeID": "8096b92c-a292-4fb8-bff9-01b8aa15e0a6",
      "cirkitDesignerInstanceID": "dfb9bf1c-e774-47d5-bc44-7468231f7a4a",
      "top": 1059.838206,
      "left": 1351.5849764999998,
      "rotate": 0,
      "attrs": {
        "common": "cathode"
      }
    },
    {
      "type": "wokwi-resistor",
      "id": "r9",
      "cirkitDesignerTypeID": "72c75556-baa3-04e7-55a5-e13f447c8c5a",
      "cirkitDesignerInstanceID": "08bedd14-730f-4869-8cf3-dac9178b0b9b",
      "top": 513.3251046774943,
      "left": 41.234990259466144,
      "rotate": 270,
      "attrs": {
        "value": "4700"
      }
    },
    {
      "type": "wokwi-resistor",
      "id": "r10",
      "cirkitDesignerTypeID": "72c75556-baa3-04e7-55a5-e13f447c8c5a",
      "cirkitDesignerInstanceID": "3b277fb5-1895-4939-bcc4-c7ef8f6e2e50",
      "top": 984.6659037118151,
      "left": 1203.4228767729114,
      "rotate": 0,
      "attrs": {
        "value": "220"
      }
    },
    {
      "type": "wokwi-resistor",
      "id": "r11",
      "cirkitDesignerTypeID": "72c75556-baa3-04e7-55a5-e13f447c8c5a",
      "cirkitDesignerInstanceID": "186bb9a8-39da-4a2c-b466-99bb5e6352b3",
      "top": 1021.3106367423632,
      "left": 1192.600510257637,
      "rotate": 0,
      "attrs": {
        "value": "220"
      }
    },
    {
      "type": "wokwi-resistor",
      "id": "r12",
      "cirkitDesignerTypeID": "72c75556-baa3-04e7-55a5-e13f447c8c5a",
      "cirkitDesignerInstanceID": "d7cd7abf-8c53-4949-a83d-786abcc6cb5d",
      "top": 1079.2218200000002,
      "left": 1194.689327,
      "rotate": 0,
      "attrs": {
        "value": "220"
      }
    }
  ],
  "connections": [
    [
      "r9:1",
      "p7:NO",
      "#ff006f",
      []
    ],
    [
      "p7:NO",
      "p7:VCC",
      "#ff006f",
      []
    ],
    [
      "p7:VCC",
      "p3:VCC",
      "#ff006f",
      []
    ],
    [
      "p3:VCC",
      "p6:V+",
      "#ff006f",
      []
    ],
    [
      "p6:V+",
      "u2:5V",
      "#ff006f",
      []
    ],
    [
      "u2:5V",
      "p5:VCC",
      "#ff006f",
      []
    ],
    [
      "p5:VCC",
      "p1:VCC",
      "#ff006f",
      []
    ],
    [
      "p1:VCC",
      "p4:VCC",
      "#ff006f",
      []
    ],
    [
      "u2:2",
      "p1:SDA",
      "#9E008E",
      []
    ],
    [
      "u2:GND.3",
      "p5:GND",
      "#000000",
      []
    ],
    [
      "p5:GND",
      "p1:GND",
      "#000000",
      []
    ],
    [
      "p1:GND",
      "p8:COM",
      "#000000",
      []
    ],
    [
      "p7:GND",
      "p3:GND",
      "#FFE502",
      []
    ],
    [
      "p3:GND",
      "p6:GND",
      "#FFE502",
      []
    ],
    [
      "p6:GND",
      "u2:GND.2",
      "#FFE502",
      []
    ],
    [
      "u2:GND.2",
      "p4:GND",
      "#FFE502",
      []
    ],
    [
      "p3:DQ",
      "u2:3",
      "#007DB5",
      []
    ],
    [
      "u2:3",
      "r9:2",
      "#007DB5",
      []
    ],
    [
      "p5:SCL",
      "u2:A5",
      "#6ddfbf",
      []
    ],
    [
      "u2:7",
      "p7:IN",
      "#ca56d2",
      []
    ],
    [
      "u2:8",
      "p4:D0",
      "#b80a75",
      []
    ],
    [
      "p4:A0",
      "u2:A0",
      "#683D3B",
      []
    ],
    [
      "p5:SDA",
      "u2:A4",
      "#169c3e",
      []
    ],
    [
      "u2:6",
      "p6:PWM",
      "#f5b8e8",
      []
    ],
    [
      "p8:R",
      "r10:2",
      "#e70d23",
      []
    ],
    [
      "r11:1",
      "p7:COM",
      "#A75740",
      []
    ],
    [
      "p7:COM",
      "r10:1",
      "#A75740",
      []
    ],
    [
      "r10:1",
      "r12:1",
      "#A75740",
      []
    ],
    [
      "r11:2",
      "p8:G",
      "#08aa5f",
      []
    ],
    [
      "r12:2",
      "p8:B",
      "#3520cf",
      []
    ]
  ],
  "dependencies": {}
}
