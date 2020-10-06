# reproducibility-tutorial-2020

## Computer setup 

1. Clone my git repo
    
    git clone https://github.com/JasonJWilliamsNY/reproducibility-tutorial-foss-2020.git

2. Download and install Miniconda
    
    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh


   15  bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/conda
   16  clear
   17  ln -s /opt/conda/pkgs/*/bin/* /bin
   18  ln -s /opt/conda/pkgs/*/lib/* /usr/lib
   19  clear
   20  /opt/conda/bin/conda install -c conda-forge -y jupyterlab=1.2.3
   21  /opt/conda/bin/conda install -c conda-forge -y nodejs=10.13.0
   22  clear
   23  \
   24  conda search qiime
   25  /opt/conda/bin/conda search qiime
   26  /opt/conda/bin/conda search -c bioconda qiime
   27  clear
   28  /opt/conda/bin/jupyter lab --no-browser --allow-root --ip=0.0.0.0 --NotebookApp.token='' --NotebookApp.password='' --notebook-dir='/scratch/reproducibility-tutorial/'
   29  clear
   30  /opt/conda/bin/pip install bash_kernel
   31  /opt/conda/bin/pip install ipykernel
   32  /opt/conda/bin/python3 -m bash_kernel.install
   33  clear
   34  /opt/conda/bin/conda search -c bioconda snakemake
   35  /opt/conda/bin/conda install -c bioconda -c conda-forge -y snakemake=5.8.1
   36  clear
   37  ln -s /opt/conda/bin/* /bin
   38  ln -s /opt/conda/lib/* /usr/lib
   39  clear
   40  snakemake --version
   41  cd /scratch/
   42  ls
   43  git clone https://github.com/JasonJWilliamsNY/reproducibility-tutorial-2020.git
   44  mv reproducibility-tutorial-2020 reproducibility-tutorial
   45  ls
   46  snakemake --version
   47  exit
   48  cd /scratch/
   49  snakemake --version
   50  docker run hello-world
   51  clear
   52  sudo apt-get update
   53  sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
   54  clear
   55  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   56  sudo add-apt-repository  "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
 $(lsb_release -cs) \
 stable"
   57  sudo apt-get update
   58  clear
   59      sudo apt-get install -y docker-ce docker-ce-cli containerd.io
   60  clear
   61  docker run hello-world
   62  clear
   63  ls
   64  cd reproducibility-tutorial/
   65  ls
   66  history
   67  clear
   68  history >> README.md 
