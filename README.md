# Real-Time Sign Language Translation

###  Screenshots
Screenshots demonstrating the working of the system are included in the uploaded project report.


##  About the Project
This project focuses on building a real-time sign language translation system that converts hand gestures into readable text. It is designed to help bridge the communication gap between hearing-impaired individuals and people who do not understand sign language. The system works live using a webcam and displays the translated output instantly on the screen.



##  Project Overview
The application detects hand movements using MediaPipe and recognizes gestures using a deep learning model. A combination of CNN and LSTM is used so that the system can understand both hand shape and motion over time. This allows the system to recognize not only static signs but also dynamic gestures such as actions and expressions. The model processes live video input and provides accurate text output in real time.



##  How the Project Works
1. **Live Video Capture**: The system captures the user's hand gestures using a webcam via OpenCV.  
2. **Hand Detection**: MediaPipe identifies the hand and extracts 21 key landmarks for each frame (x, y, z coordinates).  
3. **Sequence Formation**: Consecutive frames are collected to form a sequence, capturing the motion of the gesture.  
4. **Feature Extraction**: CNN layers process each frame to extract spatial features like finger positions and hand shape.  
5. **Temporal Analysis**: LSTM layers analyze the sequence of frames to understand dynamic motion patterns.  
6. **Gesture Classification**: The combined CNN–LSTM model predicts the gesture and converts it into text.  
7. **Text Display**: The recognized gesture is displayed on screen in real time, updating continuously as gestures change.  

This workflow allows the system to handle both static gestures (like numbers or letters) and dynamic gestures (like waving or actions), providing real-time translation.



##  Key Features
- Real-time gesture recognition using a webcam  
- Supports numbers, words, emotions, and action-based gestures  
- Detects hand landmarks using MediaPipe  
- Uses CNN for spatial feature extraction  
- Uses LSTM to learn gesture movement over time  
- Displays translated text instantly on screen  
- Works well under different lighting and hand orientations  



##  Tools & Technologies Used
- **Python** for overall implementation  
- **OpenCV** for webcam capture and video processing  
- **MediaPipe** for real-time hand landmark detection  
- **TensorFlow / Keras** for building the CNN–LSTM model  
- **NumPy** for data processing and array handling  
- **VS Code** as the development environment  



##  Project Goals
- Enable real-time translation of sign language into text  
- Support dynamic gestures instead of only static signs  
- Improve accessibility for hearing-impaired users  
- Create a system suitable for assistive and educational use  



##  Applications
- Communication aid for hearing- and speech-impaired users  
- Educational platforms for learning sign language  
- Customer service and public service assistance  
- Human–Computer Interaction (HCI) systems  
- Smart devices and gesture-based control systems  
- Virtual and augmented reality environments  



##  Conclusion
This project demonstrates how deep learning and computer vision can be used to solve real-world accessibility challenges. By combining MediaPipe with a CNN–LSTM model, the system successfully translates sign language gestures into text in real time. With further improvements, it has the potential to become a powerful assistive communication tool.
