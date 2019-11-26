# GNSS_test
Fiddling around with the Myriota API and getting GNSS fixes

The Makefile file has the following changes from the Blinky example:  
The PROGRAM_NAME field is set to GNSS_test  
The ROOTDIR field is set to $(abspath ../..)/SDK  
As far as I can tell, ROOTDIR should point to the SDK directory, and because I made the application folder outside the SDK directory it requires a bit of navigation to get there. The directory system is thus:
 * Documents
   * SDK 
   * Myriota_apps
      * GNSS_test  

What $(abspath ../..)/SDK   does is go back two levels from the current directory (assuming we start in GNSS_test) and then into SDK from there
