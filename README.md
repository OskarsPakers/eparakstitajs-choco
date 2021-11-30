# eParakstītājs 3.0 Chocolatey

Repository to hold configuration files and instructions to push eparakstitajs to Chocolatey package manager.

# Prerequisites

- Chocolatey command line tool. Obtain from: https://chocolatey.org/install

# Releasing

1. Download .msi installer file for eParakstītājs e.g. `wget https://www.eparaksts.lv/files/ep3updates/eparakstitajs3-1.5.19.msi`
2. Update <version> in eparakstitajs.nuspec file if necessary
2. Create chocolatey package `choco pack`
3. Push package to chocolatey.org repository e.g. `choco push .\eparakstitajs3.1.5.19.nupkg --key <apiKey> --source https://push.chocolatey.org/`