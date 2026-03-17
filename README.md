# StyleMix - Outfit Creator

A Pinterest-like app for creating and sharing clothing outfits with automatic color matching analysis.

![StyleMix Screenshot](./screenshot.png)

## Features

- **Dark/Light Theme** - Toggle between themes with the moon/sun button
- **Create Outfits** - Build outfits by combining tops, bottoms, shoes, and outerwear
- **Auto Background Removal** - Uploaded images get their background removed automatically
- **Color Detection** - Automatically detects the dominant color of each clothing item
- **Color Matching** - Analyzes color compatibility between outfit items
- **Drag & Drop** - Arrange your outfit items in the preview canvas
- **Public/Private** - Share outfits publicly or save them privately
- **Profile** - View your posts, likes, and saved outfits

## Tech Stack

- React + TypeScript + Vite
- Tailwind CSS
- shadcn/ui components
- Zustand for state management
- ColorThief for color detection
- Canvas API for background removal

## Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/stylemix.git
cd stylemix

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

### GitHub Pages Deployment

The app is configured to work with GitHub Pages. To deploy:

1. Update `vite.config.ts` with your repository name:
```ts
export default defineConfig({
  base: '/your-repo-name/',
  // ... rest of config
})
```

2. Build and deploy:
```bash
npm run build
# Copy images to dist folder
cp -r public/images dist/
# Deploy dist folder to gh-pages branch
```

## How to Use

1. **Browse Feed** - See outfits from the community
2. **Create Outfit** - Tap the + button to start building
3. **Add Items** - Select from wardrobe or upload new items
4. **Upload** - Drag & drop or select an image. Background will be removed automatically
5. **Check Match** - After adding 2+ items, check color compatibility
6. **Publish** - Arrange items by dragging, then post publicly or save privately

## File Upload

The app supports:
- JPG, PNG, HEIC formats
- Automatic background removal using canvas-based edge detection
- Dominant color detection using ColorThief library

## License

MIT
