# Camera
Este software premite a abertura de uma webcam, ou uma camera usb.
oooooooooooooooooooooooooooooooooooooooooooooooooooooooooooo

import cv2 -> Importa OpenCV Python

import numpy as np -> Importa biblioteca Numpy, e a apelida de np

cap = cv2.VideoCapture(0) -> Declara variavel de captura de video com parametro localizador = 0

while True: -> Crialup infinito para atualixaçao de frames.

   _, frame = cap.read()
   cv2.imshow("frame",frame)
   key = cv2.waitKey(1)
   if key == 27:
    break
cap.release()
cv2.destryAllWindows()