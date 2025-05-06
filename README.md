# AI29 Chat Assistant

A clean, responsive chatbot interface using Flask and OpenAI's GPT-4o model.

## Features

- 💬 Real-time chat interface with AI responses
- 💾 Message history saved in PostgreSQL database
- 🔄 Conversation persistence between sessions
- ❤️ Custom heart icon branding
- 📱 Responsive design for all devices

## Tech Stack

- **Frontend**: HTML, CSS, JavaScript, Bootstrap
- **Backend**: Flask (Python)
- **Database**: PostgreSQL
- **AI**: OpenAI GPT-4o API

## Setup Instructions

### Prerequisites

- Python 3.9+
- PostgreSQL database
- OpenAI API key

### Environment Variables

Create a `.env` file with the following variables:

```
DATABASE_URL=postgresql://username:password@host:port/database
OPENAI_API_KEY=your_openai_api_key
SESSION_SECRET=your_random_secret_key
```

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/ai29-chat.git
   cd ai29-chat
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Start the application
   ```bash
   gunicorn --bind 0.0.0.0:5000 --reuse-port --reload main:app
   ```

4. Visit `http://localhost:5000` in your web browser

## Usage

- Type your message in the text box and press Enter or click the send button
- The AI will respond with a thoughtful answer
- Your conversation history is saved automatically
- Click "New Chat" to start a fresh conversation

## License

MIT

## Credits

- OpenAI for the GPT-4o model
- Bootstrap for the UI components
- Font Awesome for the icons
