# Rocky 10.2 for Grid5000

## Issues right now:
- Min image does not auto-create Grid5000 user account
- TPM is default enabled, needs to be disabled for deployment to the older nodes.
- Setup needed to be done with VNC for checking the deploy disk and kernel parameters in Kameleon

## What works
- Rocky10-x64-nfs is autocreating user and mounting the home directory from the login node
- EESSI mounting for rocky has been tested, works
- Easybuild installation worked in LMOD

## What will be tested in the coming weeks
- Deployment to Vianden-1 to check rocm-compatibility and if the issue with kernel crashes observed in Rocky9.7 persists
- flux scheduling on this specific image with various node configurations
- more LMOD
  
## How the build process works

Build it with the normal `kameleon3` command, but before, relocate all files from here to their respective corresponding directories in the default environment recipes.
