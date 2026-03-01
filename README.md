#  Expense Tracking Web Application
This project is a full-stack web application for expense management, built with Streamlit for the frontend, FastAPI for the backend, and SQL for database management. It allows users to track daily expenses, analyze spending trends, and store and retrieve data efficiently.
-  A **Streamlit frontend** for intuitive user interaction  
-  A **FastAPI backend** for handling API logic and database operations  
-  A **MySQL database** for persistent storage  
-  Logging for debugging and traceability 



## Installation

### 1. Clone the repository:
```
git clone https://github.com/yourusername/expense-tracking-web_application.git

```

### 2. Install dependencies:
```
pip install -r requirements.txt
```

### 3. Start the FastAPI backend server:
```
uvicorn Backend.server:app --reload
```

> 📁 Make sure you're in the `Backend/` folder when running the above command.

### 4. Run the Streamlit frontend:
```
streamlit run Frontend.\app.py
```



## 🚀 Features
- Add/Update Expenses by date  
- View Category-Wise Analytics (with percentage breakdown)  
- View Month-Wise Expense Trends (bar chart + table)  
- REST API Integration with FastAPI  
- MySQL backend for real-time data storage  
- Logging to `server.log` for backend traceability  

## 🔌 API Endpoints

| Method | Endpoint                  | Description                                                     |
|--------|---------------------------|-----------------------------------------------------------------|
| `GET`  | `/expenses/{expense_date}` | Get all expenses for a given date                               |
| `POST` | `/expenses/{expense_date}` | Add expenses for a given date                                   |
| `POST` | `/analytics/`             | Category summary by percentage (bar chart) for given date range |


## Usage
After setting up the application, you can start tracking your expenses. Here’s how to use the key features:

### Adding an Expense
1. Navigate to the "Add Expense" section.
2. Fill in the details such as amount, category, and date.
3. Click "Submit" to save the expense.
## Add/Update Tab Picture
<image src="https://github.com/sangamesh5725/Expense-Tracking-Web-Application/blob/main/Add_Update%20Tab.png">

### Viewing Analytics
1. Go to the "Analytics" tab.
2. View your spending patterns through visualization using bar chart
3. Use filters to refine your data based on categories or dates.
## Analytics Tab Picture
<image src="https://github.com/sangamesh5725/Expense-Tracking-Web-Application/blob/main/Analytics_Tab.png">

### Update Expenses
1. Access the "Update Expenses" section.
2. You can edit or delete any existing expense records.
<image src="https://github.com/sangamesh5725/Expense-Tracking-Web-Application/blob/main/MySql_Database.png">


## 📌 Notes
- Ensure MySQL is running and the `expense_manager` database is created.  
- Update DB credentials in `db_helper.py` if needed.  
- Logs are saved to `Backend/server.log`.

## 🙌 Acknowledgments
### Built using
- streamlit==1.54.0
- FastApi==0.122.0
- pandas==2.3.3
- pytest==9.0.2
- pydantic==2.12.4
- uvicorn==0.41.0
- mysql-connector-python==9.5.0
- requests==2.32.5
- CodeBasics DS AI Bootcamp

## 📧 Contact

For questions or suggestions:  
**Sangamesh Devani** | `sangamesh.devani@gmail.com`

