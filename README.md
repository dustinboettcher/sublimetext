<b>Preferences.sublime-settings</b><br>
a basic config to enhance the workflow with sublime.

<b>Soda Dark 3.sublime-theme</b><br>
a slight modification of the main SODATheme - basically thinner tabs.

<b>1) Install Manager</b>

Access the console via ctrl+` shortcut or the View > Show Console menu. Once open, paste the appropriate Python code for your version of Sublime Text into the console.

<i>Sublime3</i>

import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

<i>Sublime2</i>

import urllib2,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')

<b>2) Install Package</b>

Open the palette, press ctrl+shift+p (Win, Linux) or cmd+shift+p (OS X). All Package Control commands begin with Package Control:, so <b>start</b> by typing Package or Install.

Search for SODATheme proceed with Enter.

<b>3) "Install" Files</b><br>
Copy the Files from the repository in your personal folder. Go to Preferences > Browse Packages. Put the files in the "User" folder.


<b>HINT</b><br>
Install the Package "sFTP" a great way to modify documents on a web server. Don't forget to open the  View > SideBar > Folders.
