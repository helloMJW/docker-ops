# docker-ops

监控、CI/CD、版本控制、代理服务、工具、备份管理、定时任务

### 内网穿透服务

**frps服务端**
`docker run --restart=always --network host -d -v /websys/opt/docker/docker-ops/frp/frps.ini:/etc/frp/frps.ini --name frps snowdreamtech/frps:0.32.0`

**frpc客户端**
`docker run --restart=always --network host -d -v /websys/opt/docker/docker-ops/frp/frps.ini:/etc/frp/frpc.ini --name frpc snowdreamtech/frpc:0.32.0`