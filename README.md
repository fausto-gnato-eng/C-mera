# Camera
Este software premite a abertura de uma webcam, ou uma camera usb.
oooooooooooooooooooooooooooooooooooooooooooooooooooooooooooo

import cv2 -> Importa OpenCV Python

import numpy as np -> Importa biblioteca Numpy, e a apelida de np

cap = cv2.VideoCapture(0) -> Declara variavel de captura de video com parametro localizador = 0

while True: -> Cria loop infinito para atualixaçao de frames.

   _, frame = cap.read() -> Invoca o retorno(_), e o frame.

   cv2.imshow("frame",frame) -> Mostra o frame.

   key = cv2.waitKey(1) -> Solicita o tempo de atualizaçao em milisegundos (Num/ seg), corresponde a o delay do loop.

   if key == 27: -> invoca o esc.

    break -> Freia o loop.

cap.release() -> Libera a variavel cap.

cv2.destryAllWindows() -> Destroi todas as janelas.