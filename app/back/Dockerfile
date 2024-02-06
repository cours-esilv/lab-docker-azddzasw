# 使用官方的 Python 运行时作为父镜像
FROM python:3.8

# 将工作目录设置为 /app
WORKDIR /app

# 将当前目录的内容复制到容器中的 /app
COPY . /app

# 安装 requirements.txt 中指定的所有依赖包
RUN pip install --no-cache-dir -r requirements.txt

# 将端口 5000 开放给容器外部
EXPOSE 5000

# 运行应用程序
CMD ["python", "-m", "flask", "run", "--host=0.0.0.0"]


