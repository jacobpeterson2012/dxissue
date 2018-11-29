# SFDX  App
This demostrates the issue with trying to create an unlocked package when "features": ["ContactsToMultipleAccounts"] is part of the package definition.

## Dev, Build and Test
sfdx force:package:create --name TestPackage1 --description "Test package creation" --packagetype Unlocked --path  force-app --nonamespace --targetdevhubusername JacobDevHub

sfdx force:package:version:create -p TestPackage1 -x --wait 600 -v [JacobDevHub]
NOTE: To reploicate issue ensure you have added the reference to the pacakge definition files in the version build request or in the package definition
