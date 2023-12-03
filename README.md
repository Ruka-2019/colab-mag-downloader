# colab-mag-downloader

copy this to colab to download the repo
```jupyterpython
# @title Download downloader { display-mode: "form" }
!pip install gitpython
from google.colab import drive
from git import Repo
drive.mount('/content/drive')
file_path = '/proj/dler' #@param {type:"string"}
root_path = '/content/drive/MyDrive'+file_path
Repo.clone_from('https://github.com/Ruka-2019/colab-mag-downloader.git', root_path)
```

Set the file_path to an empty folder, then open the animedl.ipynb in the folder using colab.