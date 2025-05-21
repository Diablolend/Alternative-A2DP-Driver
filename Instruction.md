### How to Install Alternative A2DP Driver

**Instructions:**
_(WARNING: This information may not work or may work incorrectly! Welcome to the Issue.)_
_(NOTE: This manipulation may not work on Windows 11 24H2. Try using Windows test mode, where actions with DSE-Patcher are specified.)_

-Install the original program from the provided archive. (AlternativeA2dpSetup-1.6.0.1.msi)

-Close the program without changing anything. Copy the contents from the "crack" folder into the program directory, confirming file replacement. (C:\Program Files\Luculent Systems\AltA2DP)

-Run DSE-Patcher (if your version is earlier than 24H2) and disable DSE.

-Launch Alternative A2DP Driver and install the driver according to the original manual. Check via win+r > devmgmt.msc > Sound to ensure everything installed without errors.
- -If the fake signature fails, you will have to repeat this every time Windows boots. However, a .bat file is included to simplify the process. DSE-Patcher will still need to be run manually.

-That's it. If the driver loads correctly after a reboot, everything was successful. Enjoy using it. :)

_(P.S. If you accidentally installed the original driver, you can remove it like this: pnputil.exe -f -d C:\Windows\System32\DriverStore\FileRepository\alta2dp.inf_amd64_8adcf7b721e1e624\AltA2DP.inf)_
