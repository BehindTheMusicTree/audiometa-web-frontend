# AudioMeta Web

[![License](https://img.shields.io/badge/license-Apache%202.0-green.svg)](LICENSE)

A web-based interface for the AudioMeta Python library, allowing users to upload audio files, read their metadata, and update metadata fields through an intuitive web interface built with Next.js.

**Backend**: See [audiometa-web-api](https://github.com/BehindTheMusicTree/audiometa-web-api) - Powered by [AudioMeta Python](https://github.com/Andreas-Garcia/audiometa) - A powerful, unified Python library for reading and writing audio metadata across multiple formats.

## 🔒 Privacy & Data Handling

**Important**: This application does not store any uploaded files or metadata permanently. All processing is done in memory, and files are deleted immediately after processing. Your audio files and metadata remain private and are never saved to disk or transmitted elsewhere.

## ✨ Features

- **File Upload**: Securely upload MP3, FLAC, and WAV audio files
- **Metadata Reading**: View comprehensive metadata including technical information
- **Metadata Editing**: Update metadata fields with validation
- **Format Support**: Full support for ID3v1, ID3v2, Vorbis, and RIFF metadata formats
- **Web Interface**: Clean, responsive web UI for easy metadata management
- **Batch Operations**: Process multiple files efficiently
- **Validation**: Built-in metadata validation before updates

## 📦 Installation

### Prerequisites

- Node.js 18+ (for Next.js frontend)
- Backend API running (see [audiometa-web-api](https://github.com/BehindTheMusicTree/audiometa-web-api))

### Frontend Setup

1. Clone this repository:

```bash
git clone https://github.com/BehindTheMusicTree/audiometa-web.git
cd audiometa-web
```

2. Install dependencies:

```bash
npm install
```

3. Configure the backend API URL in your environment variables or config file.

4. Start the development server:

```bash
npm run dev
```

The frontend will be available at `http://localhost:3000` (default Next.js port).

## 🚀 Running the Application

### Prerequisites

Ensure the backend API from [audiometa-web-api](https://github.com/BehindTheMusicTree/audiometa-web-api) is running and accessible.

### Development Mode

```bash
npm run dev
```

The application will be available at `http://localhost:3000`

### Production Build

```bash
npm run build
npm start
```

## 💻 Usage

1. **Upload Files**: Use the web interface to upload your audio files (MP3, FLAC, WAV)
2. **View Metadata**: Browse and inspect metadata for uploaded files
3. **Edit Metadata**: Update fields like title, artist, album, rating, etc.
4. **Download Updated Files**: Download files with updated metadata

### Supported Operations

- **Read Metadata**: View all metadata fields and technical information
- **Update Metadata**: Modify metadata with real-time validation
- **Delete Metadata**: Remove specific fields or all metadata
- **Format Conversion**: Migrate metadata between formats
- **Batch Processing**: Handle multiple files simultaneously

## 🛠️ Technology Stack

- **Frontend**: Next.js (React framework) for the web interface
- **Backend**: Separate Python Flask/FastAPI API (see [audiometa-web-api](https://github.com/BehindTheMusicTree/audiometa-web-api))
- **Communication**: REST API calls to the backend
- **Styling**: CSS/Tailwind (or your preferred styling solution)

## 💻 Command Line Interface

Unlike the original [AudioMeta Python library](https://github.com/Andreas-Garcia/audiometa) which provides a command-line interface, this web version focuses on a graphical web interface for metadata management. For command-line operations, use the original AudioMeta Python CLI directly.

If you need CLI functionality for this web app, you could potentially create an npm-based CLI that interacts with the web API, but this is not currently implemented.

## 📁 Project Structure

This repository contains only the Next.js frontend code. The backend API is in a separate repository: [audiometa-web-api](https://github.com/BehindTheMusicTree/audiometa-web-api).

```
audiometa-web/
├── package.json          # Node.js dependencies
├── pages/               # Next.js pages
├── components/          # React components
├── public/              # Static assets
├── styles/              # CSS styles
├── utils/               # Frontend utilities
├── README.md            # This file
└── next.config.js       # Next.js configuration
```

## 🤝 Contributing

Contributions are welcome! Please see the [AudioMeta Python contributing guidelines](https://github.com/Andreas-Garcia/audiometa/blob/main/CONTRIBUTING.md) for details.

## 📄 License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

## 🙏 Acknowledgments

- [AudioMeta Python](https://github.com/BehindTheMusicTree/audiometa) - The core audio metadata library
- [Andreas Garcia](https://github.com/Andreas-Garcia) - Original AudioMeta library author
