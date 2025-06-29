# 🧠 Multi Qdrant Stack – Self-Hosted com Autenticação e Traefik

Este repositório contém a configuração completa para executar **cinco instâncias isoladas do Qdrant**, cada uma dedicada a uma área jurídica específica, com autenticação via API Key e proxy reverso com Traefik.

---

## 🚀 Objetivo

- Rodar múltiplas instâncias do [Qdrant](https://qdrant.tech) via Docker Compose
- Gerenciar via [Portainer](https://www.portainer.io/)
- Expor via Traefik com HTTPS automático (Let's Encrypt)
- Usar API Keys únicas por instância para controle de acesso
- Organizar variáveis sensíveis via arquivo `.env`

---

## 🧱 Estrutura

```bash
multi-qdrant/
├── docker-compose.yml   # Stack principal com os 5 serviços Qdrant
└── .env                 # Chaves API de cada instância
