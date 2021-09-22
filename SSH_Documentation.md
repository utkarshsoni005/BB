### SSH FOR WINDOWS

1. Open https://github.com/PowerShell/Win32-OpenSSH/releases in any browser.
2. Click on the latest version of ssh.
    - e.g. V8.6.0.0p1-Beta
3. In the asset section download the OpenSSH based on your windows architecture.
	- For 64 bit Windows:
		- Download : OpenSSH-Win64.zip
	- For 32 bit Windows:
		- Download : OpenSSH-Win32.zip
4. Extract the downloded files using any extractor e.g. Winrar.
5. Open CMD on the extracted folder and execute below cmd.
		ssh

# Setting environment variable for openSSH.
1. Right-click the Computer icon and choose Properties, or in Windows Control Panel, choose System.
2. Choose Advanced system settings.
3. On the Advanced tab, click Environment Variables.
4. Select Path variable in system and click edit.
	- To edit Path variable in windows 7 and windows  8.
		- To append new path, add a new path seperated by semicolon " ; ".
		- Add path of openSSH that we have extracted in above steps.
			- e.g. C:\Downloads\OpenSSH-Win64\
	- To edit path in widnows 10.
		- Click on New to add a new path in the list.
		- Add path of openSSH that we have extracted in above steps.
		 	- e.g. C:\Downloads\OpenSSH-Win64\
5. After modifying the environment variable, click Apply and then OK to have the change take effect.



# Generate an SSH key pair in Windows 
1. Press the Windows key.
2. Type cmd.
3. Under Best Match, right-click Command Prompt.
4. Click Run as Administrator.
5. In the command prompt, type the following:
	 	ssh-keygen
6. By default, the system will save the keys to C:\Users\your_username/.ssh/id_rsa. You can use the default name, or you can choose more descriptive names. This can help distinguish between keys, if you are using multiple key pairs. To stick to the default option, press Enter.
7. You'll be asked to enter a passphrase. Hit Enter to skip this step.
8. The system will generate the key pair, and display the key fingerprint and a randomart image.
9. Open your file browser.
10. Navigate to C:\Users\your_username/.ssh.
11. You should see two files. The identification is saved in the id_rsa file and the public key is labeled id_rsa.pub. This is your SSH key pair.
