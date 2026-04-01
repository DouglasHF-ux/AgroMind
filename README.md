# 🌱 AgroGestão Rural

> Sistema acadêmico de gestão para propriedades rurais, desenvolvido com foco em
> escalabilidade, separação de responsabilidades e boas práticas de engenharia de software.

![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=flat&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-5.x-092E20?style=flat&logo=django&logoColor=white)
![React](https://img.shields.io/badge/React-19+-61DAFB?style=flat&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat&logo=typescript&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.x-4479A1?style=flat&logo=mysql&logoColor=white)
![License](https://img.shields.io/badge/licença-MIT-green?style=flat)

---

## 📋 Sobre o Projeto

O **AgroGestão Rural** é um sistema de gestão desenvolvido como projeto acadêmico,
voltado ao controle e acompanhamento de propriedades rurais. O sistema permite o
gerenciamento de safras, operações de campo, dados climáticos, controle financeiro,
estoque, colaboradores e precificação de commodities — tudo centralizado em uma
única plataforma.

---

## 🧩 Módulos

| Módulo | Descrição |
|---|---|
| **Usuários** | Autenticação JWT, RBAC (Produtor / Admin), recuperação de senha |
| **Propriedades** | Cadastro e gestão de fazendas e talhões |
| **Plantio** | Controle de safras, culturas e ciclos produtivos |
| **Clima** | Registro e consulta de dados climáticos por propriedade |
| **Operações** | Registro de atividades de campo e maquinário |
| **Financeiro** | Receitas, despesas e relatórios por safra |
| **Estoque** | Controle de insumos e produtos armazenados |
| **Colaboradores** | Gestão de equipe e alocação por operação |
| **Commodities** | Acompanhamento de preços de mercado |

---

## 🛠️ Stack Tecnológica

### Backend
- **Python 3.12+** com **Django 5.x** e **Django REST Framework**
- Autenticação via **SimpleJWT**
- Banco de dados **MySQL 8.x**
- Arquitetura em camadas: `services.py` / `selectors.py` / `serializers.py`
- Testes com **pytest** + **factory-boy**

### Frontend
- **React 19+** + **Vite** + **TypeScript**
- Estilização com **Tailwind CSS**
- Requisições com **Axios** + **TanStack Query**
- Formulários com **React Hook Form** + **Zod**
- Gráficos com **Recharts**

---

## 🏗️ Estrutura do Projeto
```
AgroGestao/
├── backend/
│   ├── config/
│   │   └── settings/
│   │       ├── base.py
│   │       ├── development.py
│   │       └── production.py
│   ├── apps/
│   │   ├── users/
│   │   ├── properties/
│   │   ├── planting/
│   │   ├── climate/
│   │   ├── operations/
│   │   └── financial/
│   └── manage.py
└── frontend/
    ├── src/
    └── vite.config.ts
```

---

## 🚀 Como Executar Localmente

### Pré-requisitos
- Python 3.12+
- Node.js 18+
- MySQL 8.x

### Backend
```powershell
cd AgroGestao/backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env   # configure suas variáveis
python manage.py migrate
python manage.py runserver
```

### Frontend
```powershell
cd AgroGestao/frontend
npm install
npm run dev
```

---

## ✅ Status do Desenvolvimento

- [x] Sprint 01 — Autenticação e gestão de usuários (RF-01 a RF-06)
- [ ] Sprint 02 — CRUD completo de usuários + início do frontend
- [ ] Sprint 03 — Módulo de Propriedades
- [ ] Sprint 04 — Módulo de Plantio
- [ ] *(em andamento...)*

---

## 📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.
