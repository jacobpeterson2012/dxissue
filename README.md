# SFDX  App

## Dev, Build and Test
sfdx force:package:create --name TestPackage1 --description "Test package creation" --packagetype Unlocked --path  force-app --nonamespace --targetdevhubusername JacobDevHub

sfdx force:package:version:create -p TestPackage1 -x --wait 600 -v [JacobDevHub]

## Resources


## Description of Files and Directories


## Issues


