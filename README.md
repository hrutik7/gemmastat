demo : https://drive.google.com/file/d/1fhGkG_xGT6PIDmi06OCLpS0yO_UVgxQ8/view?usp=sharing

live url : https://app.salusgemmalabs.com

landig page :   https://www.salusgemmalabs.com

dummy credentials : 

email : string@string.com

password : string

*note : if dummy credentials does not work just click twice first time its facing issue sometimes .


# GemmaStat

GemmaStat is a sophisticated data analytics platform that combines PostgreSQL database and excel  integration with AI-powered analysis capabilities. It provides intuitive data visualization, statistical analysis, and interactive exploration features.


## Tech Stack

- **Frontend**: React, Tailwind CSS, Framer Motion 
- **Backend**: FastAPI, SQLAlchemy, PostgreSQL
- **AI/ML**: llama-3.3-70b
- **Authentication**: JWT-based auth system

## Getting Started

### Prerequisites

Before you begin, ensure you have:
- Python 3.8+ installed
- Node.js 16+ installed
- PostgreSQL database
- Environment variables set up in a `.env` file

### Quick Start (Run Both Frontend & Backend)

1. **Clone the repository:**
    ```bash
    git clone https://github.com/hrutik7/physisyncstat.git
    cd physisyncstat
    ```

2. **Run the start script:**
    ```bash
    ./start.sh
    ```
    This will:
    - Set up Python virtual environment if needed
    - Install all dependencies (both frontend and backend)
    - Start both frontend and backend servers

    The frontend will be available at `http://localhost:5173`
    The backend will be available at `http://localhost:8000`

### Manual Setup (If you prefer separate setup)

2. **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate
    ```

3. **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables:**
    - Copy `.env.example` to `.env`
    - Fill in your environment variables
    - Install python-dotenv: `pip install python-dotenv`

## Running the Application

### Development Mode

To run the application in development mode with auto-reloading:

```bash
uvicorn app.main:app --reload
```

### Production Mode

To run the application in production mode using Gunicorn:

```bash
gunicorn -k uvicorn.workers.UvicornWorker app.main:app --bind 0.0.0.0:8000
```

## Project Structure

```
data-analytics-backend/
├── app/
│   ├── __init__.py
│   ├── main.py             # Main FastAPI application
│   └── ...                 # Other modules (e.g., routers, services, models)
├── venv/                   # Python virtual environment
├── .env                    # Environment variables (do not commit)
├── .env.example           # Example environment variables
├── .gitignore
├── README.md              # This file
├── requirements.txt       # Project dependencies
└── ...
```



## This project bnuild in AiBoomi startup weekend

