# RFID Based Attendance and Security System

## Project Overview

This project is designed as a security and attendance management system using **RFID (Radio Frequency Identification)** technology. It aims to reduce the time and errors involved in manual attendance-taking processes in educational institutions. The system also provides an added layer of security by regulating access to classrooms based on user identification.

### Key Components:
- **Arduino MEGA**
- **RFID Tags and Reader**
- **LED and LCD Display**
- **USART Communication**

## Features
- **Automated Attendance System**: Uses RFID tags for students to mark attendance by scanning their cards.
- **Access Control**: Only faculty, staff, and registered students are allowed to enter classrooms. Guests are denied entry.
- **Real-time Feedback**: Displays access status and attendance confirmation on an LCD screen.
- **SMS Notification**: Option to send attendance details to parents.

## Motivation
In traditional colleges, attendance is often managed manually on paper, which can be error-prone and time-consuming. By using RFID technology, this project aims to streamline the process and ensure greater security within the campus.

## System Flow
1. **RFID Tag Detection**: When a student, faculty, or guest scans their RFID tag at the reader, the tag's information is sent to the controlling Arduino MEGA via USART.
2. **Identity Verification**: The Arduino checks the identity of the person (student, faculty, staff, or guest).
3. **Attendance Marking**: If the person is a student, their attendance is automatically marked.
4. **Access Control**: If the user is a faculty or staff member, they are granted access to the classroom. Guests are denied entry.
5. **LCD Feedback**: The system displays whether access is permitted and attendance is marked.

## Program Flow Chart

1. The RFID reader detects the RFID tag.
2. Tag information is sent to Arduino via USART.
3. Arduino checks if the tag belongs to a student or staff.
4. If student, attendance is marked.
5. Access is granted or denied based on user role.

## Android Application (Optional)
This project can also integrate with an Android application that allows users to check their attendance status or receive alerts when attendance is marked.

## How to Run

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/username/rfid-attendance-security-system.git
    cd rfid-attendance-security-system
    ```

2. **Upload the Code**:
    - Use the **Arduino IDE** to upload the complete C program to the Arduino MEGA.

3. **Circuit Setup**:
    - Connect the RFID reader, LCD, LED, and other components as per the circuit diagram provided.

4. **Test the System**:
    - Place an RFID tag near the reader to test the system's functionality.

## Dependencies

- Arduino IDE
- RFID Library for Arduino
- LCD Display Library

## Future Enhancements
- **Mobile Notification**: Expand the system to send real-time notifications to parents when attendance is marked.
- **Database Integration**: Connect the system to a central database for storing attendance records.
- **Web Interface**: Create a web-based dashboard for administrators to monitor attendance and access logs.

## Contributors
- Manav Shah (1741042)
- Dhruvil Shah (1741024)
- Deep Gohel (1741060)
- Yug Patel (1741017)

## Guide and Mentor
- Prof. Anurag Lakhlani, School of Engineering and Applied Science, Ahmedabad University

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## References
- [Arduino MEGA Documentation](https://www.arduino.cc/en/Main/ArduinoBoardMega)
- [RFID Technology Overview](https://en.wikipedia.org/wiki/Radio-frequency_identification)
