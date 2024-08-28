# Let's now have the bot tell us Sunrise and Sunset Times. 
- We are going to build off of our last Enhancement.
- This will allow us to present Sunrise and Sunset Times to the user. 

### requirements.txt
- We'll need to add *suntime* to the requirements.txt file that way when we do our pip install we ensure all dependencies are accounted for. 

- 
### config.ini
- Let's scroll down to the utilities_menu_items and add N
- It should look something like this now:
  ```
  utilities_menu_items = S, F, W, X, T, N
   ```
- This will enable our new Menu Item
### command_handlers.py
- Let's start by adding at the very top of the document importing some libraries from suntime
  ```
  from suntime import Sun, SunTimeException
  ```
  


### message_processing.py




