
# **TrackEase: Automatic Attendance System Using Face Recognition**  

---

## **Project Description**  

**TrackEase** is a fully automated attendance management system designed to simplify and enhance the attendance tracking process for educational institutions. Using advanced face recognition models, it enables contactless, real-time attendance marking via live camera feeds. It eliminates manual errors and ensures data accuracy while providing teachers with powerful reporting tools.  

---

## **Features**  

### For Students:    
- **Attendance Tracking**: Attendance is marked automatically when their face is detected in the live feed.  
- **Attendance History**: View attendance history on the platform.  

### For Teachers:  
- **Secure Registration**: Teachers register via email/phone with OTP verification.  
- **Real-Time Attendance**: Automatically detect and mark student attendance from a live camera feed.  
- **Attendance Reports**: Generate and view reports for specific dates and time periods.  

---

## **Technologies Used**  

### **Frontend**:  
- **HTML & CSS + Jinja**: For building a fast, responsive, and user-friendly web interface.  

### **Backend**:  
- **Flask**: A lightweight Python web framework to handle API requests and backend logic.  
- **dlib**: For face recognition and feature extraction using pre-trained models.  
  - `dlib_face_recognition_resnet_model_v1.dat`: Extracts facial embeddings.  
  - `shape_predictor_68_face_landmarks.dat`: Identifies facial landmarks.  

### **Database**:  
- **MongoDB**: For storing user data, facial features, and attendance records.  

### **Other Tools**:  
- **OpenCV**: For live camera feed processing.  
- **DCGAN**: For generating synthetic data to augment a small dataset.  

---

## **System Architecture**  

```plaintext
Frontend (React + Vite) --> Backend (Flask API) --> MongoDB Database
                                      |
                                Face Recognition
                                      |
                             Live Camera Feed (OpenCV)
