


# video2pdfslides

**video2pdfslides** is a Python tool that converts video presentations into PDF slide decks by capturing unique frames as screenshots.

## Overview

This tool extracts distinct frames from a video, saves them as images, and compiles these images into a PDF. It’s designed for creating slide decks from video presentations, ideal for turning recorded talks or tutorials into shareable PDF formats.

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/CODERdotEXE/video2pdfslides.git
   cd video2pdfslides
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the script:**

   ```bash
   python video2pdfslides.py <video_path>
   ```

   Replace `<video_path>` with the path to your video file. The script will:

   - Capture unique frames from the video.
   - Save these screenshots in the `output` folder.
   - Pause for manual verification of screenshots to remove any duplicates.
   - Continue and generate a PDF from the verified screenshots.

2. **Example Commands:**

   ```bash
   python video2pdfslides.py "./input/Test Video 1.mp4"  # Produces 4 unique slides
   python video2pdfslides.py "./input/Test Video 2.mp4"  # Produces 19 unique slides
   ```

   Note: Sample videos are available in the `./input` directory for testing.

## Customization

The default settings work well for standard video presentations. For videos with extensive animations or unusual content, you might need to adjust parameters to avoid duplicate or missing slides.

**Key Parameters to Tweak:**
- `MIN_PERCENT`: Minimum threshold for detecting unique frames.
- `MAX_PERCENT`: Maximum threshold for detecting unique frames.
- `FGBG_HISTORY`: History parameter for background subtraction.

Adjust these parameters in the code comments to fine-tune results for your specific video.

## Contributing

Feel free to submit issues or pull requests to improve this project. Contributions are always welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Happy slide creating!

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-blue)](https://github.com/CODERdotEXE/video2pdfslides)


