Project Setup Steps

1. Install Python(3.9) => If Python is not installed

2. Clone RealTime-FaceMask-Detection Project from github => https://github.com/DinithS/RealTime-FaceMask-Detection.git

3. Creating Virtual Environment:
        Open Command Prompt
        cd RealTime-FaceMask-Detection
        py -m venv venv //This command will create virtual environment for your project(with virtual environment our computer/laptop file are not harmed because of installed dependencies).
        venv\Scripts\activate //This will activate the virtual environment

4. Install all Dependencies:
        pip install tensorflow>=1.15.2
        pip install keras==2.3.1
        pip install imutils==0.5.3
        pip install numpy==1.18.2
        pip install opencv-python==4.5.5
        pip install matplotlib==3.2.1
        pip install scipy==1.4.1

5. Insert dataset from here => https://www.kaggle.com/vijaykumar1799/face-mask-detection

6. Train the model => py train_facemask_detector.py

7. Test the model => py facemask_detector.py

8. Build exe 
        pip install pyinstaller
        pyinstaller facemask_detector.py
        pyinstaller -F facemask_detector.py
        pyinstaller -F --paths=<your_path>\Lib\site-packages facemask_detector.py