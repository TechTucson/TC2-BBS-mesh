
# Let's now have the bot give us definitions of words. 
- We are going to build off of our last Enhancement.
- Our but will ask for the Word you would like defined and then provide the definition. 


### requirements/.txt
- We'll use this JSON English Language Dictionary located here: https://github.com/matthewreagan/WebstersEnglishDictionary/blob/master/dictionary.json I've also placed a copy in /Tools/dictionary.json
  
### config.ini
- Let's scroll down to the utilities_menu_items and add D
- It should look something like this now:
  ```
  utilities_menu_items = S, F, W, X, T, N, D
   ```
- This will enable our new Menu Item

  
### command_handlers.py

    ```


### message_processing.py


# That's it

