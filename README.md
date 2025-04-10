# KI kafé chat

### Frontend

Install docker, docker compose

Start servers:
```
docker compose up -d
```

### GPU server

Open firewall for frontend server

Install uv
```
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Install vllm
```
uv venv myenv --python 3.12 --seed
source myenv/bin/activate
uv pip install vllm
```

Run
```
vllm serve norallm/normistral-7b-warm-instruct
```



