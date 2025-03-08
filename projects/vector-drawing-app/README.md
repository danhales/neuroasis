# Vector Drawing Exchange Application

A web-based application that facilitates sketch exchanges between humans and AI using a lightweight vector format. This project demonstrates effective collaborative development patterns and creates a practical tool for visual communication in AI-human interactions.

![Vector Drawing App Screenshot](../docs/images/app-screenshot.png)

## Project Background

This application was created through a collaborative process between a human developer and an AI assistant (Claude). It evolved from a practical need to exchange sketches during conversations, addressing limitations with previous approaches using base64-encoded images.

The project demonstrates:
- Effective prompt engineering for collaborative development
- Progressive refinement of solutions through dialogue
- Balancing functionality with educational value
- A vector-based approach to sharing visual information in text formats

## Key Features

- **Canvas Drawing Interface**: Draw freely using mouse or Apple Pencil
- **Vector Data Format**: Lightweight, text-based format for sketches
- **Color & Width Options**: Customize line appearance
- **Import/Export System**: Easy exchange of sketches with AI assistants
- **Educational Codebase**: Thoroughly commented for learning

## How to Use

1. **Download the HTML file**: Save the `index.html` file from the `src` directory
2. **Open in a browser**: Double-click the file or drag it into any modern web browser
3. **Draw on the canvas**: Use your mouse, touchpad, or Apple Pencil (via Sidecar)
4. **Export your drawing**: Go to the "Exchange" tab and click "Generate Sketch Data"
5. **Share with Claude**: Copy the generated data and paste it into your conversation
6. **Import Claude's sketches**: Copy sketch data from Claude, paste in the import box, and click "Load Sketch"

## Project Structure

- `README.md` - This overview document
- `src/` - Source code
  - `index.html` - The complete application (HTML, CSS, and JavaScript)
- `docs/` - Additional documentation
  - `prompt-engineering.md` - Analysis of the development process
  - `user-guide.md` - Detailed usage instructions
- `examples/` - Example sketches and use cases

## Technical Details

The application uses:
- HTML5 Canvas for drawing
- Vanilla JavaScript with no external dependencies
- A custom JSON format for representing vector lines
- Browser localStorage for optional sketch persistence

## Learning from This Project

This project provides several valuable learning opportunities:

1. **Vector Drawing Implementation**: Learn how to create a basic drawing application using HTML Canvas
2. **Data Exchange Formats**: Understand how to design lightweight formats for sharing structured data
3. **Prompt Engineering Patterns**: See examples of effective human-AI collaboration
4. **Progressive Enhancement**: Follow how the project evolved from simple concept to refined implementation

## Extending and Adapting

We encourage you to fork, modify, and extend this project! Some ideas:
- Add new drawing tools (shapes, text, etc.)
- Implement undo/redo functionality
- Create additional export formats
- Add collaborative features for multiple users
- Adapt the vector format for other visual communication needs

If you create something interesting based on this project, we'd love to feature it in our [Community Showcase](../../docs/community/showcase.md).

## Development Story

This project began as an exploration in efficient sketch exchange between humans and AI. Initial attempts used base64-encoded JPEG images, but this approach proved unwieldy due to the large data size and transmission issues.

Through collaborative problem-solving, we pivoted to a vector-based approach that represents drawings as collections of lines with coordinates, width, and color. This reduced data size by orders of magnitude and created a more robust exchange format.

For a detailed analysis of the prompt engineering process that led to this project, see [prompt-engineering.md](./docs/prompt-engineering.md).

## License

This project is available under the MIT License. See the [LICENSE](../../LICENSE) file for details.

---

We're excited to see what you create with this tool and what new directions you might take it!