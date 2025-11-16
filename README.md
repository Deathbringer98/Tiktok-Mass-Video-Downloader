# TikTok Video Downloader (Interactive)

`tiktokvdl.py` is a simple Python script that downloads TikTok videos in bulk.  
When you run the script, it *asks you to paste URLs*, one per line, and downloads them all automatically.

Clean, safe filenames are generated (no emojis, no illegal characters, no weird Unicode).

---

## ✅ Features

- Interactive mode — no command-line arguments needed  
- Paste one TikTok URL per line  
- Press ENTER on an empty line to start downloading  
- Auto-cleaned filenames (no emojis, symbols, strange characters)  
- Correct file renaming based on video title + video ID  
- Uses `yt-dlp` for fast and reliable downloading  
- Saves files into a folder called **tiktok_downloads**

---

## 📦 Requirements

Install Python packages:

```sh
pip install yt-dlp
```

---

## ▶️ How to Run

Navigate to the script folder in PowerShell or Terminal:

```sh
python tiktokvdl.py
```

You will see:

```
Enter TikTok URLs (one per line).
Press ENTER on an empty line when done:

> https://www.tiktok.com/@user/video/123
> https://www.tiktok.com/@another/video/456
> 
```

The downloader will process every link and save all videos into:

```
./tiktok_downloads/
```

Each file is renamed like:

```
Cleaned_Title_1234567890.mp4
```

---

## 📁 Folder Structure

```
tiktokvdl.py
tiktok_downloads/
    ├── example_video_12345.mp4
    ├── another_clip_67890.mp4
```

---

## 🛠 How It Works

1. Script prompts the user for URLs  
2. User pastes URLs line by line  
3. URLs are passed to `yt-dlp`  
4. Videos are downloaded using temporary filename (ID.ext)  
5. Script renames each file using a sanitized version of the title  
6. Download complete 🎉

---

## 💡 Notes

- Supports *any* public TikTok link  
- If TikTok changes their system, just update `yt-dlp`:

```sh
pip install -U yt-dlp
```

- You can paste dozens or hundreds of links in one go  

---

## 🔧 Customization

If you want additional features, you can request upgrades such as:

- Load URLs from `.txt`  
- Save URLs to `.txt`  
- Multithreaded downloads  
- Full user-profile download  
- Proxy support  
- Auto-retry failed downloads  

---

## ✔ License

Free to use, modify, and distribute.

---
