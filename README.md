# ollama-chat-ui-html
Don't want to use the heavy chat ui, but just want a simple to setup and run chat UI for chatting with your local ollama? Then this is for you!

# Ollama Chat Interface

A modern, responsive web interface for interacting with Ollama language models. Built with Vue.js and Bootstrap.


## Features

- 💾 Persistent chat history using IndexedDB
- ✨ Real-time streaming responses
- 📝 Markdown support with syntax highlighting
- 🔧 Configurable model parameters
- 🔄 Multiple chat sessions
- 🌐 Configurable server address
- 🎨 Clean and intuitive UI

## Quick Start

1. Make sure you have [Ollama](https://ollama.ai) installed and running on your system
2. Download the `index.html` file
3. Serve `index.html` in a modern web browser. Easiest way is to run <code>npx http-server</code>
4. Start chatting with your Ollama models!

## Configuration Options

### Server Settings
- **Server Address**: Configure the Ollama server address (default: `http://127.0.0.1:11434`)

### Model Parameters
- **Model Selection**: Choose from available installed models
- **Temperature**: Adjust response randomness (0-2)
- **Context Length**: Set the context window size
- **Top P**: Control response diversity
- **Top K**: Limit vocabulary choices

## Features in Detail

### Chat Management
- Create new chat sessions
- Delete existing chats
- Automatic chat title generation from first message
- Real-time chat persistence

### Message Display
- Markdown rendering
- Code syntax highlighting
- Special formatting for model's thinking process
- Smooth animations and transitions
- Auto-scroll to latest messages

### User Interface
- Sidebar with chat history
- Settings modal for configuration
- Responsive design for all screen sizes
- Loading indicators
- Error handling and notifications

## Technical Details

### Built With
- Vue.js 3
- Bootstrap 5
- Marked (for Markdown parsing)
- IndexedDB (for data persistence)

### Browser Support
Requires a modern browser with support for:
- ES6+ JavaScript
- IndexedDB
- Fetch API
- CSS Grid/Flexbox

## Development

To modify the interface:

1. Clone the repository
2. Edit the `index.html` file
3. Test with a local Ollama instance

The entire application is contained in a single HTML file for easy deployment and modification.

## Troubleshooting

### Common Issues

1. **Can't Connect to Ollama**
   - Ensure Ollama is running
   - Check the server address in settings
   - Verify no CORS issues

2. **Messages Not Saving**
   - Check browser IndexedDB support
   - Clear browser data if database is corrupted

3. **Models Not Loading**
   - Verify Ollama has models installed
   - Check network connectivity
   - Confirm server address is correct

## Contributing

Feel free to:
- Submit bug reports
- Propose new features
- Create pull requests

## Acknowledgments

- [Ollama](https://ollama.ai) for the amazing local LLM runtime
- Vue.js team for the reactive framework
- Bootstrap team for the UI components
- Cursor for helping me build this quick
