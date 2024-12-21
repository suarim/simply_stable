# Stable Diffusion Image Generator

## Overview
This project provides a web-based application to generate high-quality images from textual descriptions using the Stable Diffusion model. The app is built using the following:

- **Stable Diffusion** for text-to-image generation.
- **Gradio** for creating a user-friendly interface.
- **PyTorch** for leveraging GPU acceleration.

## Features
- Generate stunning, high-quality images from text prompts.
- User-friendly web interface for ease of use.
- GPU-accelerated for fast image generation.

## Setup Instructions

### Prerequisites
Make sure you have the following installed:
- Python 3.8 or higher
- GPU with CUDA support (optional but recommended for faster generation)

### Installation
1. Clone the repository:
    ```bash
    git clone <repository_url>
    cd <repository_folder>
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Download the Stable Diffusion model:
    - The code will automatically fetch the model using the `from_pretrained` method from the `diffusers` library.

### Running the Application
1. Launch the application:
    ```bash
    python app.py
    ```

2. Open the Gradio interface in your browser:
    - By default, it will be hosted locally at `http://127.0.0.1:7860`.

3. Enter a text prompt in the input box and click "Submit" to generate an image.

## File Structure
```
.
|-- app.py                # Main application script
|-- requirements.txt      # List of Python dependencies
|-- README.md             # Project documentation
```

## Example Usage
1. Start the app:
    ```bash
    python app.py
    ```

2. Open the interface and enter a prompt like:
    ```
    "A futuristic cityscape at sunset with flying cars."
    ```

3. View the generated image in the web interface.

## Dependencies
- `diffusers`
- `gradio`
- `torch`
- `transformers`

Install all dependencies using:
```bash
pip install -r requirements.txt
```

## Known Issues
- **Insufficient GPU Memory**: Generating high-resolution images may fail if your GPU does not have enough VRAM. Use a lower precision or a smaller model variant.
- **Model Download Issues**: Ensure you have an internet connection during the first run to download the model.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- [Hugging Face](https://huggingface.co/) for the `diffusers` library and pre-trained Stable Diffusion model.
- [Gradio](https://gradio.app/) for the interactive UI framework.

## Contact
For any questions or suggestions, please reach out to [Your Name] at [Your Email].
