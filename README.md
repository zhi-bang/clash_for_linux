# Clash_for_linux
这是我分享的关于在linux上使用魔法的工具文件，首先说明一下，作者不是我。
> ⚠️ 本项目原始作者为：https://github.com/nelvko
> 本仓库仅用于分享或备份，原始版权归原作者所有。
<img width="1851" height="1100" alt="image" src="https://github.com/user-attachments/assets/40e1b260-97b4-4d77-82db-56f10129933b" />


首先，我们使用如下命令将文件clone到linux宿主机

> git clone https://github.com/zhi-bang/clash_for_linux
> 
> 结果发现不能clone，因为没有魔法。所以，我们使用Code -> Download ZIP手动下载clash_for_linux-main.zip这个文件，然后上传到目标linux服务器
> 
> 接下来，使用unzip clash_for_linux-main.zip解压缩
> 
然后，cd clash_for_linux-main/ 

进入主文件夹后输入如下命令安装clash

sudo bash install.sh

输入订阅连接（没有订阅的可以查看如下网站：https://sakura-cat1.com/）

然后看到提示 “未检测到代理变量，可执行 clashon 开启代理环境”

输入

clashon 

然后就可以使用HTTPS_PROXY=http://127.0.0.1:7890 git clone https://huggingface.co/。。。。进行下载github和hugging face上的内容了, 比如：

HTTPS_PROXY=http://127.0.0.1:7890 git clone https://huggingface.co/Qwen/Qwen3-Embedding-0.6B-GGUF

