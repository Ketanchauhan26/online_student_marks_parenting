# Online Student Marks Parent SMS Alerting System

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction
The Online Student Marks Parent SMS Alerting System is a web-based application that allows schools to manage and communicate student marks to parents via SMS alerts. This system ensures that parents are promptly informed about their child's academic performance.

## Features
- Admin panel for managing students, subjects, and marks
- Automatic SMS alerts to parents for each student's marks
- Secure login for admins and teachers
- Detailed reports on student performance
- Easy-to-use interface

## Technologies Used
- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask)
- **Database**: SQLite (default), can be configured to use other databases like PostgreSQL or MySQL
- **SMS Gateway**: Twilio API

## Installation
1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/online-student-marks-parent-sms-alerting-system.git
    cd online-student-marks-parent-sms-alerting-system
    ```

2. **Create a virtual environment and activate it:**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

4. **Set up the database:**
    ```sh
    python manage.py migrate
    ```

## Configuration
1. **Twilio Setup:**
   - Create an account on [Twilio](https://www.twilio.com/).
   - Get your Account SID, Auth Token, and a Twilio phone number.

2. **Environment Variables:**
   - Create a `.env` file in the root directory and add the following:
     ```plaintext
     SECRET_KEY=your_secret_key
     DEBUG=True
     TWILIO_ACCOUNT_SID=AC191b8e32bc31f78d18bf56bfe1a5ee9f
     TWILIO_AUTH_TOKEN=234e54d4ec23cbab0efc4c6938a68ddb
     TWILIO_PHONE_NUMBER=+18723279783
     ```

3. **Django Settings:**
   - Ensure that your `settings.py` file is configured to read from the `.env` file for the secret key and other sensitive information.

## Usage
1. **Run the application:**
    ```sh
    python manage.py runserver
    ```

2. **Access the application:**
   Open your web browser and go to `http://127.0.0.1:8000`.

3. **Admin Login:**
   - Use the default admin credentials or create a new admin account through the admin panel.

4. **Manage Students and Marks:**
   - Add students, subjects, and their marks through the admin interface.
   - The system will automatically send SMS alerts to the registered phone numbers of parents.

## Contributing
We welcome contributions to the Online Student Marks Parent SMS Alerting System. To contribute, follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add new feature'`)
5. Push to the branch (`git push origin feature-branch`)
6. Create a new Pull Request

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact
If you have any questions or suggestions, please feel free to contact us at [ankitraj14052003@example.com].

---

Thank you for using the Online Student Marks Parent SMS Alerting System!
