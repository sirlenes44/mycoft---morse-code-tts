# mycoft---morse-code-tts

speaks in morse code, it simply checks each letter to the corresponding morse code and plays the morse sound taken from wikimedia

# install

copy everything to mycroft-core folder

# config

add a section to TTS with morse code, change module to "morse"

      "tts": {
          "module": "morse",
          "morse":{
            "time_step": 0.5,
            "path": "/home/user/mycroft-core-base/mycroft/res/morse_sound_files/"
          }, 
          ......

in server set update to false or mycroft.home.ai will over-ride your change

      "server": {  
          "url": "https://api.mycroft.ai", 
           "version": "v1",  
           "update": false,  
           "metrics": false},
