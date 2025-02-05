# En-Dictionary
A GUI based open-source English dictionary for desktop. Feel free to install & use. Also available the code for developers.

# How it works
Since the dictionary doesn't use 'API keys' primarily, it provides you the full customization of the dictionary database.

it has it's own json file as the database. If the word you searched doesn't contain the database, it will use API keys to fetch the word from online & show you the result also save the word in json file. 

Again, if you misspell the searched word it will suggest you the closest similar word.

if the searched word doesn't found in neither json file nor API key, it will simply ask you to enter the result of the word & save it in json file.

Also you can edit the result of the searched word & save the changes in json file.
This code is completely written in python & no need to install python interpreter to excute it.

You can also use keybinding to make a shortcut to excute the app

# Provide
"Definition": 


"Examples": 

"Synonyms": 

"Antonyms": 

# Installation:
To run this program place the 'dict' folder to your home directory & 'dictionary-app' to desktop folder.
Open the folder & excute the 'dictionary-app'

1. Also you can add it to your panel(for XFCE) following the following steps:

	Right-click on the panel (the top/bottom bar in XFCE).

	Select "Panel" → "Add New Items".

	Search for "Launcher" and click "Add".

	A new launcher icon will appear on the panel. Right-click on it and select "Properties".

	Click the "+" button to add a new application.

	Fill in the details:

	Name: Your app name (e.g., "Dictionary").

	Command: The full path to your app’s script or executable (e.g., /home/usr/dictionary-app).

	Icon: Click the icon button and select an image.

	Click "Close", and now your app will be accessible from the panel.


2. Launch the app from the application menu or panel(for XFCE):
   Also you can use my 'dictionary.desktop' file for configuration. Put the file into the following path "~/.local/share/applications/" 
   	Or, Make your own

	Open a terminal & run:

	nano ~/.local/share/applications/dictionary.desktop

	Add the following content(modify as needed):

	[Desktop Entry]

	Version=1.0

	Type=Application

	Name=Dictionary

	Exec=/home/user/dictionary-app

	Icon=/home/user/icon.png

	Terminal=false

	Categories=Utility;


	save(CTRL =X, then 'Y' to confirm)

	Make the file executable:

	chmod +x ~/.local/share/applications/dictionary.desktop

	Right-click on the panel → "Add New Items" → "Launcher" → Add your app.

Note: I use linux software(XFCE edition) & don't know if this program is compitable for other linux distributions, windows or mac. You can give a try to install it. 

If you can't install it please notify me.
If you are a developer feel free to upgrade it. It would be a great help.

For support contact me at
mahmudurahmanmahi26@gmail.com

Thank you 😊
