# Pasos para ejecutar programa
conda create --name (nombre enviroment) python=3.12 -y
conda activate (nombre enviroment)
# Colocar la direccion de la carpeta después de clonarla e.g. -> cd C:\Users\USER\Documents\yolo\...
pip install label-studio # Solo si quieres modificar el dataset
pip install ultralytics
pip install opencv-python
pip3 install --upgrade torch torchvision torchaudio --index.url https://download.pytorch.org/whl/cu124 # Solo si tienes Nvidia GPU
python yolo_detect.py --model my_model.pt --source usb0 --resolution 1280x720 # Usa la cámara en el entorno local
