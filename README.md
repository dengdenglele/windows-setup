# Optimize your Windows 10/11 setup

## [Disable network configuration during setup/allow local account](https://learn.microsoft.com/en-us/answers/questions/1179311/windows-11-setup-without-internet)
Open a terminal window with shift + F10 and run the following command:

```PowerShell
OOBE\BYPASSNRO
```

The system will reboot and Windows setup will allow a setup without internet connection

## [Debloat with a script from Raphire](https://github.com/Raphire/Win11Debloat)

```PowerShell
& ([scriptblock]::Create((irm "https://win11debloat.raphi.re/")))
```

- Run "(1) Default Mode" to get rid of the rough dirt
- Also run "(3) App removal mode" manually
  - Let it list all installed apps
  - Delete Microsoft Store, apps can be installed and updated manually with PowerShell as Administrator
  - Apps to be kept:
    - Photos (Microsoft.Windows.Photos)
    - Paint (Microsoft.Paint)
    - Calculator (Microsoft.WindowsCalculator)
    - Snipping Tool (Microsoft.ScreenSketch)
  - Run "(2) Custom Mode" to customize taskbar, explorer, context menu, AI stuff and telemetry

## Install Lenovo **Commercial** Vantage on ThinkPad laptops
- No Ads
- Less intrusive

```Powershell
winget search "lenovo commercial vantage"
```
