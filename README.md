# n8n_study

## Aula 02: Instalando o N8N com Docker

### Pré-requisitos

Antes de começar, certifique-se de que você tem as seguintes ferramentas instaladas:

1. **Docker**: Utilize a [documentação oficial do Docker](https://docs.docker.com/get-docker/) para instalar.

### Passo a passo para instalação (estudo)

#### 1. Crie um volume

```bash
docker volume create n8n_data
```

#### 2. Suba o serviço

```bash
docker run -d --name n8n -p 5678:5678 -e N8N_ENFORCE_SETTINGS_FILE_PERMISSIONS=true -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```
