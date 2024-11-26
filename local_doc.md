# Local_doc

> 来自Local_doc的md

## Docker操作

docker build . -t ghcr.io/yingchaoorg/local_docs-v1-cn-vuejs-org:master

docker  stop local_docs-v1-cn-vuejs-org
docker  rm local_docs-v1-cn-vuejs-org

docker run -it  --name local_docs-v1-cn-vuejs-org -p 34807:80 -d --rm -v ./:/usr/share/nginx/html ghcr.io/yingchaoorg/local_docs-v1-cn-vuejs-org:master

docker  exec -it  local_docs-v1-cn-vuejs-org  bash

## bash脚本

```bash

#!/bin/bash

Header always set Content-Security-Policy "script-src 'self'"
add_header Content-Security-Policy "script-src 'self'";

<meta http-equiv="content-security-policy" content="策略集">


```
