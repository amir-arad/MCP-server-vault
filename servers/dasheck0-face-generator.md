---
type: server
repo_url: https://github.com/dasheck0/face-generator
name: Face Generator MCP Server
owner: dasheck0
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/thispersondoesnotexist",
    "purpose/image-generation",
    "purpose/prototyping",
    "purpose/dataset-creation",
    "tech/javascript",
    "tech/image-processing"
  ]
---

# Face Generator MCP Server

#status/active #category/ai #integration/thispersondoesnotexist #purpose/image-generation #purpose/prototyping #purpose/dataset-creation #tech/javascript #tech/image-processing

## Description

Generates customizable human face images using thispersondoesnotexist.com, offering options for shape, dimensions, and batch processing for UI prototyping and dataset creation. It provides an interface to generate synthetic human face images with customizable attributes, leveraging AI to create unique and non-existent faces.

## Features

- Face image generation
- Customizable dimensions
- Shape customization (square, circle, rounded)
- Batch processing
- UI prototyping support
- Dataset creation
- Image format options (png, jpeg)
- Quality settings
- Metadata generation
- Cache management
- AI-powered generation
- Synthetic face creation
- Image manipulation

## Installation

```bash
# Install dependencies
npm install
```

## Usage

```javascript
{
  "mcpServers": {
    "face-generator": {
      "command": "npx",
      "args": ["@dasheck0/face-generator"],
      "env": {
        "OUTPUT_DIR": "./faces",
        "IMAGE_FORMAT": "png",
        "DEFAULT_SIZE": "512x512",
        "BATCH_SIZE": "10"
      }
    }
  }
}

// Tool Parameters
outputDir: Directory to save images (required)
fileName: Optional file name (defaults to timestamp)
count: Number of images to generate (default: 1)
width: Image width in pixels (default: 256)
height: Image height in pixels (default: 256)
shape: Image shape (square|circle|rounded, default: square)
borderRadius: Border radius for rounded shape (default: 32)
```

## Dependencies

- Node.js >= 14
- Internet connection
- Image processing libraries (e.g., sharp)
- Storage space
- Cache system
- thispersondoesnotexist.com API

## Related Servers

- None currently listed