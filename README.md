### Telegram Media Downloader (Youtube, Twitter and TikTok:

![Telegram Media Downloader Cover](images/ImagenPortada.webp)

**Telegram Media Downloader** is a Python-based bot designed to download videos and audios from platforms like YouTube, Twitter/X, and TikTok. If the file exceeds Telegram's 50 MB limit, it automatically compresses the file using `ffmpeg` and sends it to the user. This bot allows easy downloading and conversion of media through simple commands.

## Features

- Download videos and audios from YouTube, Twitter/X, and TikTok.
- Automatically compresses videos larger than 50 MB using `ffmpeg`.
- Provides real-time download progress through Telegram messages.
- Supports both video and audio downloads.
- Simple commands for downloading and managing media files.

## Requirements

To run this bot, you'll need the following dependencies installed:

- Python 3.7+
- `yt-dlp` for downloading media
- `ffmpeg` for video compression
- `python-telegram-bot` library for bot functionality

Install the dependencies using pip:

```bash
pip install yt-dlp python-telegram-bot asyncio
```

## Setup

1. **API Token**: Get your API token from [BotFather](https://core.telegram.org/bots#botfather) on Telegram and update the `API_TOKEN` in the script.
2. **Download Folder**: Set the `TEMP_DOWNLOAD_FOLDER` to a temporary folder where you want media to be downloaded and processed.
3. **ffmpeg Installation**: Make sure `ffmpeg` is installed and available in your system's PATH. You can download it from [ffmpeg.org](https://ffmpeg.org/download.html).

## Usage

- Start the bot using the following command:

```bash
python bot.py
```

- Send `/start` in the bot chat to receive instructions.
- Use the `/download <url>` command to download media. For example:

```
/download https://www.youtube.com/watch?v=example
```

By default, the bot will download videos. To download audio, you can specify the format:

```
/download https://www.youtube.com/watch?v=example audio
```

## Compression

If the downloaded media file exceeds the 50 MB limit imposed by Telegram, the bot will automatically compress the video to fit within the size restriction using `ffmpeg`.

## Example Commands

- `/start`: Introduction and usage instructions.
- `/download <url> [audio]`: Download a video or audio from the given URL.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributions

Feel free to submit pull requests to enhance the functionality of the bot or to fix any issues. All contributions are welcome!

---

### Disclaimer

This bot is intended for educational and personal use. Please comply with the respective platform's terms of service when downloading content.
```
