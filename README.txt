Travdoodle - Travel Itinerary Organizer  
=======================================  

Student Details  
---------------  
- Name: Felicia Nkatha  
- Registration Number: E23S/13640/2021  
- Supervisor: Dr Eric Araka  
- Academic Year: 2024/2025  

Project Title  
-------------  
Travdoodle - A Travel Itinerary Organizer  

Project Overview  
----------------  
Travdoodle is a full-stack web application designed to help users seamlessly plan and manage their travel itineraries. The system allows users to create, modify, and organize trip details, including destinations, accommodations, activities, and packing lists.  

Main Features  
-------------  
- User Authentication: Signup, Login, Logout, and Session Management  
- Trip Management: Create, edit, and delete itineraries  
- Destination Planning: Add destinations, accommodations, and activities  
- Packing List Management: Create and update packing lists  
- Responsive UI: Mobile-friendly design  
- RESTful API: Backend handles secure data management  
- Deployment: Frontend on Netlify, Backend on Render  

Live Links  
----------  
- Frontend: Travdoodle on Netlify (https://travdoodle.netlify.app/)  
- Backend API: Travdoodle API on Render (https://travdoodle-api.onrender.com/)

GitHub Repositories:
- Frontend: (https://github.com/ki-rigi/travdoodle-frontend)
- Backend: (https://github.com/ki-rigi/travdoodle-backend)


Tech Stack  
----------  

Frontend (Client-Side)  
- Framework: React  
- Routing: React Router  
- State Management: Zustand  
- Styling: Default CSS Modules  
- Form Handling & Validation: Formik & Yup  
- API Communication: Fetch API  
- Development Tools: Vite, ESLint  
- Deployment: Netlify  

Backend (Server-Side)  
- Framework: Flask, Flask-RESTful  
- Database: PostgreSQL (Managed via SQLAlchemy ORM)  
- Authentication: Flask sessions  
- Environment Variables: Dotenv  
- Database Migrations: Flask-Migrate  
- Deployment: Render  

Project Folder Structure  
------------------------  
Travdoodle/  
├── README.txt  
├── travdoodle-backend  
│   ├── app.py  
│   ├── instance  
│   ├── migrations  
│   ├── model.py  
│   ├── Pipfile  
│   ├── Pipfile.lock  
│   ├── README.txt  
│   ├── requirements.txt  
│   └── seed.py  
└── travdoodle-frontend  
    ├── eslint.config.js  
    ├── index.html  
    ├── node_modules  
    ├── package.json  
    ├── package-lock.json  
    ├── public  
    ├── README.txt  
    ├── src  
    └── vite.config.js  

Installation Guide  
------------------  

Prerequisites  
- Node.js & npm  
- Python 3.x  
- PostgreSQL  
- Git  

Frontend Setup  
--------------  

Steps to Install & Run the Frontend  
1. Navigate to the frontend folder:   
   cd travdoodle-frontend  
2. Install dependencies:  
   npm install  
3. Start the development server:  
   npm run dev  

Backend Setup  
-------------  

Steps to Install & Run the Backend  
1. Navigate to the backend folder:  
   cd travdoodle-backend  
2. Create a virtual environment and install dependencies:  
   pipenv install  
3. Set up the environment variables in a `.env` file:  
   DATABASE_URI=your_postgresql_database_url  
   SECRET_KEY=your_secret_key  
   FLASK_APP=app.py  
4. Apply database migrations:  
   flask db upgrade  
5. Seed the database (optional but recommended):  
   python seed.py  
6. Start the backend server:  
   python app.py  

Deployment Guide  
----------------  

Frontend Deployment (Netlify)  
1. Push your frontend repository to GitHub.  
2. Create a new project on Netlify and connect it to your GitHub repository.  
3. Configure build settings:  
   - Build command: npm run build  
   - Publish directory: dist  
4. Deploy the site.  

Backend Deployment (Render)  
1. Push your backend repository to GitHub.  
2. Create a new service on Render, linking your GitHub repository.  
3. Add environment variables in Settings.  
4. Deploy the service.  

API Endpoints  
-------------  

Authentication  
| Endpoint        | Method  | Description       |  
|---------------|--------|------------------|  
| /login       | POST   | User login       |  
| /logout      | DELETE | User logout      |  
| /check_session | GET   | Check session    |  

Users  
| Endpoint       | Method  | Description          |  
|-------------- |--------|----------------------|  
| /users       | GET    | List all users      |  
| /users       | POST   | Create a new user   |  
| /users/<id>  | GET    | Get user details    |  
| /users/<id>  | PATCH  | Update user details |  
| /users/<id>  | DELETE | Delete a user       |  

(More detailed API documentation can be found in the backend README.)  

Testing  
-------  

Frontend Testing  
- Run the development server and manually test features.  
- Check for linting errors:  
  npm run lint  

Backend Testing  
- Use Postman or cURL to test API endpoints.  


License  
-------  

This project is licensed under the MIT License.  

---