
# Let's now have the bot give us some ADSB Data. 
- So far we've been working with local/static data. We'll be introducing a live data source, while the data will be live it is still offline. We'll be using
  - Hardware
    - RTL-SDR USB Dongle
    - Antenna ( The one that comes with is is fine for a proof of concept)
  - Software
    - Dump 1090
      - https://github.com/gvanem/Dump1090
      - This software uses the RTL-SDR Dongle and Dumps ADSB Data :)     
    - ADSB Stats Logger
      - https://github.com/nfacha/adsb-stats-logger/
      - This software uses the output from Dump1090 Logs it and has some statistics around the data.
     
  - Initially, we'll build the data to play with it within our bot.  Initially, it will be a request/response type of scenario. If ( big If) I feel confident I may incorporate an if-then-else function here, where if an aircraft is within a certain mileage it will alert the meshtastic channel. I am not confident in my abilities so far yet, that's why I preface it with an If. 
## Section 1 ( ADSB Data)
- 1 Install RTL-SDR Dongle and IT's drivers, while we won't be using SDRSharp it would be wise to get that up and running. (It will ensure you have your SDR dongle working)
  - 1.1 Plug Everything in 
- 2 Download and extract Dump1090
  - 2.1 Edit the batch file
    ```
    dump1090.exe --interactive --net
    ```
  - 2.2 Double click the bat file and  you should now get some output on the Command Prompt Looking window
- 3 Take a look at the website http
- 4 Let's setup adsb-stats logger
  - 4.1 Download and extract
  - 4.2 Create and Activate Python Virtual Environet
      ```
      python -m venv venv
      venv\Scripts\activate 
      ```
  - 4.3 Modify logger.py
  - Move logger.py and search.py into the Meshtastic folder we have been using. 



## Section 2 (Meshtsastic Bot)



### requirements/.txt

### config.ini

  
### command_handlers.py

### message_processing.py

# That's it

