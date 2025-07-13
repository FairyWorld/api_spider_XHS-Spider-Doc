# 使用 Nginx 作为基础镜像
FROM nginx:alpine

# 复制当前目录（dist/）下的所有文件到 Nginx 的默认静态资源目录
COPY . /usr/share/nginx/html

# 复制 Nginx 配置文件
COPY nginx.conf /etc/nginx/conf.d/default.conf

# 暴露 80 端口
EXPOSE 80

# 启动 Nginx（保持前台运行）
CMD ["nginx", "-g", "daemon off;"]