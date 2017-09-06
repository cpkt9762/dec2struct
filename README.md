# dec2struct
Python plugin to easily setup vtables in IDA using declaration files


Using the class declaration/definition it automatically generates the vtables.

# How to use
Press Alt+F7 and run the script
Choose the file that contains the definition/declaration of the class
Now you can modify the type of the variable to the class
# Example

While reversing the game I noticed g_pSteamClientGameServer is an instance of [ISteamClient](https://github.com/ValveSoftware/source-sdk-2013/blob/master/mp/src/public/steam/isteamclient.h)

So instead of creating the whole vtable by hand this plugin allows you to generate it.

I ran the plugin then changed the type of g_pSteamClientGameServer to ISteamClient(generated by the plugin).

## Before
![Before](https://raw.githubusercontent.com/krystalgamer/dec2struct/master/before.png)

## After
![After](https://raw.githubusercontent.com/krystalgamer/dec2struct/master/after.png)
