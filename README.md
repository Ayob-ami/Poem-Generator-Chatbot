# AI Poetry Generator

A web-based chatbot that generates creative poems using the Phi-3-mini-4k-instruct model. Built with Python, Transformers, and Gradio.

## Features

- Interactive chat interface for poem generation
- Pre-defined responses for common queries
- Real-time poem generation based on user prompts
- Memory-efficient implementation using HuggingFace pipeline
- Support for custom themes and topics
- Optimized for performance with CUDA acceleration

## Technical Requirements

- Python 3.7+
- PyTorch
- Transformers library
- Gradio
- CUDA-capable GPU (recommended)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd ai-poetry-generator
```

2. Install the required dependencies:
```bash
pip install torch transformers gradio
```

3. Download the model:
The application uses the `microsoft/phi-3-mini-4k-instruct` model, which will be automatically downloaded when you run the application for the first time.

## Usage

1. Start chatting with the AI by:
   - Entering a topic or theme for a poem
   - Using casual greetings like "hi" or "hello"
   - Asking about the creator using "who built this?"

## Features in Detail

### Conversation Handling
- Supports basic greetings and common queries
- Maintains conversation history
- Provides predefined responses for frequently asked questions

### Poetry Generation
- Generates unique poems based on user prompts
- Uses temperature control for creativity
- Supports various poetic styles and themes

### Technical Optimizations
- Uses half-precision (float16) for efficient memory usage
- Automatic device mapping for optimal performance
- Implements efficient token generation with adjustable parameters

## Model Configuration

The application uses the following key parameters:
- Max token length: 500
- Temperature: 0.7
- Device mapping: Automatic (CUDA if available)
- Torch dtype: float16 for optimal performance

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

[MIT]

## Acknowledgments

- Microsoft for the Phi-3-mini-4k-instruct model
- HuggingFace for the Transformers library
- Gradio team for the web interface framework
