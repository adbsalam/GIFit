# GIFit

This script converts video files (`.mp4` or `.mov`) into GIFs.

## Usage

### Basic Syntax

`bash /location/to/adb_gifit /path/to/file.mp4 [fps] [width]`

### Parameters

- **`/path/to/file.mp4`**: The path to the video file you want to convert. The file can be in `.mp4` or `.mov` format.
- **`fps`** *(optional)*: Frames per second for the output GIF. If not provided, the default value is `5`.
- **`width`** *(optional)*: Width of the output GIF in pixels. The height will be scaled to maintain the aspect ratio. If not provided, the default width is `300`.

### Example Commands

- **Convert a `.mp4` file with default settings (5 fps, 300 width):**

```bash
bash /location/to/adb_gifit /path/to/file.mp4
```

- **Convert a `.mov` file with custom settings (10 fps, 640 width):**

```bash
bash /location/to/adb_gifit /path/to/file.mov 10 640
```

- **Convert a `.mp4` file with a custom frame rate (15 fps) (width will be set to default 300):**

```bash
bash /location/to/adb_gifit /path/to/file.mp4 15
```

## Notes
- Ensure that the path to the video file is correct and accessible.
- The script assumes that you have permissions to read the video file and write the output files to the same directory.

## Troubleshooting
- **Command Not Found Errors:** Ensure that `Homebrew` is installed correctly.
- **Command Not Found Errors:** Ensure that `ffmpeg` and `convert` (from ImageMagick) are correctly installed and available in your system's PATH.
- **File Type Errors:** Only `.mp4` and `.mov` files are supported. Ensure your file has a correct extension.

To Install 

- **Homebrew**
- **ffmpeg** (video processing)
- **ImageMagick** (image processing)

You can install these tools using Homebrew with the following commands:

```bash
brew install ffmpeg
brew install imagemagick
```
