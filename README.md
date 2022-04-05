## Install drivers, cuda, and cudnn on Ubuntu 20.04
1. Install ubuntu drivers:
     1. Check the recommended drivers by running ```$ ubuntu-drivers devices```
     ![image](https://user-images.githubusercontent.com/46700815/161786238-b84799dd-83d0-4afa-950a-efb6febc83a3.png)
     2. Install the recommended driver ```$ sudo apt install nvidia-driver-470```
2. Install cuda
     1. Download the cuda toolkit from the [nvidia website](https://developer.nvidia.com/cuda-downloads)
     2. Select the version![image](https://user-images.githubusercontent.com/46700815/161787988-b718ba8f-2048-43f5-a20b-3647d7fb4a74.png)
     3. Run the installation instructions   ```$ wget https://developer.download.nvidia.com/compute/cuda/11.6.2/local_installers/cuda_11.6.2_510.47.03_linux.run```   
     4. Install cuda ```$ sudo sh cuda_11.6.2_510.47.03_linux.run```. ![image](https://user-images.githubusercontent.com/46700815/161793805-cba7ebdc-ac00-46fd-a4eb-f0874b7744dd.png)![image](https://user-images.githubusercontent.com/46700815/161793962-00bf1be7-3640-4da9-9a5f-bb144a8607f8.png)![image](https://user-images.githubusercontent.com/46700815/161794143-93674607-bff9-4e97-9152-bf99332d440c.png)
     5. Add PATH to ~/.bashrc following the instruction. ![image](https://user-images.githubusercontent.com/46700815/161795356-ce100c0e-c38f-4423-aa84-8fd3462914aa.png)![image](https://user-images.githubusercontent.com/46700815/161795424-0f6fdd42-6535-46e7-baba-d82cfef1e031.png)
     6. Check if CUDA is installed ```$ nvcc -V```![image](https://user-images.githubusercontent.com/46700815/161795580-79d6d23f-7d99-4a50-b2a4-7b212fb315b3.png)


3. Install cudnn
     1. Download cudnn from [nvidia](https://developer.nvidia.com/rdp/cudnn-download)
     2. Extract the downloaded file and copy to the cuda directory.![image](https://user-images.githubusercontent.com/46700815/161800007-e0e5d72a-db71-4c64-bafd-13699f4aec18.png)
     3. Check the cudnn version ```$ cat /usr/local/cuda/include/cudnn_version.h | grep CUDNN_MAJOR -A 2
```![image](https://user-images.githubusercontent.com/46700815/161800204-184dc423-25e0-4798-aa5f-fa5206b6d7c5.png)






