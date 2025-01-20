# TTS_steam_links

If you're having issues in Tabletop Simulator with files saved to the Steam Cloud, and you have some or all asset files cached locally, you can use this script to change broken or all URL's in your file to local file locations. The script will make a backup of the original file as well, so if something does go wrong, you still have the original file. 
The script should work for Windows (tested on Windows 11), Linux (tested on Ubuntu), and MacOS (tested on Sequoia). The script assumes you have installed Tabletop Simulator in the default location for your Operating System. Follow these steps to use this script. 

1. [Have Python installed if you haven't already](https://www.python.org/downloads/). [How to check whether you have Python installed already](https://www.freecodecamp.org/news/check-python-version-how-to-check-py-in-mac-windows-and-linux/) 
2. [Download this project (this link points to a zip of it)](https://github.com/FVMF/TTS_steam_links/archive/refs/heads/main.zip)
3. Unzip the contents of the file downloaded in step 2 to any folder. 
4. Open the terminal (Linux/MacOS) or command prompt (Windows), and navigate to the folder of step 3. Then run this:
   ```
   # Use this one to replace all URLS's in your save file.  
   python point_asset_links_to_local_files.py [FILE_LOCATION_1] [FILE_LOCATION2]

   # Use this one to only replace dead URL's in your save file.
   python fix_dead_TTS_links_with_local_file_links.py [FILE_LOCATION_1] [FILE_LOCATION2]
   ```
   The easiest way to get the file location is to drag and drop the file that you want to change the assets links of to the window of the terminal. Then the file location will be automatically copy-pasted in the terminal window. The script needs at least 1 file location, but can handle multiple files at once by adding more file locations seperated by a space.
6. The terminal should show which URL's were replaced with local links and where you can find the backup file of a copy of the unaltered file.

After you have replaced URL's with local links, you can follow these steps in TTS to upload your locally cached files to the Steam Cloud and fix the URL's the easy way: 
1. Open TTS and open the altered file (the one with the local links). 
2. Go to Modding -> Cloud Manager
3. Click on the button with the up arrow. This will upload all locally cached files of the local links to your Steam Cloud
4. When the uploading is done, save the result.
5. You can share the result on the Steam workshop or directly with other people, and everything should work again. Of course, only files that have you cached locally will be fixed. If there are broken links in your save file for which you don't have the file cached locally, those won't be fixed.  
