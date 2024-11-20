# Pytorch-Setup-for-GPU-with-Anacodna  

**Step-1: Check whether your system has nvidia gpu or not.**  
Open the command prompt and  
type ``` nvidia-smi``` to see the if you have GPU or not  
type ```nvcc --version``` to see the cuda version  

**Step-2: Install Anaconda on your system**  
Go to the Anaconda download website and then download for your operating system suitable verison.  
Run the .exe file as administration and install as usual.  

**Step-3: Setting up a Pytorch environment**  
--> Open Anaconda Prompt from the start menu
--> type ```conda create --name env_name``` then type ```y```  
--> type ```conda activate env_name```  
--> type ```conda install cudatoolkit -c anaconda -y```  
--> type ```conda install pytorch-cuda=12.1 -c pytorch -c nvidia -y```  
--> type ```conda install pytorch torchvision torchaudio -c pytorch -c nvidia -y```  
--> type ```import torch``` to check pytorch installation   
--> type ```torch.cuda.is_avaiable()``` to check is GPU is enabled or not

**Step-4: Installing Jupyter Lab using cuda**  
--> type ```conda install -c conda-forge jupyterlab```  


You are good to go and do some deep learning stuff in your local machine



