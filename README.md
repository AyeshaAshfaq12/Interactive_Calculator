# Interactive Calculator

**Interactive Calculator** is an innovative web application that enables users to draw complex equations, problems, or diagrams on a canvas and receive real-time solutions using the power of AI. This project leverages ReactJS and Tailwind CSS on the frontend and Python for backend processing, with integration of Gemini AI for deep analysis and solution generation.

## Features

- **Hand-drawn Problem Recognition**: Users can draw equations or diagrams, and the AI will interpret the content.
- **AI-powered Solutions**: Utilizes Gemini AI to process and solve complex math problems, diagrams, and equations.
- **Responsive & Modern UI**: Built with ReactJS and Tailwind CSS, offering an intuitive and responsive interface.
- **Optimized Request Processing**: A well-structured file system in the backend ensures efficient handling of multiple requests with reduced load on each request cycle.

## Tech Stack

- **Frontend**: [ReactJS](https://reactjs.org/), [Tailwind CSS](https://tailwindcss.com/)
- **Backend**: Python, [Gemini AI Integration](https://www.gemini.com/)
- **Other Tools**: Canvas for user-drawn input

## Table of Contents

- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Best Practices](#best-practices)
- [Contributing](#contributing)
- [License](#license)

---

## Getting Started

These instructions will help you set up and run the project on your local machine for development and testing purposes.

### Prerequisites

- **Node.js** (v14 or higher)
- **Python** (v3.8 or higher)
- [Gemini AI API Key](https://www.gemini.com/) (required for backend integration)

### Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/interactive-calculator.git
cd interactive-calculator
```

#### 2. Frontend Setup
Navigate to the `frontend` directory and install dependencies.

```bash
cd frontend
npm install
```

#### 3. Backend Setup
Navigate to the `backend` directory, set up a virtual environment, and install dependencies.

```bash
cd backend
python -m venv venv
source venv/bin/activate  # For Windows use `venv\Scripts\activate`
pip install -r requirements.txt
```
Add your Gemini API key to the environment file:
```bash
echo "GEMINI_API_KEY=your_api_key_here" > .env
```

#### 4. Run the Application
**Frontend**: In the frontend directory, start the React app.
```bash
npm start
```
**Backend**: In the backend directory, run the Python server.
```bash
python app.py
```
The application should now be running at `http://localhost:3000` with the backend server handling requests.


## Usage

1. Draw your equation, problem, or diagram on the canvas.
2. Submit the drawing, and the AI backend will analyze it using Gemini AI.
3. Receive the solution or suggested answer directly on the screen.


## Project Structure
The project is divided into two main directories: `frontend` and `backend`.

```graphql
interactive-calculator/
├── frontend/           # ReactJS + Tailwind CSS frontend
│   ├── public/
│   └── src/
│       ├── components/ # Reusable UI components
│       ├── hooks/      # Custom hooks for state management
│       └── utils/      # Helper functions and utilities
│
└── backend/            # Python backend
    ├── api/            # API routes and controllers
    ├── models/         # Data models and Gemini AI integration
    └── utils/          # Helper functions
```
This structure maintains modularity and reduces the load on each request cycle, ensuring a scalable, efficient architecture.


## Best Practices
- **Code Consistency**: Consistent code style throughout frontend and backend files.
- **Optimized File Structure**: Maintains separation of concerns for clear readability and maintainability.
- **Error Handling**: Comprehensive error handling for seamless user experience.
- **Security**: Sensitive information like the Gemini API key is stored in environment variables.

  
## Contributing
We welcome contributions! Please follow these steps:
1. Fork the repository.
2. Create your branch: `git checkout -b feature/YourFeature`.
3. Commit your changes: `git commit -am 'Add new feature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Open a Pull Request.

## Contact
For questions or support, please contact `Ayesha Ashfaq`.




