오목코딩에서 numpy, pyqt5, tensorflow를 import하는데 생겼던 오류들을 해결하고 나서는 새로운 오류가 생겼다
play_with_AI의 코드에서 
Traceback (most recent call last):
  File "C:\Windows\system32\python", line 343, in <module>
    ex = MyApp()
  File "C:\Windows\system32\python", line 16, in __init__
    self.initUI()
  File "C:\Windows\system32\python", line 38, in initUI
    self.board_cv2 = cv2.cvtColor(board_cv2, cv2.COLOR_BGR2RGB)
cv2.error: OpenCV(4.4.0) C:\Users\appveyor\AppData\Local\Temp\1\pip-req-build-xr4y3u3_\opencv\modules\imgproc\src\color.cpp:182: error: (-215:Assertion failed) !_src.empty() in function 'cv::cvtColor'
와 같은 오류가 생겨나는데 이건 이미지 파일이 제데로 로딩되지 않아서 발생하는 문제이다. 
  답변자 님의 말대로 코드를 고쳐보았지만 않된다
