

# 🔒 Testes de Segurança & Carga com Cypress

Este módulo faz parte de uma suíte de testes com **Cypress**, com foco em validar **segurança** e **resiliência sob carga** de APIs públicas.

## ⚙️ O que está incluso

### 1. **Testes de Segurança**
Local: `security.cy.js`
- Validação de login com credenciais inválidas.
- Simulação de ataques (ex: SQL Injection).
- Verificação de ausência de dados sensíveis na resposta.
- Teste de autenticação e tratamento de erro.

### 2. **Testes de Carga**
Local: `load.cy.js`
- Execução de 30 requisições simultâneas em endpoints críticos.
- Validação do tempo de resposta (`duration`) para GET e POST.
- Simulação de criação massiva de usuários com dados variados.

## 🧰 Tecnologias

- **Cypress** – Automação de testes moderna.
- **Reqres.in** – Testes com foco em segurança/autenticação.
- **FakeStoreAPI** – Testes com foco em performance/carga.

## 🎯 Benefícios

- **Detecta vulnerabilidades comuns** antes de afetar o usuário final.
- **Valida resiliência da API** em cenários com múltiplos acessos simultâneos.
- **Garante o comportamento esperado** em ambientes de produção simulados.

## ▶️ Como executar

```bash
npm install
npx cypress open
