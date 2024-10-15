<h1>Intrusion Detection System</h1>

<p>This project is an <strong>Intrusion Detection System</strong> built using Python and OpenCV, designed to detect human intrusions in real-time using computer vision techniques. The system uses a camera feed to capture and process video, detecting human faces and triggering alerts when an intrusion is detected. Upon detection, the system generates instant reports, saves snapshots, and sends email alerts with the detected images.</p>

<h2>Features</h2>
<ul>
  <li><strong>Real-time Face Detection</strong>: Detects human faces in the video feed using the Haar Cascade classifier.</li>
  <li><strong>Intrusion Alerts</strong>: Automatically captures and saves images of detected intrusions with a timestamp.</li>
  <li><strong>Image Capture and Storage</strong>: Saves the detected face images with precise timestamps for record-keeping.</li>
  <li><strong>Instant Reporting</strong>: Generates instant alerts and prepares the video summary of detected intrusions.</li>
</ul>

<h2>How It Works</h2>
<ol>
  <li>The system captures video from a connected camera.</li>
  <li>It processes each video frame and converts it to grayscale.</li>
  <li>Using a Haar Cascade Classifier, it detects human faces in the frame.</li>
  <li>Upon detection, the system:
    <ul>
      <li>Highlights the face with a bounding box.</li>
      <li>Captures and stores an image of the face with a timestamp.</li>
      <li>Saves all captured images to generate a video summary later.</li>
    </ul>
  </li>
  <li>The system generates an MP4 video summary of all intrusions when terminated by the user.</li>
</ol>

<h2>Prerequisites</h2>
<ul>
  <li>Python 3.x</li>
  <li>OpenCV (Install using <code>pip install opencv-python</code>)</li>
  <li>A camera (webcam) for video capture</li>
  <li>Haar Cascade Classifier file (included in OpenCV or download from <a href="https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml">here</a>)</li>
</ul>

<h2>How to Run</h2>
<ol>
  <li>Clone the repository.</li>
  <li>Ensure all dependencies are installed (OpenCV).</li>
  <li>Run the Python script:
    <pre><code>python Detector.py</code></pre>
  </li>
  <li>The video stream will appear. To terminate the program, press <code>q</code>.</li>
</ol>

<h2>Future Improvements</h2>
<ul>
  <li>Adding email alert functionality upon detection.</li>
  <li>Integrating more advanced machine learning models for activity detection.</li>
  <li>Improving face detection accuracy in low-light conditions.</li>
</ul>

<h2>License</h2>
<p>This project is licensed under the MIT License.</p>
