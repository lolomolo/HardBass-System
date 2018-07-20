# HardBass-System
ESP8266 based meshnet which will monitor only one state; HARDBASS State. 

If the any of the many esp8266 bases sensors detect a HARDBASS-STATE ON all meshnet components will activate.
There are 4 discrete peripheral types. Each is based around the ESP8266_01 Module. 
1; Button|  this platform will only monitor the state of the hardbass button and inform the meshnet of the current state.
2; RasPi|   this platform will inform the raspberry pi when the bardbass state has been switched to on.
3; Relay|   this platform will switch a 10A 120VAC relay when it detects that the hardbass state has been switched on.
4; RGB|     this platform will drive an LED strip to a specific color cycle when it detects that the hardbass state has been switched on.

On detect; the RasPi will procede to raise volume to max and play Tri_Poloski.mp4 on its audio output.
On detect; all illuminating lights in the garage will be switched off by the Relay platform(s)
On detect; rgb strips controls will be highjacked by the RGB platform and go into rave mode
