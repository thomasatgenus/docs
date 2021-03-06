## Administrative Genus Desktop Client Installation - Step by Step

This step by step procedure equals the steps automatically done by the Genus desktop client installation program and the Genus desktop client upgrader.

Please review [Administrative Genus Desktop Client Installation](install-genus-desktop-clients-silently-for-your-users.md) and [Installation Variables](administrative-genus-desktop-client-installation--installation-variables.md "Administrative Genus Desktop Client Installation - Installation Variables") before continuing.

**Step 1**

Decide on an installation root directory and create it, e.g. on a shared file server. Example: _b H:\Programs\Genus\Client\b _.

**Step 2**

Copy the version of the Genus desktop client executable to be deployed to this installation root directory, e.g. _b H:\Programs\Genus\Client\Genus.exeb _.

**Step 3**

In environments running multiple versions of Genus, you must make sure that both the newest and the older versions are located in the folders described in [Genus Desktop Client Installation Files Footprint](install-genus-desktop-client-on-your-computer.md).

**Step 4**

Genus installs custom URL protocol handlers for "genuslink" and "genusstudiolink", used for handling shortcuts inside the Genus desktop client application. The document types _b .genusb _ (Content Type = b application/x-genusb ) is used for downloading genuslink shortcuts from the server and opening them. The following text, with replacement of variables with their values, constitute Registry content which you can save to a file and deploy in your corporate environment:

Windows Registry Editor Version 5.00  

[HKEY_USER_SELECTABLE]  

[HKEY_USER_SELECTABLE\Software]  

[HKEY_USER_SELECTABLE\Software\Classes]  

[HKEY_USER_SELECTABLE\Software\Classes\genusfile]  
@="Genus Shortcut"  
"EditFlags"=dword:00010000  
"IsShortcut"=""  
"NeverShowExt"=""  

[HKEY_USER_SELECTABLE\Software\Classes\genusfile\DefaultIcon]  
@="\"[INSTALLDIR]Genus.exe\",0"  

[HKEY_USER_SELECTABLE\Software\Classes\genusfile\shell]  

[HKEY_USER_SELECTABLE\Software\Classes\genusfile\shell\open]  

[HKEY_USER_SELECTABLE\Software\Classes\genusfile\shell\open\command]  
@="\"[INSTALLDIR]Genus.exe\" \"%1\""  

[HKEY_USER_SELECTABLE\Software\Classes\genuslink]  
@="URL:Genus Link Protocol"  
"URL Protocol"=""  

[HKEY_USER_SELECTABLE\Software\Classes\genuslink\DefaultIcon]  
@="\"[INSTALLDIR]Genus.exe\",0"  

[HKEY_USER_SELECTABLE\Software\Classes\genuslink\shell]  

[HKEY_USER_SELECTABLE\Software\Classes\genuslink\shell\open]  

[HKEY_USER_SELECTABLE\Software\Classes\genuslink\shell\open\command]  
@="\"[INSTALLDIR]Genus.exe\" \"%1\""  

[HKEY_USER_SELECTABLE\Software\Classes\genusstudiolink]  
@="URL:Genus Studio Link Protocol"  
"URL Protocol"=""  

[HKEY_USER_SELECTABLE\Software\Classes\genusstudiolink\DefaultIcon]  
@="\"[INSTALLDIR]Genus.exe\",4"  

[HKEY_USER_SELECTABLE\Software\Classes\genusstudiolink\Shell]  

[HKEY_USER_SELECTABLE\Software\Classes\genusstudiolink\Shell\open]  

[HKEY_USER_SELECTABLE\Software\Classes\genusstudiolink\Shell\open\command]  
@="\"[INSTALLDIR]Genus.exe\" \"%1\""  

[HKEY_USER_SELECTABLE\Software\Classes\.genus]  
@="genusfile"  
"Content-Type"="application/x-genus"  

[HKEY_USER_SELECTABLE\Software\Classes\MIME]  

[HKEY_USER_SELECTABLE\Software\Classes\MIME\Database]  

[HKEY_USER_SELECTABLE\Software\Classes\MIME\Database\Content Type]  

[HKEY_USER_SELECTABLE\Software\Classes\MIME\Database\Content Type\application/x-genus]  
"Extension"=".genus"  

[HKEY_USER_SELECTABLE\Software\Microsoft]  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer]  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer\ProtocolExecute]  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer\ProtocolExecute\genuslink]  
"WarnOnOpen"=dword:00000000  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer\ProtocolExecute\genusstudiolink]  
"WarnOnOpen"=dword:00000000  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer\Low Rights]  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer\Low Rights\ElevationPolicy]  

[HKEY_USER_SELECTABLE\Software\Microsoft\Internet Explorer\Low Rights\ElevationPolicy\{066FE867-F43C-4828-8A0D-F82D25D63426}]  
"Policy"=dword:00000003  
"AppName"="Genus.exe"  
"AppPath"="[INSTALLDIR]"  

**Step 5**

The Genus desktop client installation program enables automatic update of the Genus desktop client application by adding the following information to the Registry:

Windows Registry Editor Version 5.00  
[HKEY_USER_SELECTABLE]  
[HKEY_USER_SELECTABLE\Software]  
[HKEY_USER_SELECTABLE\Software\Genus]  
"IsOfficeAutoUpdateEnabled"=dword:00000001  

If this information is omitted, automatic update of the Genus desktop client application is disabled.

**Step 6**

The Genus desktop client installation program adds a shortcut to the Genus desktop client application in the Windows Start menu as an URL file with the text _b genuslink:b _.

This file is saved on the following location for "Per-Machine" installations:

_CSIDL_COMMON_PROGRAMS\Genus Client\Genus.url_

For "Per-User" installations the file is saved on the following location:

_CSIDL_PROGRAMS\Genus Client\Genus.url_

**Step 7**

If the user, using the Genus desktop client installation program, chooses "Custom Setup", the user will be offered the possibility to create shortcuts to the Genus desktop client application on the desktop.

For "Per-Machine" installations: _CSIDL_COMMON_DESKTOP\Genus.url_.

For "Per-User" installations: _CSIDL_DESKTOP\Genus.url_.