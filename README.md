# Art Print - Epson P9750 Print Manager

A web-based application for managing and printing large format art on the Epson SureColor P9750 (44" wide, 10-color UltraChrome PRO).

## Features

- **Print Tab**: Drag & drop images, analyze resolution/DPI, select print sizes
- **My Collection**: Browse 161 high-res art images with thumbnails, filter by artist
- **Printer Settings**: 30+ paper profiles (Epson, Arches, Hahnemuhle, Canson, Moab)
- **Sources Tab**: Museum links and collector information

## Supported Artists

| Artist | Images | Resolution |
|--------|--------|------------|
| Andy Warhol | 60 | 2000-3000px |
| Keith Haring | 6 | 2000-3000px |
| Shepard Fairey | 95 | 2160-4800px |

All images are 2000px+ minimum, suitable for 40" prints at 300-600 DPI with AI upscaling.

## Print Size Presets

- **Warhol Original Sizes**: 36x36" (Marilyn), 38x38" (Moonwalk), 40x40" (Lennon)
- **Arches Sheet Sizes**: 20x28", 27x39" (with 1" margin)
- **Standard Sizes**: 24x24", 30x30", 24x36", 30x40"

## Paper Profiles

Pre-configured for:
- Epson Premium (Matte, Luster, Glossy, Canvas, Velvet, Hot/Cold Press)
- Arches (Aquarelle, BFK Rives, 88)
- Hahnemuhle (Photo Rag, Bamboo, German Etching, Torchon)
- Canson Infinity (Rag Photographique, Platine, Aquarelle)
- Moab (Entrada, Somerset)
- Red River (Aurora, Polar Matte)

## Printer Settings

- **Black Ink Mode**: Auto-switch between Matte Black and Photo Black
- **Platen Gap**: Auto/Wide/Wider/Widest for different paper thicknesses
- **Suction Control**: Standard to Off for curled/thick papers
- **Drying Time**: Standard/Longer/Longest
- **Color Management**: Adobe RGB, sRGB, or Printer Manages Colors

## Upscaling Workflow

For 40" prints at 300 DPI (12,000px required):

1. Download high-res source (2000px+)
2. Upscale 6x with Topaz Gigapixel AI
   - Model: Standard or Art & CG
   - Output: 16-bit TIFF, Adobe RGB
3. Open in Art Print app
4. Select paper and print settings
5. Print

## Usage

1. Open `index.html` in a browser
2. Add images to `/Images/` folder organized by artist
3. Browse collection or drag & drop new images
4. Configure print settings
5. Click Print to open system print dialog

## Local Setup

```
/Users/johnshay/ArtPrint/
├── index.html          # Main application
├── README.md           # This file
└── Images/             # Local images (not in git)
    ├── Warhol/         # 60 high-res images
    ├── Haring/         # 6 high-res images
    └── ShepardFairey/  # 95 high-res images
```

## Notes

- Images are stored locally (not in GitHub due to size)
- For educational/personal use only
- Recommended: AI upscaling before printing large formats

## License

Personal use only. Art images are subject to their respective copyrights.
