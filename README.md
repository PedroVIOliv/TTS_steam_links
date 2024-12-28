# TTS_steam_links

If you're having issues in Tabletop Simulator with files saved to the Steam Cloud, and you have all asset files cached locally, you can use this script to change all the URL's in your file to local file locations. The script will make a backup of the original file as well, so if something does go wrong, you still have the original file. 
The script should work for Windows (tested on Windows 11), Linux (tested on Ubuntu), and MacOS (tested on Sequoia). The script assumes you have installed Tabletop Simulator in the default location for your Operating System. Follow these steps to use this script. 

1. [Have Python installed if you haven't already](https://www.python.org/downloads/)
2. [Download this project (this link points to a zip of it)](https://github.com/FVMF/TTS_steam_links/archive/refs/heads/main.zip)
3. Unzip the contents of the file downloaded in step 2 to any folder. 
4. Open the terminal, and navigate to the folder of step 3. Then run this:
   ```
   python point_asset_links_to_local_files.py [FILE_LOCATION_1] [FILE_LOCATION2]
   ```
   The easiest way to get the file location is to drag and drop the file that you want to change the assets links of to the window of the terminal. Then the file location will be copy-pasted in the terminal window. The script needs at least 1 file location, but can handle multiple files at once by adding more file locations seperated by a space.
6. The terminal should show which URL's were replaced with local links and where you can find the backup file.
