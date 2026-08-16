# How to Install Alternative A2DP Driver

> **WARNING**: These instructions may not work or may work incorrectly! You're welcome to make an issue.

> **NOTE**: This manipulation may not work on Windows 11 24H2 and above. Try doing it through the ALT version with Windows test mode (`bcdedit.exe -set TESTSIGNING ON` in `cmd.exe` with administrator privileges, then you can turn it off with `bcdedit.exe -set TESTSIGNING OFF` after the install), where the actions with DSE-Patcher are specified.

1. Install the original program from the provided archive. (`AlternativeA2dpSetup-1.6.0.1.msi`)
2. Close the program without changing anything. Copy the contents from the `crack` folder into the program directory, confirming file replacement. (`C:\Program Files\Luculent Systems\AltA2DP`)
3. Run DSE-Patcher (if your version is earlier than 24H2) and disable DSE.
4. Launch Alternative A2DP Driver and install the driver according to the original manual. Check via `Win+R` > `devmgmt.msc` > Sound to ensure everything installed without errors.
    - If the fake signature fails, you will have to repeat this every time Windows boots. However, a `.bat` file is included to simplify the process. DSE-Patcher will still need to be run manually.
5. That's it. If the driver loads correctly after a reboot, everything was successful. Enjoy using it. :)

P.S. If you accidentally installed the original driver, you can remove it like this: `pnputil.exe -f -d C:\Windows\System32\DriverStore\FileRepository\alta2dp.inf_amd64_8adcf7b721e1e624\AltA2DP.inf`
- `alta2dp.inf_amd64_8adcf7b721e1e624` may differ from yours. Go to `C:\Windows\System32\DriverStore\FileRepository\` and find your `alta2dp` folder.

P.P.S. VirusTotal or any antivirus may swear at the driver. This is a normal occurrence for unsigned or fake-signed applications. But it's also about trust. :)

P.P.P.S. Judging by the reviews, it is best to install the ALT version of the driver, as the antivirus may remove the driver version due to a false positive.
