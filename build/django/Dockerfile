#定义该镜像使用的基础镜像为：python:3.7.4-stretch
FROM python:3.6.8-stretch

#定义容器的工作目录
WORKDIR /wwwroot

#拷贝pip安装项目所需要的包名称和第三方django xadmin管理后台
COPY requirements.txt ./

RUN pip install --upgrade pip -i https://pypi.douban.com/simple/
#安装
RUN pip install -r requirements.txt -i https://pypi.douban.com/simple/

#开放的端口
EXPOSE 8000