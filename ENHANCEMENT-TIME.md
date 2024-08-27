# Let's have the BOT give us it's current time

### config.ini
- Let's scroll down to the utilities_menu_items and add T
- It should look something like this now:
  ```
  utilities_menu_items = S, F, W, X, T
   ```
- This will enable our new Menu Item
### command_handlers.py
- Let's start by adding at the very top of the document 
   ```
   import datetime
   ```
 - Now let's add an entry to the def(build_menu) function that will conincide with our *T*.
   ```
           elif item.strip() == 'T':
            menu_str += "[T]est\n"
   ```

### message_handlers.py

