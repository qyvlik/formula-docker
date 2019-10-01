# formula-full

1. make sure you have install `docker` and `docker-compose`
2. copy [.env.example](./.env.example) to [`.env`](./.env)
3. define the env var in the [`.env`](./.env) file
4. copy [fetch-config.json.example](./formula-data/fetch-config.json.example) as [fetch-config.json](./formula-data/fetch-config.json)
5. define the exchange and market which you want fetch
6. `docker-compose pull`
7. `docker-compose up -d`

## cn

1. 确认安装好 `docker`, `docker-compose`
2. 将 [.env.example](./.env.example) 拷贝到同目录下，并命名为 [`.env`](./.env)，[`.env`](./.env) 是给 `docker-compose` 使用的
    - [`.env`](./.env) 有若干环境变量
3. 将 [fetch-config.json.example](./formula-data/fetch-config.json.example)  拷贝到同目录下，并命名为[fetch-config.json](./formula-data/fetch-config.json)，供 `formula-data` 使用
    - 这个文件定义了你需要抓取的交易所和交易对
4. 然后拉取 `docker` 镜像：`docker-compose pull`
5. 启动项目：`docker-compose up -d`
6. 如果需要重启项目，可以直接 `docker-compose restart`

