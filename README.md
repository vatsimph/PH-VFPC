# PH-VFPC Plugin 

[![Github](https://img.shields.io/github/v/release/vatsimph/PH-VFPC?color=%23F56040)](https://github.com/vatsimph/PH-VFPC/releases/latest)

[![Discord](https://img.shields.io/discord/275064722678743042.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://vats.im/vatphil-discord)  [![Facebook](https://img.shields.io/badge/-Philippines%20vACC-e84393?label=&logo=facebook&logoColor=ffffff&color=3b5998&labelColor=2f477a)](https://www.facebook.com/philippinesvacc/) [![Instagram](https://img.shields.io/badge/-@vatphil-e84393?label=&logo=instagram&logoColor=ffffff&color=ada332&labelColor=9c922c)](https://www.instagram.com/vatphil/)

The PH-VFPC (Philippines Virtual Flight Plan Checker) plugin for EuroScope is used by vACC controllers in the Philippines to review flight plans against pertinent route and altitude constraints. It was originally created by [hpeter2](https://github.com/hpeter2) and [DrFreas](https://github.com/DrFreas) and adapted by the Philippines vACC from the vatsimhk repository. To better meet the demands of the vACC, it has been improved with updated features. The original plugin's codebase is available [here](https://github.com/hpeter2/VFPC). 

As a result, the code will continue to be available for download for free on all controllers. However, other vACCs may find the original plugin's adaptability to be more beneficial if they wish to develop or alter a similar flight plan checker.

This plugin is still under development. Thus, there may still be logical errors and overall instability. Flight controllers shouldn't just rely on this plugin to validate flight plans, especially inexperienced ones.

**While it will be of considerable assistance to delivery controllers, it cannot resolve more significant route problems.** Delivery controllers must still carefully review each flight plan before releasing it.

## Features
- Tag item VFPC: Shows check-result as green 'OK!' or red 'FPL!' ('SID' = No valid SID found, 'ENG' = Failed Engine type restriction, 'E/O' = Failed even/odd Flightlevel, 'MIN' = Failed minimum Flight Level, 'MAX' = Failed maximum Flightlevel)
- Tag function 'Check FP': Explains the check-result in chat output
- Chat command '.vfpc reload': reload the Sid.json config
- Chat command '.vfpc check': checks currently selected AC and outputs result
- Restrictions customizable in Sid.json config
- Checks Even/Odd Flightlevel restriction
- Checks Minimum & Maximum Flightlevel restriction
- Check condition 'route must contain airway' available
- Check condition 'destination must be' available
- Check condition 'aircraft type must be' available (? - unknown, P - piston, T - turboprop/turboshaft, J - jet, E - electric)

## How to use
### Load up the plugin
- Proceed to ```Other Set > Plug-ins```
![Plugin Dialog](https://i.imgur.com/a1knt0u.png)
- Add Tag Item type & function to Departure List (See full instruction [here](https://github.com/hpeter2/VFPC#how-to-use))
![Edit](https://camo.githubusercontent.com/3d68db61053fa95e7d36f87dcade765bd66aa0af53e9f52f598287d880a6d8ff/68747470733a2f2f692e696d6775722e636f6d2f6b51727456664e2e706e67)

If you get an error on load, please install the [latest C++ redistributables](https://aka.ms/vs/17/release/vc_redist.x86.exe)

## Report a Bug
You can create an issue [report](https://github.com/vatsimph/PH-VFPC/issues) with a brief description of the bug/problem and we will address it for the next release.

## Contribute
All vACC certified controllers and staff members are eligible to contribute to the sector file. Feel free to send me an email on [kenzo.tayko@vatphil.com](mailto:kenzo.tayko@vatphil) with your Github Username and your VATSIM CID for the mere reason to verify your identity. Contributions from unverified accounts will not be accepted/merged.

Once the verification is finish, you can now modify the plugin contents by forking this repository and pulling a request for merging.
