# Bluesh Modified
 A modified Rainmeter skin originally created by [ApexXx-SenSei](https://www.deviantart.com/apexxx-sensei).
 
## Preview
![Preview IMG](./Screenshots/preview.png)\
Artwork by [HJ_penguin](https://www.pixiv.net/en/artworks/115226775)

## Used Plugins
1. [RainRGB](https://forum.rainmeter.net/viewtopic.php?f=18&t=6215) by [jsmorley](https://www.deviantart.com/jsmorley)
2. [FrostedGlass](https://github.com/khanhas/FrostedGlass) by [TheAzack9](github.com/TheAzack9) & [khanhas](https://github.com/khanhas)
3. [NirCmd](https://www.nirsoft.net/utils/nircmd.html) by [Nir Sofer](nirsoft.net)

## FAQ
1. How to change the widget size?
    * Adjust it with scroll wheel.
2. What does the translate button do?
    * You can change the display name of weekday and month by the translate function.
    * For example,\
    ![](./Screenshots/translate_edit.png)
    * Save the file and refresh all skin.\
    ![](./Screenshots/refresh.png)
    * Done.\
    ![](./Screenshots/translate_done.png)
3. Why the power buttons aren't showing?
    * If you are using Windows 10, you will see this:\
    ![](./Screenshots/win10.png)
    * Just find `Segoe Fluent Icons` and replace it with `Segoe MDL2 Assets` in the `Bluesh\Links\Links.ini` file.
    * Done.\
    ![](./Screenshots/win10_done.png)
4. Can I make the sleep button turn off my screen instead of sleeping my computer?
    * Sure, just change the `[Sleep1]` section in the `Bluesh\Links\Links.ini` file or add a new button with following code. (May not work on most laptops.)
    ```
    [ScreenOff1]
    Meter=String
    MeterStyle=StylePowerStyle1
    X=(32*#Scale#)r
    Y=0r
    Text="[\xEA14]"
    LeftMouseUpAction=[#@#Addons\nircmd.exe monitor off]
    ```
5. Why my shortcuts aren't working?
    * In order to make those shortcuts work, you need to change the paths in the `Bluesh\Links\Links.ini` file.
    * For example, click the edit button first.\
    ![](./Screenshots/edit.png)
    * Change the shortcut name and path to whatever you want.\
    ![](./Screenshots/link_1.png)
    * You can also add a new shortcut by adding these lines.\
    ![](./Screenshots/link_2.png)
    ![](./Screenshots/link_3.png)
    * Don't forgot to save and refresh.
    * Done.\
    ![](./Screenshots/link_done.png)    
6. How to read the second dots?
    * The second dots are displayed in binary-coded sexagesimal, the leftmost bit is the most significant one.
    * For example, the time in the following imange is 17:49:51.\
    ![](./Screenshots/binary_clock.png)
    * It's originally created by [FlyingHyrax](https://www.deviantart.com/flyinghyrax).

## Known Issues
The Rainmeter AudioLevel plugin prevents the computer from auto sleeping. Sadly, there is nothing I can do.

**Workaround:**
1. **Open Group Policy Editor:**
    - Press `Windows + R`, type `gpedit.msc`, and press Enter.
   
2. **Navigate to the Sleep Settings:**
    - Go to `Computer Configuration` > `Administrative Templates` > `System` > `Power Management` > `Sleep Settings`.
   
3. **Configure the setting:**
    - Find and double-click on **"Allow applications to prevent automatic sleep (plugged in)"**.
    - Set it to **Disabled**.
   
4. **Apply and restart your computer.**