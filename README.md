# Mnemosyne

**A portable video archiver for YouTube channels and individual videos from yt-dlp-supported sites.** Choose video quality, downscale with FFmpeg, embed subtitles and cover art, select custom or hardware video codecs, and organize downloads in flat folders or one folder per video.

## Features

- Archive a YouTube channel or download a single video URL from a site supported by yt-dlp.
- Select video quality, audio-only downloads, output container, and an optional maximum output height.
- Embed available English subtitles and thumbnail artwork into the media file, or save sidecar files.
- Choose built-in FFmpeg codecs, enter a custom encoder name, or prefer CPU, NVIDIA, AMD, or Intel encoding.
- Save videos directly in a channel folder or create a separate subfolder for each video.
- Optionally save descriptions, metadata, subtitles, channel artwork, Shorts, and past live streams.
- Pause, resume, cancel, and retry failed downloads. An archive file helps skip videos already saved.
- Use optional YouTube browser sign-in and slower request pacing.

## Quick setup

1. Download and extract the Mnemosyne ZIP. Keep the files together in one folder.
2. Start the app for your computer:
   - **Windows:** double-click `Start-Windows.bat`.
   - **macOS:** double-click `Start-macOS.command`.
   - **Linux:** run `bash Start-Linux.sh` in a terminal.
3. Mnemosyne opens in your browser. On first launch, choose **Download tools** to get yt-dlp and FFmpeg.
4. Choose **Channel archive** or **Single video / other supported site**, paste a link, and press **Check**.
5. Choose your download settings and press **Download**. Files are saved in the `downloads` folder beside the launcher.

Mnemosyne needs Python 3.9 or newer. For full YouTube support, install Node.js 22 or newer or Deno 2.3 or newer if a supported runtime is not already available on your computer.

## Output layout

By default, channel downloads are saved under `downloads/<channel>/`, with a subfolder for each video. Turn off **One subfolder per video** in **Advanced settings** to put the videos directly in the channel folder. Single-video downloads go under `downloads/Videos/`.

Subtitles and cover images are embedded by default when the media format supports them. Turn on optional sidecar settings in the app to save extra files. Use **Update yt-dlp** if a supported website changes and downloads stop working.

For more detailed instructions and troubleshooting, see [`files/README.md`](files/README.md).
