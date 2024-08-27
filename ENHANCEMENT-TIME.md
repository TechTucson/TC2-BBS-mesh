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
 - Now let's add an entry to the def(build_menu) function that will conincide with our *T*. Place it in between anything you'd like for now. 
   ```
           elif item.strip() == 'T':
            menu_str += "[T]ime\n"
   ```
     - This allows the Menu item *T* to be added to the Menus. 
  - Now we'll need to create our own function to do what we want it to do.
    ```
    def handle_time_command(sender_id, interface, menu_name=None):
    now = datetime.datetime.now()
    send_message(now.strftime("%Y-%m-%d %H:%M:%S"), sender_id, interface)
    ```
    - This function defines the  *now* variable and assigns it a value using the DateTime library (I think that's what it is) that we imported. Followed by sending the message back to the user. There's some formatting but that's not important for now. 

### message_processing.py


