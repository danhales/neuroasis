# Vector Drawing Exchange: User Guide

This guide provides detailed instructions for using the Vector Drawing Exchange application to create and share sketches with AI assistants like Claude.

## Getting Started

### Basic Setup

1. **Open the application**:
   - If you downloaded the HTML file, simply open it in any modern web browser
   - No installation or server setup is required

2. **Understand the interface**:
   - **Drawing Canvas**: The large white area where you'll create your sketches
   - **Drawing Tools Tab**: Tools for creating and modifying your sketch
   - **Exchange Tab**: Tools for importing and exporting sketch data

### Drawing Controls

The application offers several tools for creating your sketches:

- **Color Selection**: Choose from black, red, blue, green, or purple for your lines
- **Line Width**: Select thin, medium, or thick line widths
- **Clear Canvas**: Erase everything and start over

## Creating a Sketch

1. **Select your drawing tools**:
   - Click on a color to select it
   - Click on a line width to select it

2. **Draw on the canvas**:
   - Click and drag to draw lines
   - Release to end a line segment
   - Each line is stored individually in the vector format

3. **Modify your drawing**:
   - Use different colors and line widths to add variety
   - Use the Clear Canvas button to start over if needed

## Sharing Your Sketch with Claude

1. **Generate sketch data**:
   - Click the "Exchange" tab
   - Click the "Generate Sketch Data" button
   - The application will convert your drawing into a compact text format

2. **Copy the sketch data**:
   - Click the "Copy to Clipboard" button, or
   - Manually select all text in the export text area and copy (Ctrl+C or Cmd+C)

3. **Paste into your conversation with Claude**:
   - Go to your conversation with Claude
   - Paste the sketch data (Ctrl+V or Cmd+V)
   - Send the message

## Viewing Claude's Sketches

1. **Copy Claude's sketch data**:
   - When Claude sends sketch data (formatted as `[SKETCH-DATA]...[/SKETCH-DATA]`), select and copy it

2. **Import the sketch data**:
   - In the application, go to the "Exchange" tab
   - Paste the data into the import text area
   - Click the "Load Sketch" button

3. **View and modify**:
   - The application will render Claude's sketch on the canvas
   - You can now add to it, modify it, or use it as a reference for your own drawing

## Understanding the Sketch Data Format

The Vector Drawing Exchange uses a simple, text-based format to represent sketches:

[SKETCH-DATA][{"x1":100,"y1":100,"x2":200,"y2":150,"width":5,"color":"black"},...][/SKETCH-DATA]

This format consists of:
1. A start tag: `[SKETCH-DATA]`
2. A JSON array of line objects, each with:
   - Starting coordinates (x1, y1)
   - Ending coordinates (x2, y2)
   - Line width in pixels
   - Line color
3. An end tag: `[/SKETCH-DATA]`

This approach creates a compact, readable format that can be easily shared in text-based conversations.

## Tips for Effective Sketch Exchange

- **Keep sketches simple**: Simpler sketches translate better to the vector format
- **Use color purposefully**: Different colors can help distinguish parts of your sketch
- **Build incrementally**: Create a basic sketch, share it, then add to Claude's response
- **Try different line widths**: Varying line widths can add emphasis and clarity
- **Label important elements**: Add simple text or indicators if parts of your sketch need explanation

## Troubleshooting

### Import Issues

- **"Invalid sketch data format" error**: Make sure you've copied the entire sketch data, including the `[SKETCH-DATA]` and `[/SKETCH-DATA]` tags
- **"Error parsing JSON" error**: The sketch data may be corrupted or incomplete. Try copying again.

### Export Issues

- **Nothing happens when clicking "Generate Sketch Data"**: Make sure you've drawn something on the canvas first
- **Clipboard permissions error**: Some browsers restrict clipboard access. Try manually selecting and copying the text.

### Drawing Issues

- **Lines appear in wrong positions**: Make sure you're not zoomed in or out in your browser (use Ctrl+0 or Cmd+0 to reset zoom)
- **Drawing feels laggy**: Complex drawings with many lines may cause performance issues on some devices

## Next Steps

Once you're comfortable with basic sketch exchange, try these advanced techniques:

- **Iterative sketching**: Build on each other's ideas through multiple exchanges
- **Annotation**: Use different colors to annotate or highlight parts of a sketch
- **Mixed media**: Combine sketches with text descriptions for clearer communication
- **Template creation**: Create reusable templates for common discussion topics

---

We hope this guide helps you get the most out of the Vector Drawing Exchange application! If you discover interesting techniques or uses, consider sharing them with the community.