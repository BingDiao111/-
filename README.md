- 该代码所需用到的26个matrix太大了，没有上传到github，已经随邮件里的压缩包发送到助教的邮箱  
- 创建一个新的文件夹，并将压缩包中的matrix文件夹下载到该目录下，同时将该仓库中的BRMerge文件夹下载到该目录下  
- (本仓库中的Existing文件夹是论文原作者所用到的，但本实验并没有用到，可不下载)

- **配置环境  (均在unbuntu终端中输入)**  
(1) 配置`Intel`的`oneAPI base toolkit`代码：  
`wget https://registrationcenter-download.intel.com/akdlm/IRC_NAS/20f4e6a1-6b0b-4752-b8c1-e5eacba10e01/l_BaseKit_p_2024.0.0.49564_offline.sh`  
`sudo sh ./l_BaseKit_p_2024.0.0.49564_offline.sh`  
(2) 配置`Intel`的`HPC toolkit`代码：  
`wget https://registrationcenter-download.intel.com/akdlm/IRC_NAS/1b2baedd-a757-4a79-8abb-a5bf15adae9a/l_HPCKit_p_2024.0.0.49589_offline.sh`  
`sudo sh ./l_HPCKit_p_2024.0.0.49589_offline.sh`  
(3) 接着把`oneAPI`和`HPC`的路径加入到`makefile`的`include`中

- **编译**  
- 在终端进入`BRMerge`文件夹，编译所有文件`$ sudo bash make.sh`  

- **运行**
- 接着运行`.sh`文件，如 `./brmerge_precise patents_main patents_main 80` 或者 `./brmerge_upper patents_main patents_main 80`，中间的`patents_main`为矩阵的名称，可以更改
