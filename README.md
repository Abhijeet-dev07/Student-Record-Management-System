# Student-Record-Management-System
# Student Record Management System

## Description
A comprehensive student management system with both web and CLI interfaces. The web version uses Flask with Firebase integration, while the CLI version stores data locally. Provides full CRUD (Create, Read, Update, Delete) operations for managing student records.

## Features
- **Web Interface**:
  - Add new students
  - Update existing records
  - Delete student records
  - Search for individual students
  - View all students
  - Firebase database integration

- **CLI Interface**:
  - Add/Update/Delete students
  - Search and view records
  - Simple text-based interface
  - Local data storage

## Technologies Used
- Python 3.x
- Flask (Web Framework)
- Firebase Firestore (Database)
- HTML/CSS/JavaScript (Frontend)
- Tailwind CSS (Styling)

## File Structure
```
.
├── app.py            # Flask backend with Firebase integration
├── main.py            # CLI interface with local storage
├── templates/
│   └── index.html    # Web interface
└── README.md          # Project documentation
```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/student-management-system.git
   cd student-management-system
   ```

2. Install dependencies:
   ```bash
   pip install flask firebase-admin
   ```

3. Set up Firebase:
   - Create a Firebase project
   - Download serviceAccountKey.json
   - Place it in the project root

4. Run the application:
   ```bash
   python app.py
   ```

## Usage
### Web Interface
1. Access the web interface at `http://localhost:5000`
2. Use the form to add new students
3. Use API endpoints for other operations:
   - Add: POST /add_student
   - Update: PUT /update_student
   - Delete: DELETE /delete_student/<id>
   - Search: GET /search_student/<id>
   - View All: GET /view_students

### CLI Interface
1. Run the CLI:
   ```bash
   python main.py
   ```
2. Follow the menu prompts to:
   - Add/Update/Delete students
   - Search and view records
   - Exit the program

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
