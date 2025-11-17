#🎯 Attendance Management System Using Face Recognition (AMSUFR)

A smart, camera-based attendance system built with Python that leverages facial recognition to automate and streamline identity verification. Designed with a user-friendly GUI, this project integrates OpenCV, Tkinter, and machine learning to capture, train, and recognize faces—making manual attendance obsolete.

## 📸 Features

- **Real-Time Face Detection** using OpenCV
- **Face Capture and Dataset Creation** with ID, Name, and Email
- **Model Training** using LBPH (Local Binary Patterns Histograms)
- **Automated Face Recognition** for attendance logging
- **Email Notification System** to send alerts or summaries
- **Intuitive GUI** built with Tkinter for seamless interaction
- **Camera Check Utility** to verify hardware readiness

## 🛠️ Tech Stack

| Component        | Technology Used            |
|------------------|----------------------------|
| Programming      | Python 3.x                 |
| GUI Framework    | Tkinter                    |
| Face Detection   | OpenCV (Haar Cascades)     |
| Recognition Model| LBPH Face Recognizer       |
| Email Service    | smtplib (Python SMTP)      |
| Data Storage     | CSV / Local Filesystem     |

## 🚀 How It Works

1. **Check Camera**: Ensures webcam is connected and functioning.
2. **Capture Faces**: Collects facial images with associated ID, Name, and Email.
3. **Train Images**: Builds a recognition model from the captured dataset.
4. **Recognize Faces**: Identifies individuals and logs attendance.
5. **Auto Mail**: Sends email notifications (e.g., attendance summary).
6. **Exit**: Closes the application safely.

## 📂 Project Structure

```
AMSUFR/
├── dataset/              # Stores captured face images
├── trainer/              # Stores trained model files
├── attendance.csv        # Logs recognized attendance
├── main.py               # Entry point with GUI
├── camera.py             # Camera check and capture logic
├── trainer.py            # Model training script
├── recognizer.py         # Face recognition logic
├── mailer.py             # Email automation
└── README.md             # Project documentation
```

## 🧑‍💻 Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/amsufr.git
   cd amsufr
   ```

2. Install dependencies:
   ```bash
   pip install opencv-python numpy pillow
   ```

3. Run the application:
   ```bash
   python main.py
   ```

## 📧 Email Configuration

To enable the Auto Mail feature:
- Update `mailer.py` with your SMTP credentials.
- Use app-specific passwords if using Gmail with 2FA.

## 🧪 Future Enhancements

- Integration with cloud-based databases
- Mobile app interface
- Multi-camera support
- Attendance analytics dashboard

## 🙌 Acknowledgements

- [OpenCV](https://opencv.org/)
- [Tkinter](https://docs.python.org/3/library/tkinter.html)
- Python community for open-source inspiration
