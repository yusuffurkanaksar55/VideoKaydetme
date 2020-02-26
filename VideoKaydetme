import cv2
import numpy as np

kamera=cv2.VideoCapture(0)

fourcc=cv2.VideoWriter_fourcc(*"XVID")#FORMAT BELİRLEME(İNTERNETTEN BAKABİLİRİZ)
      
kayıt=cv2.VideoWriter("kayıt.avi",fourcc,30,(640,480))
      
def main():
    while True:
      ret,kare=kamera.read()
      #ters_goruntu=cv2.flip(kare,0)
      if ret==True:
          kayıt.write(kare)
          
                
     

      #cv2.imshow("Ters",ters_goruntu)
      cv2.imshow("video",kare)
    
      if cv2.waitKey(1) & 0xFF==ord('q'):
        break
    kamera.release()
    cv2.destroyAllWindows()
if __name__=="__main__":
    main()
