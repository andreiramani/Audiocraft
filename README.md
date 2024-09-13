# Audiocraft
How to install Audiocraft
<br>
(Case study in Windows 11)
<br>

1. Create conda environment with Python 3.9
   ```
   conda create --name audiocraft python=3.9
   ```
3. Conda activate environment with ```conda activate audiocraft```
4. Download and install CUDA Toolkit 12.1 from NVIDIA website
5. Install pytorch with CUDA 12.1 support
   ```
   conda install pytorch==2.1.0 torchvision==0.16.0 torchaudio==2.1.0 pytorch-cuda=12.1 -c pytorch -c nvidia
   ```
6. Make sure torch cuda enable, with:
   ```
   import torch
   print(torch.cuda.is_available())
   ```
8. Git clone from ```git clone -b plus https://github.com/ClownOfMadness/audiocraft_plus```
9. Install all requirements package with ```pip install -r requirements.txt```
10. Run UI with ```python app.py```, make sure there is no single error
11. Access the frontend with your browser, type in address bar ```http://127.0.0.1:7860```
<br>
Note: ignore error from <b>Error caught was No module named 'triton'</b>
