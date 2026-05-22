<h6>PhishGuard: Smart Phishing URL Detection System</h6>
PhishGuard is a cybersecurity SaaS prototype for detecting phishing URLs using advanced AI models and heuristic rules.

Tech Stack
Frontend: Next.js (App Router), TypeScript, Tailwind CSS, shadcn/ui, Zustand, React Query
Backend: FastAPI, Python 3.12+, Uvicorn, Pydantic
Database/Auth: Supabase (PostgreSQL)
Setup Instructions
Prerequisites
Node.js (v18+)
Python (3.12+)
Frontend Setup
Navigate to the frontend directory:
cd frontend
Install dependencies:
npm install
Set up environment variables:
cp .env.local.example .env.local
Fill in your Supabase credentials in .env.local.
Run the development server:
npm run dev
Backend Setup
Navigate to the backend directory:
cd backend
Create and activate a virtual environment:
python -m venv venv
# Windows:
.\venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
Install dependencies:
pip install -r requirements.txt
Set up environment variables:
cp .env.example .env
Fill in your Supabase and Postgres credentials in .env.
Run the FastAPI development server:
python run.py
The API will be available at http://localhost:8000. Documentation is available at http://localhost:8000/api/v1/docs (Swagger UI) or /redoc.
Manual Setup Remaining
Set up a Supabase project and obtain your URL and Anon Key / Service Role Key.
Configure Supabase authentication.
Update the .env.local and .env files with your actual credentials.
Future Roadmap
Integration of actual ML models for threat detection.
Heuristic rule engine setup.
Advanced reporting and export functionality.
