# deepl-bk
用于zotero中deepl的key

1.安装docker
参考： https://www.docker.com/

2. 拉取镜像
    在终端中执行：

       docker pull kanikig/deepl-bk

4. 部署 DeepL 服务
   Mac（Intel）和 Windows ：

       docker run -itd -p 8080:80 kanikig/deepl-bk 
   Mac（M1/M2）：

       docker run --platform linux/amd64 -p 8080:80 -itd kanikig/deepl-bk
    其中，8080 是服务运行的端口，可以修改为其他数值。

6. 在 Zotero 中配置
    打开 Zotero – 选项 – 翻译 – 翻译引擎 – DeepL(自定义)，在密钥中输入网址。
    如果按照上完进行配置，则链接为： http://127.0.0.1:8080/translate 。
