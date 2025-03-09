# M3U Playlist Generator

A simple Python script to generate M3U playlists with custom display names for TV shows and media collections. This tool allows for bulk input of media links and organizes them into seasons and episodes with customizable naming formats.

## Features

- Bulk input of media links with automatic parsing
- Season and episode organization
- Custom display names without modifying the original links
- Support for various media file extensions (.mkv, .mp4, .avi, .mov, .flv)
- Preview of custom names before finalizing
- Easy to use command-line interface
- Compatible with VLC and other media players that support M3U playlists

## How It Works

The script takes media links (local paths or URLs) and generates an M3U playlist file that can be opened in media players like VLC. While preserving the original links to ensure they remain functional, the script allows you to customize how episodes appear in your media player's interface using the standard "ShowName S01E01" format.

## Usage

1. Run the script: `python m3u_playlist_generator.py`
2. Enter the base filename to use for display (e.g., "ShowName")
3. Enter the number of seasons
4. For each season:
   - Enter the number of episodes
   - Paste all links (one per line or continuous text)
   - Choose whether to use custom naming format
   - Review and confirm the custom display names
5. Enter the name for the M3U file
6. Open the generated M3U file in your media player

## Example

```
Welcome to the M3U Playlist Generator
====================================
Enter the base filename to use for display (e.g., 'ShowName'): Breaking Bad

Enter the number of seasons: 1
Enter the number of episodes for Season 1 (or type 'esc' to create file now): 2

Paste all links for Season 1 (one per line or continuous text).
Make sure each link ends with a file extension like .mkv or .mp4
When finished, press Enter twice:

http://example.com/episode1.mkv
http://example.com/episode2.mkv

Do you want to use custom naming format for Season 1 (e.g., 'ShowName S01E01')? (y/n): y

Preview of custom display names:
Episode 1:
  Link: http://example.com/episode1.mkv
  Display Name: Breaking Bad S01E01
Episode 2:
  Link: http://example.com/episode2.mkv
  Display Name: Breaking Bad S01E02

Do you want to use these custom display names? (y/n): y

Enter the name for the M3U file (including .m3u extension): breaking_bad.m3u

M3U file 'breaking_bad.m3u' generated successfully! Open it in VLC.
```

## Requirements

- Python 3.6 or higher

## Installation

Simply download the script and run it with Python:

```bash
python m3u_playlist_generator.py
```

## License

MIT

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
