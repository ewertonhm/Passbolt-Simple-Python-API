# Passbolt-Simple-Python-API
An easy to use and easy to understand, Windows compatible, Python script for using Passbolt API

Python Requirements: 
- httpx
- python-gnupg

Also you will need the GnuPG software, instructions and downloads can be found here:
https://gnupg.org/download/index.html
* for windows you need to download gpg4win, also found in the gnupg donwload page (scroll to the end). 

How to use:
- First you need to import your passbolt user Private Key to the gnupg, in Windows you do this through the Kleopatra software that comes in with gpg4win.
- Then you need to edit the base_url and gpgbinary in the __init__ function of the PassboltAPI, with your passbolt address (withou the last '/'), and the gpgbinary file location
- Last, you just instanciate the PassboltAPI passing your user fingerprint, it will then ask your passphrase, login, and get the CsrfToke setup for later use.

Then you can just use the already build functions to read/create/update your passbolt or create your own using mines as model. 
