# StudyCaddy

```sh
# 查看帮助文档
caddy
# 前台启动
caddy run
# 指定配置文件，前台启动
caddy run --config /path/to/Caddyfile
# 后台启动
caddy start
# 停止
caddy stop

# 加载配置文件
curl localhost:2019/load \
  -H "Content-Type: application/json" \
  -d @caddy.json

# 添加权限，如果监听端口需要的话
sudo setcap cap_net_bind_service=+ep $(which caddy)
```
