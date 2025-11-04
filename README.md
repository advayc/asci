# ASCII Art Converter

A Next.js web application that converts images into ASCII art with customizable parameters.

## Features

- **Image Upload**: Drag and drop or click to upload images
- **Real-time Conversion**: Instantly converts images to ASCII art
- **Customizable Parameters**:
  - Resolution slider to adjust detail level
  - Multiple character sets (Standard, Detailed, Blocks, Minimal)
  - Grayscale or colored ASCII output
  - Color inversion option
- **Responsive Design**: Works on desktop and mobile devices
- **Export Options**: Copy to clipboard or download as text file

## Getting Started

### Prerequisites

- Node.js 18+ installed on your machine
- npm (comes with Node.js)

### Installation

1. The project is already set up in the current directory

2. Install dependencies (if not already installed):
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## Usage

1. **Upload an Image**: 
   - Click the Upload button or drag and drop an image onto the preview area
   - Supported formats: JPG, PNG, GIF, WebP

2. **Adjust Settings**:
   - **Resolution**: Control the detail level (lower = more detail, but larger output)
   - **Character Set**: Choose from different ASCII character sets
   - **Grayscale Mode**: Toggle between grayscale and colored output
   - **Invert Colors**: Reverse the brightness mapping

3. **Export**:
   - Click "Copy ASCII Art" to copy to clipboard
   - Click the download icon to save as a .txt file

## Project Structure

```
asci/
├── src/
│   ├── app/
│   │   ├── page.tsx          # Main page component
│   │   ├── layout.tsx        # Root layout
│   │   └── globals.css       # Global styles
│   ├── components/
│   │   ├── ascii-converter.tsx  # Main ASCII converter component
│   │   └── ui/               # Reusable UI components
│   │       ├── button.tsx
│   │       ├── label.tsx
│   │       ├── select.tsx
│   │       ├── slider.tsx
│   │       └── switch.tsx
│   └── lib/
│       └── utils.ts          # Utility functions
├── public/
│   └── images/
│       └── dark.png          # Placeholder image
└── package.json

```

## Technologies

- **Next.js 14**: React framework with App Router
- **TypeScript**: Type-safe JavaScript
- **Tailwind CSS v4**: Utility-first CSS framework
- **Radix UI**: Accessible component primitives
- **Lucide React**: Icon library

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## Development Notes

- The ASCII converter runs entirely client-side using HTML5 Canvas API
- Image processing is done in real-time without server uploads
- The component supports both grayscale and colored ASCII art
- Adjustable panel widths for desktop viewing (drag the divider)

## License

MIT

## Credits

Built with Next.js and modern web technologies.
