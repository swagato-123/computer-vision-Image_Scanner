# computer-vision-Image_Scanner
from PIL import Image
import pytesseract as tess
tess.pytesseract.tesseract_cmd=r'C:\Users\Soumik Ghosh\AppData\Local\Programs\Tesseract-OCR\tesseract.exe'
demo = Image.open('success.jpg')
text = tess.image_to_string(demo,lang='eng')
print(text)
