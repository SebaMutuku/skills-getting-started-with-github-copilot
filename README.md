# Mergington High School Extracurricular Activities API

This project provides a FastAPI-based web API for managing extracurricular activities at Mergington High School. Students can view available activities and sign up using their email addresses.

## Key Features

- FastAPI endpoints for listing activities and handling sign-ups
- In-memory storage of activities and participants
- Static file serving for the frontend
- Basic error handling for invalid activity requests
- Expanded selection of activities, including:
  - **Sports:** Basketball Team, Gym Class, Soccer Club, Swimming Team, plus more
  - **Artistic:** Drama Club, Art Workshop, plus more
  - **Intellectual:** Chess Club, Programming Class, Debate Team, Math Club, plus more

This implementation provides a simple foundation for further development and integration with persistent storage or authentication systems.

## Getting Started

1. Install dependencies:
   ```
   pip install fastapi uvicorn
   ```
2. Run the application:
   ```
   uvicorn src.app:app --reload
   ```
3. Access the API and static frontend at [http://localhost:8000](http://localhost:8000).

## Endpoints

- `GET /activities` — List all available activities
- `POST /activities/{activity_name}/signup?email=your_email` — Sign up for an activity

## Customization

You can easily add or modify activities in the `src/app.py` file under the `activities` dictionary.
