# Optimize your Windows 10/11 setup

## [Debloat with a script from Raphire](https://github.com/Raphire/Win11Debloat)

```PowerShell
& ([scriptblock]::Create((irm "https://win11debloat.raphi.re/")))
```

- Run "(1) Default mode" to get rid of the rough dirt
- Also run "(3) App removal mode" manually
  - Let it list all installed apps
  - Delete Microsoft Store, apps can be installed and updated manually with PowerShell as Administrator
  - Apps to be kept include: Photos, Calculator, Snipping Tool (Sketch)

## Install Lenovo **Commercial** Vantage on ThinkPad laptops
- No Ads
- Less intrusive

```Powershell
winget search "lenovo commercial vantage"
```
