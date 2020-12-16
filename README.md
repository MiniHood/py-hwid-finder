# py-hwid-finder


This was for my cheat loader for the HWID lock which is crappy but works, here's the HWID finder I used, I made it but you can plaster your name on it or whatever you got full rights to it now. Enjoy!


Source Code:

import subprocess
import requests
import time
import sys
import os
"""
Yeah I know, why all the imports, uhh so pretty much. I can't remember what import I used for it so I just imported them all, it's probably none of them but fuck it :shrug:
"""
hwid = str(str(subprocess.check_output('wmic csproduct get uuid')).strip().replace(r"\r", "").split(r"\n")[1].strip())
print("HWID: " + hwid)
os.system('pause >NUL')
