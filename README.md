https://github.com/mattbarty/cv_sudoku_solver/assets/52583796/23ee9cc6-10d5-40e4-b605-2d07caca98ca

<h1>Sudoku Solver and Grid Highlighter</h1>
(Check out the post on --> <a href="https://www.linkedin.com/feed/update/urn:li:activity:7101517894634586112/" target="_blank">LinkedIn</a>)</br></br>
<p>This project looked to solve Sudoku puzzles in real-time via a live webcam feed. 
  It integrates a TensorFlow-based convolutional neural network for digit prediction with sophisticated OpenCV techniques for image processing and grid detection. Capable of identifying puzzles, recognizing digits, solving puzzles algorithmically, and overlaying solutions onto the original images or video frames, this system demonstrates the power of combining machine learning and computer vision.</p>

<h2>Features</h2>
<ul>
<li><strong>Digit Prediction Model:</strong> Leverages TensorFlow and Keras to build a CNN for accurate digit prediction within Sudoku puzzles.</li>
<li><strong>Image Processing for Grid Detection:</strong> Utilizes OpenCV for advanced image manipulation, including grid detection and perspective transformation.</li>
<li><strong>Sudoku Solver:</strong> Employs a backtracking algorithm to efficiently solve detected puzzles.</li>
<li><strong>Real-time Puzzle Solving:</strong> Can process video input from a webcam, detecting, solving, and overlaying the solution on Sudoku puzzles in real time.</li>
</ul>

<h2>Computer Vision Pipeline Overview</h2>
<h3>Grid Detection and Perspective Correction</h3>
<p>Converts to grayscale and applies Gaussian blur to smoothen the image. Highlights the grid for contour detection, identifying the largest quadrilateral as the grid. Corrects the perspective to a top-down view, squaring the grid for digit processing.</p>

<h3>Digit Recognition</h3>
<p>Divides the grid into 81 cells, enhancing each for digit recognition. A CNN classifies cell contents, recognizing digits or identifying empty cells.</p>

<h3>Sudoku Solving and Solution Overlay</h3>
<p>Uses a backtracking algorithm to solve the puzzle efficiently. Maps the solution onto the grid, reverses the perspective transformation, and integrates the solved grid with the original image or video frame.</p>

<h2>Requirements</h2>
<ul>
<li>TensorFlow</li>
<li>OpenCV</li>
<li>Matplotlib</li>
<li>NumPy</li>
<li>PIL</li>
<li>Python 3.x</li>
</ul>

<h2>Installation</h2>
<p>Clone the repository and install the required Python packages:</p>
<code>pip install tensorflow opencv-python matplotlib numpy Pillow</code>

<h2>Usage</h2>
<h3>Webcam Puzzle Solving</h3>
<p>To solve puzzles in real-time via a webcam:</p>
<code>python your_script_name.py</code>
<p>Press 'q' to quit the webcam feed.</p>

<h3>Custom Puzzle Images</h3>
<p>Place puzzle images in the <code>./puzzles/</code> directory. The script processes these images, solving and displaying the solutions.</p>

<h2>Note</h2>
<p>This project is intended for educational and entertainment purposes, showcasing the integration of machine learning and computer vision techniques in Python. Performance in real-time scenarios may vary based on hardware capabilities and the complexity of the input images.</p>
