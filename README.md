# HireDriver-Database-System  

## Overview  
**HireDriver-Database-System** is a centralized database solution built to enhance the operational efficiency of **Hire Driver Co. Ltd**, a recruitment agency specializing in providing safe and reliable drivers to a diverse range of customers. This system centralizes records for drivers, clients, training sessions, and hires, ensuring seamless operations and strategic decision-making across the company’s departments.  

## Purpose  
This project aims to:  
- Provide an efficient driver-client pairing system based on customer specifications and driver qualifications.  
- Centralize data to streamline operations for Human Resources, Management, Finance, Marketing, and Hire Control teams.  
- Facilitate training assignment and monitoring.  
- Ensure compliance with hiring contracts and terms.  

## Features  
- **Driver Records Management**: Store driver profiles, licensing details, vehicle associations, and hiring history.  
- **Client Management**: Maintain customer profiles, preferences, and hiring history.  
- **Training Sessions**: Assign and monitor training sessions for drivers based on their qualifications.  
- **Hire Tracking**: Monitor compliance with hire terms and the hiring status of all drivers.  
- **Data Insights**: Analyze hiring trends and identify high-value customers to optimize marketing and profitability strategies.  

## Technologies  
- **Frontend**: HTML, CSS  
- **Backend**: Python  
- **Database**: MySQL  
- **Version Control**: Git  

## Installation  

### Prerequisites  
- Python 3.x installed  
- MySQL installed and running  
- Git installed  

### Steps  
1. Clone the repository:  
   ```bash
   git clone https://github.com/jochyybasil/HireDrive-Database-System.git
   cd DriveHub-Database-System
   ```  

2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  

3. Set up the database:  
   - Create a MySQL database (e.g., `hire_driver_db`).  
   - Configure database credentials in the `.env` or `settings.py` file.  

4. Import the database schema:  
   - Run the SQL file provided in the `database/` folder:  
     ```sql
     mysql -u username -p hire_driver_db < database/schema.sql
     ```  

5. Run the application:  
   ```bash
   python main.py   
   ```  

6. Access the system:  
   - Open your browser and navigate to `http://localhost:5000` (default Flask server) or `http://localhost:8000` (Django server).  

## Folder Structure  
```
DriveHub-Database-System/  
├── backend/  
│   ├── models/            # Database models  
│   ├── templates/         # HTML templates rendered by the backend  
│   ├── static/            # CSS and other static files  
│   └── views/             # Backend logic (Python)  
├── database/              # Database schema and scripts  
├── docs/                  # Documentation  
├── .env                   # Environment variables  
├── requirements.txt       # Python dependencies  
└── README.md              # Project overview  
```  

## Usage  
- Access the **frontend interface** rendered directly by the Python backend to manage drivers, customers, and hires.  
- Use the system to track training sessions, hire contracts, and compliance directly through an intuitive web interface.  
- Analyze trends via built-in views tailored for specific teams (e.g., HR, Marketing).  

## Contributing  
Contributions are welcome! Please follow these steps:  
1. Fork the repository.  
2. Create a new branch: `git checkout -b feature-name`.  
3. Commit your changes: `git commit -m "Add feature description"`.  
4. Push to the branch: `git push origin feature-name`.  
5. Open a pull request.  

## License  
This project is licensed under the [Ashesi License].  

## Contact  
For any inquiries or issues, please contact:  
- **Your Name**: [jochybasil@gmail.com](mailto:jochybasil@gmail.com)  
- **GitHub**: [https://github.com/jochyybasil](https://github.com/jochyybasil)  
