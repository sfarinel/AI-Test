### Clone roop repo and install dependencies

``` 
!git clone https://github.com/based9based/roop
%cd roop
!pip install -r requirements.txt
``` 




### download model

``` 
!wget https://civitai.com/api/download/models/85159 -O inswapper_128.onnx
``` 



### Deepfake
ricordarsi di cambiare il path sia dell'immagine che del video di origine (target)
``` 
!python run.py --target /content/NSF.mp4 --source /content/AS.jpg -o /content/swapped.mp4 --execution-provider cuda --frame-processor face_swapper face_enhancer
``` 
