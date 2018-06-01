jupyter notebook --generate-config
sed -ie "s/#c.NotebookApp.ip = 'localhost'/#c.NotebookApp.ip = '*'/g" ~/.jupyter/jupyter_notebook_config.py
sudo python3 -m pip install tensorflow-gpu==1.1 udacity-pa tqdm
sudo apt-get install libav-tools
sudo python3 -m pip install python_speech_features librosa soundfile
jupyter notebook --ip=0.0.0.0 --no-browser
