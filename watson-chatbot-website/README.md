# IBM Watson-Powered Chatbot Website

A modern, responsive static website integrated with IBM Watson Assistant chatbot. This project demonstrates how to embed an AI-powered conversational interface into a web application.

## Features

- **IBM Watson Assistant Integration**: Live AI chatbot powered by IBM Watson
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Docker Support**: Easy containerization and deployment
- **Nginx Optimized**: Production-ready web server configuration

## Quick Start

### Prerequisites

- Modern web browser
- Node.js (for local development server)
- Docker (for containerized deployment)

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/watson-chatbot-website.git
cd watson-chatbot-website
```

2. Start a local server:
```bash
npx serve -p 3000
```

3. Open http://localhost:3000 in your browser

### Docker Deployment

1. Build and run with Docker Compose:
```bash
docker-compose up -d
```

2. Access the website at http://localhost:8080

Or build manually:
```bash
docker build -t watson-chatbot-website .
docker run -d -p 8080:80 watson-chatbot-website
```

## Watson Assistant Configuration

The chatbot is configured with the following IBM Watson Assistant credentials:
- **Integration ID**: 6f368a2b-ca5a-460d-be1a-12025e268bb5
- **Region**: au-syd
- **Service Instance ID**: 5991963c-9729-4f4a-831a-281a1fd73ece

To use your own Watson Assistant:
1. Create an IBM Cloud account at https://cloud.ibm.com
2. Create a Watson Assistant service
3. Build your assistant with intents, entities, and dialog
4. Get the web chat embed code
5. Replace the credentials in `index.html`

## Project Structure

```
watson-chatbot-website/
├── index.html          # Main HTML file with Watson integration
├── css/
│   └── style.css       # Responsive styles
├── js/
│   └── main.js         # Interactive features
├── images/             # Image assets
├── Dockerfile          # Container configuration
├── nginx.conf          # Web server configuration
├── docker-compose.yml  # Docker Compose setup
└── README.md           # Documentation
```

## Docker Hub

Pre-built images available:
- `riteshlingwal/watson-chatbot-website:latest`
- `tejasvapc2215/watson-chatbot-website:latest`

Pull and run:
```bash
docker pull riteshlingwal/watson-chatbot-website:latest
docker run -d -p 8080:80 riteshlingwal/watson-chatbot-website:latest
```

## Technologies Used

- HTML5 & CSS3
- JavaScript (ES6+)
- IBM Watson Assistant
- Nginx Alpine
- Docker

## License

MIT License - feel free to use for your projects!

## Author

Created as part of PBEL (Project Based Experiential Learning)
