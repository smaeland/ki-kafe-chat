# KI kafé chat

### Frontend

Install docker, docker compose

Start servers:
```
docker compose up -d
```

**TODO**  change nginx server name 

### GPU server

open firewall for frontend server (ok)

open tmux

install uv
```
curl -LsSf https://astral.sh/uv/install.sh | sh
```

install vllm
```
uv venv myenv --python 3.12 --seed
source myenv/bin/activate
uv pip install vllm
```

run
```
vllm serve norallm/normistral-7b-warm-instruct
```



