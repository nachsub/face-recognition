# face-recognition
Author: Nachiket Subbaraman <br />
Dependencies: PIL, CMake, dlib, opencv-python,
face_recognition (use pip install) and haarcascade_frontalface_default.xml

Face recognition should take input using face-input, where
the user specifies the file location for their faces to go.
It currently uses the webcam to take 10 consecutive pictures
of the user's face.

Face-recognition needs that file location as input, and
tries to match those faces with the user's face, and takes
screenshots when a matching face is found using webcam.
The screenshot's name is saved as a datetime string concatenated
with the name of the file that was found.

File structure:<br />
|posts
  * |2019
    * |markdown
|face-input.py
|face-detection.py
|haarcascade_frontalface_default.xml
|fn_dir
  * |fn_name
    * |known_faces  

Usage instructions:
  * - change fn_dir (to name where directory of faces are going to be stored)
    and fn_name in face-input (where certain users faces are going to be stored)
  * - make a directory using the same name as you put for fn_dir in the code
  * - run face-input
  * - change root variable in face-recognition to the path "fn_dir/fn_name"
  * - run face-recognition
