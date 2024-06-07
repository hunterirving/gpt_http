# GPT_HTTP (ChatGPT for Vintage Web Browsers)

This is a simple Flask-based web application that allows users to interact with OpenAI's GPT models through a web interface.
This application is designed to be compatible with vintage machines, including early Macintoshes, by ensuring responses are formatted with HTML tags and ASCII characters suitable for older systems.

![ChatGPT client running on a vintage Macintosh Plus](readme_images/macintosh_plus.jpg)

![ChatGPT client running on Windows XP](readme_images/windows_xp.jpg)


## Setup Instructions

### Prerequisites

- Python 3.x
- OpenAI API key

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/gpt_http.git
   cd gpt_http
   ```

2. Set up the virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

4. Configure your OpenAI API key:

   - Create a `config.py` file in the root of the project directory.
   - Add your OpenAI API key to `config.py`:

     ```python
     open_ai_api_key = "your_openai_api_key"
     ```

5. Run the Flask application:

   ```bash
   python3 gpt_http.py
   ```

6. Access the application:

Open a web browser on your vintage machine and navigate to ```http://<ip_address_of_flask_server>:8080```,

Note: Replace <ip_address_of_flask_server> with the actual IP address of the machine running the Flask server. Ensure both machines are connected to the same Wi-Fi network.

### .gitignore

Ensure your `.gitignore` file includes the following entries to avoid committing sensitive information and virtual environment files:

```
config.py
venv/
```

### Deactivating the Virtual Environment

When you're done working with this project, deactivate the virtual environment with:

```bash
deactivate
```

## Contributing

Feel free to submit issues or pull requests for improvements and bug fixes.