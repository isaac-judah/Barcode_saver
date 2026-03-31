# Barcode Lists

A Chrome extension for managing barcode lists with category organization and cloud sync.

## Features

- Organize barcodes into categories
- Add, rename, and delete categories
- Drag-and-drop category reordering
- Copy barcodes to clipboard
- Cloud sync via Supabase (optional)
- Offline support with local storage
- Dark theme UI

## Permissions Used

- **storage**: Local data persistence for barcodes and categories
- **sidePanel**: Opens in Chrome side panel for quick access
- **host_permissions**: https://*.supabase.co/* for cloud sync

## Installation

1. Download the extension files
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode"
4. Click "Load unpacked" and select the extension folder

## Usage

1. Enter your store number and password to login
2. New stores are created automatically on first login
3. Add categories using the + button
4. Add barcodes by typing and pressing Enter or clicking Add
5. Data syncs to cloud when online (optional)