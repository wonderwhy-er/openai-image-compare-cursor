# Made as part of Live Coding Olympics
[![Watch the video](https://img.youtube.com/vi/xySgNhHz4PI/0.jpg)](https://youtu.be/xySgNhHz4PI)

Full results with links:
https://docs.google.com/spreadsheets/d/1kgnVU6NZVTwqtUkrNetXTpm0oY7NsYGJn61u6-JMIoI/edit?usp=sharing

# OpenAI Image Compare - Made with Cursor and Sonnet 3.7 for Vibe Coding comparison

A simple web-based tool to compare image generation results from different OpenAI models:
- DALL-E 2
- DALL-E 3 (Standard quality)
- GPT-4 Vision (gpt-image-1) - Latest model

This tool allows you to generate images using the same prompt across all three model configurations, showing the progression and improvements in OpenAI's image generation capabilities.

![OpenAI Image Compare Screenshot](screenshot.png)

## Live Demo

Access the live demo: [https://wonderwhy-er.github.io/openai-image-compare-cursor](https://wonderwhy-er.github.io/openai-image-compare-cursor)

## Usage

1. Open the demo page in your web browser
2. Enter your OpenAI API key (never stored - it remains in your browser)
3. Enter a prompt for image generation
4. Click "Generate Images"

## Running Locally

Simply clone this repository and open `index.html` in your browser:

```bash
git clone https://github.com/wonderwhy-er/openai-image-compare-cursor.git
cd openai-image-compare-cursor
# Open index.html in your browser
```

## Requirements

- An OpenAI API key with access to image generation models
- A modern web browser
- Internet connection

## API Limitations

- Image generation costs credits on your OpenAI account
- DALL-E 2: Generates 512x512 images and returns a URL
- DALL-E 3 (Standard): Generates 1024x1024 images and returns a URL
- GPT-4 Vision (gpt-image-1): Generates 1024x1024 images and returns base64-encoded image data

## Response Format Differences

Note that each model returns data in a different format:
- DALL-E 2 and DALL-E 3 return a URL to the generated image
- GPT-4 Vision (gpt-image-1) returns the image directly as base64-encoded data in the `b64_json` field

## Privacy & Security

Your API key is only used in your browser to make direct API calls to OpenAI. It is never stored or transmitted to any other server.

## Deployment to GitHub Pages

1. Fork or clone this repository
2. Go to your repository settings
3. Navigate to the Pages section
4. Select the main branch as the source
5. Your site will be published at `https://wonderwhy-er.github.io/openai-image-compare-cursor`

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT 
