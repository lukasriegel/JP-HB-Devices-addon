# JP-HB-Devices-addon [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/) [![Github All Releases](https://img.shields.io/github/downloads/jp112sdl/JP-HB-Devices-addon/total.svg)](https://github.com/jp112sdl/JP-HB-Devices-addon/releases) [![GitHub issues](https://img.shields.io/github/issues/jp112sdl/JP-HB-Devices-addon.svg)](https://github.com/jp112sdl/JP-HB-Devices-addon/issues)

**:heavy_check_mark: lauffähig unter CCU / RaspberryMatic Firmware 2.31.x - 2.51.6 | 3.37.x - 3.51.6**<br/>

Die jeweils aktuellste Version ist bei den [Releases](https://github.com/jp112sdl/JP-HB-Devices-addon/releases/latest) zu finden.

**Das Wichtigste vorweg:**<br/>
Dieses Addon integriert die unten aufgelisteten HomeBrew Projekte in die CCU-Firmware.</font><br/>
Ich stelle es 
* kostenfrei 
* ohne jeglichen Anspruch auf vollständige Funktion 
* auf eigene Gefahr (z.B. unerwünschte Nebeneffekte in der CCU-Firmware)

zur Verfügung.<br/>
Da es sich um ein reines Hobby-Projekt handelt, kann ich **weder (umfangreichen) Support** leisten, **noch auf individuelle Wünsche eingehen** oder **zeitnah die neueste CCU-Firmware unterstützen**!<br/>
Es sollte klar sein, dass mit (m)einer eventuellen Aufgabe dieses Hobbys, mittel-/langfristig (teilweise) keine Verwendung u.g. Geräte mehr möglich ist. <i>Wie bei Open Source Projekten üblich, kann sich jedoch jeder an der Entwicklung beteiligen!</i>

Nach der Installation wird ein Neustart der Zentrale durchgeführt.<br/>
Die eigentliche Installation des Addons erfolgt nach diesem Neustart.<br/>
Währenddessen werden ReGa und der RFD gestoppt, so dass es _(nicht bei RaspberryMatic!)_ im Browser zu der Meldung<br/>`Eine Komponente der Homematic Zentrale reagiert nicht mehr.` kommen kann.<br/>
_Bitte etwas Geduld haben - je nach Geschwindigkeit der SD Karte kann die Installation u.U. mehrere Minuten in Anspruch nehmen!_<br/><br/>

📍 Sollten anschließend keine Geräte-Icons und/oder -beschreibungen angezeigt werden, muss der Browser-Cache gelöscht werden.

#### Dieses Addon wird benötigt, um die Kompatibilität der folgenden HomeMatic Selbstbaugeräte herzustellen:

|  | Name | Beschreibung | 🔋Batterie-/<br/>⚡️Netzbetrieb |
|--------|--------|--------|:--------:|
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-cap-moist_thumb.png" width=25/> | [HB-UNI-Sen-CAP-MOIST](https://github.com/jp112sdl/HB-UNI-Sen-CAP-MOIST) | kapazitiver Bodenfeuchtesensor<br/>_optional mit DS18B20 Temperatursensor_ | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-dist-tof_thumb.png" width=25/> | [HB-UNI-Sen-DIST-TOF](https://github.com/jp112sdl/HB-UNI-Sen-DIST-TOF) | Time-of-Flight Abstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-dist-us_thumb.png" width=25/> | [HB-UNI-Sen-DIST-US](https://github.com/jp112sdl/HB-UNI-Sen-DIST-US) | Ultraschall Abstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-lev-tof_thumb.png" width=25/> | [HB-UNI-Sen-LEV-TOF](https://github.com/jp112sdl/HB-UNI-Sen-LEV-TOF) | Time-of-Flight Füllstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-lev-us_thumb.png" width=25/> | [HB-UNI-Sen-LEV-US](https://github.com/jp112sdl/HB-UNI-Sen-LEV-US) | Ultraschall Füllstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-press_thumb.png" width=25/> | [HB-UNI-Sen-PRESS](https://github.com/jp112sdl/HB-UNI-Sen-PRESS) | Drucksensor | ⚡️ |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-temp-ds18b20_thumb.png" width=25/> | [HB-UNI-Sen-TEMP-DS18B20](https://github.com/jp112sdl/HB-UNI-Sen-TEMP-DS18B20) | 1..8fach DS18B20 Temperatursensor | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-wea_thumb.png" width=25/> | [HB-UNI-Sen-WEA](https://github.com/jp112sdl/HB-UNI-Sen-WEA) | Wetterstation | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-senact-4-4_thumb.png" width=25/> | [HB-UNI-SenAct-4-4](https://github.com/jp112sdl/HB-UNI-SenAct-4-4) | 4fach - Sender & - Aktor | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-senact-8-8_thumb.png" width=25/> |  [HB-UNI-SenAct-8-8](https://github.com/jp112sdl/HB-UNI-SenAct-8-8)  | 8fach - Sender & - Aktor | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-rgb-led-ctrl_thumb.png" width=25/> | [HB-UNI-RGB-LED-CTRL](https://github.com/jp112sdl/HB-UNI-RGB-LED-CTRL) | RGB Controller für WS28xx / Neopixel / etc. | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-temp-ir_thumb.png" width=25/> | [HB-UNI-Sen-TEMP-IR](https://github.com/jp112sdl/HB-UNI-Sen-TEMP-IR) | MLX90614 Infrarot Temperatursensor | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-dummy-beacon_thumb.png" width=25/> | [HB-UNI-Sen-DUMMY-BEACON](https://github.com/jp112sdl/HB-UNI-Sen-DUMMY-BEACON) | Dummy-Device zum Simulieren<br/>zyklischer Statusmeldungen sowie Ack-Nachrichten | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-volt_thumb.png" width=25/> | [HB-UNI-Sen-VOLT](https://github.com/jp112sdl/HB-UNI-Sen-VOLT) | universeller Spannungssensor (Template) | 🔋 |  
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/PushButton-2ch-wm_thumb.png" width=25/> | [HB-LC-Sw1PBU-FM](https://github.com/jp112sdl/Beispiel_AskSinPP/tree/master/examples/HB-LC-Sw1PBU-FM) | alternative Firmware für den<br/>HM-LC-Sw1PBU-FM (getrennte Taster-/Relais-Kanäle) | ⚡️ | 
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/PushButton-2ch-wm_thumb.png" width=25/> | [HB-LC-Sw2PBU-FM](https://github.com/jp112sdl/Beispiel_AskSinPP/tree/master/examples/HB-LC-Sw2PBU-FM) | alternative Firmware für den<br/>HM-LC-Sw2PBU-FM (getrennte Taster-/Relais-Kanäle) | ⚡️ | 
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/PushButton-2ch-wm_thumb.png" width=25/> | [HB-LC-Bl1PBU-FM](https://github.com/jp112sdl/Beispiel_AskSinPP/tree/master/examples/HB-LC-Bl1PBU-FM) | alternative Firmware für den<br/>HM-LC-Bl1PBU-FM (getrennte Taster-/Relais-Kanäle) | ⚡️ | 
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/5_hm-lc-sw2-fm_thumb.png" width=25/> | [HB-LC-Sw2-FM](https://github.com/stan23/HB-LC-Sw2-FM) | alternative Firmware für den<br/>HB-LC-Sw2-FM (getrennte Taster-/Relais-Kanäle) special thx to [stan23](https://github.com/stan23)! | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-dmx-master_thumb.png" width=25/> | [HB-UNI-DMX-Master](https://github.com/jp112sdl/HB-UNI-DMX-Master) | (sehr) einfacher DMX Master Controller | ⚡️ |  
|<img src="src/addon/www/config/img/devices/50/hb-dis-ep-42bw_thumb.png" width=25/> | [HB-Dis-EP-42BW](https://github.com/jp112sdl/HB-Dis-EP-42BW) | 4.2" ePaper Display | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-dis-ep-75bw_thumb.png" width=25/> | [HB-Dis-EP-75BW](https://github.com/jp112sdl/HB-Dis-EP-75BW) | 7.5" ePaper Display | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-rfid-rc_thumb.png" width=25/> | [HB-UNI-Sen-RFID-RC](https://github.com/jp112sdl/HB-UNI-Sen-RFID-RC) | RFID-Reader als Sender (Tasterschnittstelle) | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-ibut-8_thumb.png" width=25/> | [HB-IBUT-8](https://github.com/pa-pa/AskSinPP/tree/master/examples/custom/HB-IBUT-8) | iButton Sender Taster/Schließer | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-ou-mp3-led_thumb.png" width=25/> | [HB-OU-MP3-LED](https://github.com/jp112sdl/HB-OU-MP3-LED) | MP3-Player mit LED | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-weight_thumb.png" width=25/> | [HB-UNI-Sen-WEIGHT](https://github.com/jp112sdl/HB-UNI-Sen-WEIGHT) | universeller Wägesensor | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-weight-sc_thumb.png" width=25/> | [HB-UNI-Sen-WEIGHT-SC](https://github.com/jp112sdl/HB-UNI-Sen-WEIGHT-SC) | universeller Wägesensor mit Schließerkontakt | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-iaq_thumb.png" width=25/> | [HB-UNI-Sen-IAQ](https://github.com/jp112sdl/HB-UNI-Sen-IAQ) | universeller Luftgütesensor _(temporarily discontinued)_ [(see HM-Forum)](https://homematic-forum.de/forum/viewtopic.php?f=76&t=49422)| 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-rc-12-ep-bw_thumb.png" width=25/> | [HB-RC-12-EP](https://github.com/jp112sdl/HB-RC-12-EP) | 12 Kanal Fernbedienung mit Farb- oder Schwarz/Weiß-ePaper-Display | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-rc-2-pbu-led_thumb.png" width=25/> | [HB-RC-2-PBU-LED](https://github.com/jp112sdl/HB-RC-2-PBU-LED) | 2 Kanal Taster mit RGB-Hintergrundbeleuchtung | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-ou-mot-servo_thumb.png" width=25/> | [HB-OU-MOT-SERVO](https://github.com/jp112sdl/HB-OU-MOT-SERVO) | Servo-Motor Steuerung | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-pf-sc_thumb.png" width=25/> | [HB-UNI-Sen-PF-SC](https://github.com/jp112sdl/HB-UNI-Sen-PF-SC) | Tierklappenüberwachung | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-ou-rgb-tealight_thumb.png" width=25/> | [HB-OU-RGB-TEALIGHT](https://github.com/pafra-123/HB_RGB_LED_Candle) | RGB-LED-Kerze / Teelicht | ⚡️ / 🔋 | 
|<img src="https://raw.githubusercontent.com/eq-3/occu/master/WebUI/www/config/img/devices/50/114_hm-lc-dim1t-fm-lf_thumb.png" width=25/> | [HB-LC-Dim5PWM-CV](https://github.com/pa-pa/AskSinPP/tree/master/examples/stm32/HB-LC-Dim5PWM-CV) | 5-Kanal PWM Dimmer (STM32) | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-temp-max6675_thumb.png" width=25/> | [HB-UNI-Sen-TEMP-MAX6675](https://github.com/jp112sdl/HB-UNI-Sen-TEMP-MAX6675) | MAX6675 Temperatursensor bis 1000°C | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-temp-max6675-dt_thumb.png" width=25/> | [HB-UNI-Sen-TEMP-MAX6675-DT](https://github.com/jp112sdl/HB-UNI-Sen-TEMP-MAX6675) | MAX6675 Temperatur-Differenzsensor bis 1000°C | 🔋 | 

**Hinweis für Entwickler** _(verwendete Device Model meiner HB-Geräte)_ **:**

| Device Model | Gerät |
|--------|--------|
|E9 01 | HB-UNI-Sen-PRESS |
|E9 02 | HB-UNI-Sen-PRESS-SC |
|F1 D0 | HB-UNI-Sen-WEA |
|F1 D1 | HB-UNI-Sen-IAQ |
|F2 06 | HB-IBUT-8 |
|F3 01 | HB-UNI-Sen-TEMP-DS18B20 |
|F3 08 | HB-UNI-Sen-TEMP-IR |
|F3 09 | HB-UNI-Sen-TEMP-MAX6675 |
|F3 10 | HB-UNI-Sen-TEMP-MAX6675-DT |
|F3 11 | HB-UNI-Sen-CAP-MOIST |
|F3 12 | HB-UNI-Sen-CAP-MOIST-T |
|F3 20 | HB-LC-SW12-FM |
|F3 21 | HB-LC-Bl1-FM-BAT|
|F3 30 | HB-RC-2-PBU-LED|
|F3 31 | HB-UNI-SenAct-4-4-SC|
|F3 32 | HB-UNI-SenAct-4-4-RC|
|F3 33 | HB-UNI-SenAct-4-4-SC-BAT|
|F3 34 | HB-UNI-SenAct-4-4-RC-BAT|
|F3 35 | HB-LC-Sw1PBU-FM|
|F3 36 | HB-LC-Sw2PBU-FM|
|F3 37 | HB-LC-Bl1PBU-FM|
|F3 38 | HB-UNI-SenAct-8-8-RC|
|F3 39 | HB-UNI-SenAct-8-8-RC-BAT|
|F3 3A | HB-UNI-SenAct-8-8-SC|
|F3 3B | HB-UNI-SenAct-8-8-SC-BAT|
|F3 3C | HB-UNI-Sen-RFID-RC|
|F3 41 | HB-UNI-RGB-LED-CTRL |
|F3 42 | HB-UNI-DMX-MASTER |
|F3 43 | HB-DIS-EP-42BW |
|F3 44 | HB-OU-MP3-LED |
|F3 45 | HB-RC-12-EP-29C |
|F3 46 | HB-RC-12-EP-29BW |
|F3 47 | HB-DIS-EP-75BW |
|F3 48 | HB-OU-MOT-SERVO |
|F3 4A | HB-UNI-Sen-VOLT |
|F3 4B | HB-UNI-Sen-WEIGHT |
|F3 4C | HB-UNI-Sen-WEIGHT-SC |
|F3 4D | HB-UNI-Sen-PF-SC |
|F3 50 | HB-OU-RGB-TEALIGHT-BAT |
|F3 51 | HB-OU-RGB-TEALIGHT |
|F3 53 | HB-DIS-EP-42BW-MAINS |
|F3 57 | HB-DIS-EP-75BW-MAINS |
|F3 FF | HB-UNI-Sen-DUMMY-BEACON |
|_F5 01_ | _HB-LC-Sw2-FM_ |
|_F5 11_ | _HB-LC-Dim5PWM-CV_ |
|F9 D6 | HB-UNI-Sen-DIST-US |
|F9 D7 | HB-UNI-Sen-DIST-TOF |
|F9 D2 | HB-UNI-Sen-LEV-US |
|F9 D3 | HB-UNI-Sen-LEV-TOF |


<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Namensnennung - Nicht-kommerziell - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.

Die verwendeten Icons sind "free for non-commercial use" von
 - https://www.flaticon.com/authors/popcic from www.flaticon.com 
 - http://icons8.com 
