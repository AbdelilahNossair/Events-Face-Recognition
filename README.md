# Face Recognition Event Management System

## Overview

The **Face Recognition Event Management System** is designed to streamline event attendee management using advanced facial recognition technology. This system enables seamless check-in processes, attendee tracking, and post-event engagement by leveraging AI-driven face recognition, real-time processing, and automated email distribution of event photos.

## Features

- **Face Recognition Check-In:**  
  Attendees can register and check in using facial recognition for a contactless and efficient experience.

- **Event Photo Distribution:**  
  Automatically capture and send event photos to attendees via email.

- **Attendee Management:**  
  Maintain a comprehensive database of registered attendees for effective event tracking and management.

- **Real-Time Processing:**  
  Instant processing and verification of attendees during check-in.

- **Admin Dashboard:**  
  A user-friendly interface for event organizers to manage attendees, monitor face recognition accuracy, and track event analytics.

## Workflow

1. **Registration**
   - Attendees pre-register by providing their information and uploading a photo for facial recognition.

2. **Event Check-In**
   - Upon arrival, attendees are identified and checked in using facial recognition technology.

3. **Photo Distribution**
   - Photos captured during the event are automatically linked to attendees and emailed to them after the event concludes.

## Installation

### Prerequisites

Ensure you have the following installed on your system:

- Python 3.8+
- Node.js
- PostgreSQL (or your preferred database)
- Email Server (e.g., SMTP)
- Face Recognition Libraries: OpenCV, dlib

### Steps

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/face-recognition-event.git
    cd face-recognition-event
    ```

2. **Install Backend Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

3. **Install Frontend Dependencies**

    ```bash
    npm install
    ```

4. **Database Setup**
   - Create a PostgreSQL database.
   - Update the database configuration in the `.env` file (see below).
   - Run the migration script to set up the database schema:

    ```bash
    python manage.py migrate
    ```

5. **Environment Configuration**
   - Create a `.env` file in the root directory with the following variables:

    ```env
    DATABASE_URL=postgres://username:password@localhost:5432/yourdatabase
    EMAIL_HOST=smtp.your-email-provider.com
    EMAIL_PORT=587
    EMAIL_USER=your_email@example.com
    EMAIL_PASSWORD=your_email_password
    SECRET_KEY=your_django_secret_key
    DEBUG=True
    ```

6. **Run the Application**
   - **Start the Backend Server**

    ```bash
    python manage.py runserver
    ```

   - **Start the Frontend Development Server**

    ```bash
    npm start
    ```

7. **Access the Application**
   - Open your browser and navigate to [http://localhost:3000](http://localhost:3000) to access the frontend.
   - Access the admin dashboard at [http://localhost:8000/admin](http://localhost:8000/admin).

## Usage

- **For Event Organizers:**
  - Use the admin dashboard to manage attendee registrations, monitor check-ins, and view event analytics.

- **For Attendees:**
  - Register prior to the event by providing necessary details and a clear photo for facial recognition.
  - Check in at the event using facial recognition for a smooth and fast entry.
  - Receive event photos via email after the event concludes.

## Technology Stack

- **Backend:** Node.js / Flask (Python)
- **Frontend:** Flutter (Dart)
- **Database:** Supabase (PostgreSQL )
- **Face Recognition:** face-recognition
- **Email Service:** nodemailer

## Future Enhancements

- **Social Media Integration:**  
  Allow attendees to share their event photos directly to social media platforms.

- **Mobile Application:**  
  Develop a mobile app for on-the-go event management and attendee interaction.

- **Real-Time Notifications:**  
  Implement push notifications for attendees regarding event updates.

- **Advanced Analytics Dashboard:**  
  Enhance the admin dashboard with more detailed analytics and reporting features.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. **Fork the Repository**  
   Click the “Fork” button at the top-right corner of the repository page.

2. **Create a New Branch**

    ```bash
    git checkout -b feature/your-feature-name
    ```

3. **Make Your Changes**  
   Commit your changes with descriptive messages:

    ```bash
    git commit -m "Add some feature"
    ```

4. **Push to the Branch**

    ```bash
    git push origin feature/your-feature-name
    ```

5. **Open a Pull Request**  
   Navigate to the repository on GitHub and click “Compare & pull request” to submit your changes for review.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this software as per the terms of the license.

## Acknowledgments

- Inspired by the latest advancements in AI and facial recognition technologies.
- Special thanks to all contributors and testers for their valuable support and feedback.
