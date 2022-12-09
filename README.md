# Bluesh Modified
 A modified Rainmeter skin originally created by [ApexXx-SenSei](https://www.deviantart.com/apexxx-sensei).
 
## Preview
![](https://i.imgur.com/fVOGLsI.jpg)

## FAQ
1. How to change the widget size?
    * Adjust it with scroll wheel.
2. What does the translate button do?
    * You can change the display name of weekday and month by the translate function.
    * For example,
    ![](https://i.imgur.com/q5YaKXa.png)
    * Save the file and refresh all skin.
    ![](https://i.imgur.com/ry3h9l8.png)
    * Done.
    ![](https://i.imgur.com/SSNnRsf.png)
3. Can I make the sleep button turn off my screen instead of sleeping my computer?
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
4. Why my shortcuts aren't working?
    * In order to make those shortcuts work, you need to change the paths in the `Bluesh\Links\Links.ini` file.
    * For example, click the edit button first.
    ![](https://i.imgur.com/qEvH5VZ.png)
    * Change the shortcut name and path to whatever you want.
    ![](https://i.imgur.com/RHlkJSE.png)
    * You can also add a new shortcut by adding these lines.
    ![](https://i.imgur.com/VrLQBnP.png)
    ![](https://i.imgur.com/t5vJ1aw.png)
    * Don't forgot to save and refresh.
    * Done.
    ![](https://i.imgur.com/cF7yE9g.png)
5. How to read the second dots?
    * The second dots are displayed in binary-coded sexagesimal, the leftmost bit is the most significant one.
    * For example, the time in the following imange is 20:35:21.
    ![](https://i.imgur.com/CCKa5DF.png)
    * It's originally created by [FlyingHyrax](https://www.deviantart.com/flyinghyrax), you can find the full version (with hours and minutes) [here](deviantart.com/flyinghyrax/art/Binary-Clock-266686125).

### Used Plugins
1. [RainRGB](https://forum.rainmeter.net/viewtopic.php?f=18&t=6215) by [jsmorley](https://www.deviantart.com/jsmorley)
2. [FrostedGlass](https://github.com/khanhas/FrostedGlass) by [TheAzack9](github.com/TheAzack9) & [khanhas](https://github.com/khanhas)
3. [NirCmd](https://www.nirsoft.net/utils/nircmd.html) by [Nir Sofer](nirsoft.net)
