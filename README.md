# hello

## 启动服务

```bash
python3 server.py
```

启动后访问 <http://localhost:8000/>，根路径会返回 `index.html` 主页。

也可以通过 `PORT` 环境变量修改端口：

```bash
PORT=8080 python3 server.py
```

## 使用 Docker

构建镜像：

```bash
docker build -t hello-homepage .
```

启动容器：

```bash
docker run --rm -p 8000:8000 hello-homepage
```

然后访问 <http://localhost:8000/>。