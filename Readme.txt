Usage Instructions
Option 1: Manually Paste a YouTube Link
    -Run YouTubeVideoDownloderV2.exe 
    -Select Option 1.    
    -Paste a YouTube link and press Enter.
    -Repeat for multiple links.
Type done to start downloading.
Option 2: Read from LinkReader.txt
    -Create a file named LinkReader.txt (Should already be Present) in the same folder as the EXE.
    -Add one YouTube link per line.
    -Run VideoDownloader.exe and choose Option 2.
    -The script will download all videos listed in LinkReader.txt.

Where Are Videos Saved?
All downloaded videos are stored in the Results/ folder in the same directory as the EXE.

Logging
    A log file is saved in the Logs/ folder.
    The file name format is log_DD_MM_YYYY_HH_MM_SS.txt.
    It contains download success/failure messages.

Troubleshooting
    "Error: LinkReader.txt not found!"
    Make sure LinkReader.txt is in the same folder as VideoDownloader.exe.


!!Do not place the EXE inside a system folder (like AppData\Local\Temp).

-"ffmpeg is not installed"
    --This happens when yt-dlp tries to merge video/audio but ffmpeg is missing. 
    Fix this using the following command in CMD or Powershell.
        choco install ffmpeg  # Windows (via Chocolatey)
        brew install ffmpeg   # macOS (via Homebrew)
        sudo apt install ffmpeg  # Linux