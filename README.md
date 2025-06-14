# API Gateway com Traefik e Portainer

Este projeto utiliza o **Traefik** como um **API Gateway** leve e moderno, junto com o **Portainer** como ferramenta de gerenciamento de containers Docker para testes e administração visual.

## 🔧 Visão Geral

- **Traefik**: Responsável por rotear e balancear as requisições para os containers de forma dinâmica e inteligente.
- **Portainer**: Interface web para gerenciamento de containers Docker, facilitando a visualização, monitoramento e controle dos serviços.

## 📌 Endpoints

| Serviço   | URL de Acesso                  |
|-----------|--------------------------------|
| Traefik Dashboard | [`http://localhost:8080`](http://localhost:8080) |
| Portainer UI      | [`http://localhost:9001/portainer/#!/auth`](http://localhost:9001/portainer/#!/auth) |

## Acesso ao Portainer

Usarname: admin
Password: desenvolvimento

## 🚀 Benefícios de Utilizar um API Gateway

Usar um API Gateway como o Traefik traz várias vantagens para arquiteturas baseadas em microsserviços:

- **Roteamento Inteligente**: Roteia requisições para diferentes serviços com base em regras definidas por domínio, path, headers, etc.
- **Balanceamento de Carga**: Distribui as requisições entre múltiplas instâncias de serviço automaticamente.
- **Autenticação e Segurança**: Possibilita a adição de autenticação (como Basic Auth, JWT), SSL/TLS e middlewares de segurança com facilidade.
- **Monitoramento**: Interface visual para visualizar requisições, regras, serviços ativos, entre outros.
- **Reconfiguração Dinâmica**: Detecta alterações nos containers e se adapta automaticamente sem precisar reiniciar.

## 📂 Estrutura do Projeto

PI-GATEWAY/
└── Portainer/
├── portainer_data/ # Volume de dados persistente para Portainer
├── docker-compose.yml # Arquivo de configuração dos serviços
└── README.md # Documentação do projeto


## 🐳 Como Executar

1. Certifique-se de que o Docker esteja instalado e em execução.
2. Acesse o diretório do projeto:

```bash
cd Portainer
```
docker compose up --build

## 📘 Requisitos
Docker

Docker Compose

## 🧠 Observações
O Traefik foi configurado para operar como gateway reverso.

O Portainer é apenas uma ferramenta de apoio/teste neste setup.
