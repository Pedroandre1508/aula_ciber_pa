#  🔐Pipeline DevOps e Demonstração de Segurança em Aplicações Web

Este projeto combina a implementação de um pipeline de CI/CD com exemplos práticos de vulnerabilidades em aplicações web. Este projeto traz demonstrações de práticas de DevOps e segurança em desenvolvimento de software.

---

## 🗄️Estrutura do Projeto

### 1. **Pipeline de CI/CD**
O pipeline automatiza o processo de build, teste, empacotamento e deploy para os serviços de backend e frontend.

#### **Workflows**
- **[ci.yml](.github/workflows/ci.yml)**: 
  - Gera versões semânticas automaticamente.
  - Compila e empacota os artefatos do backend e frontend.
  - Executa testes automatizados.
  - Publica os artefatos gerados.

- **[deploy.yml](.github/workflows/deploy.yml)**:
  - Realiza o deploy dos artefatos gerados em ambientes de teste (TST) ou produção (PRD).
  - Utiliza SSH e `rsync` para atualizar os servidores.

---

### 2. **Aplicação Backend**
O backend é desenvolvido com o framework **NestJS** e inclui:
- **Build e Testes**:
  - Scripts para build e execução de testes unitários e de integração.
- **Estrutura**:
  - Código principal em TypeScript.
  - Configuração de ESLint e Prettier para padronização de código.

---

## 🚀**Execução**
1. É necessario acessar a aba "Actions" no Github.
2. Selecionar a ação a ser executada.
3. Clicar no botão "Run Workspace".
4. Selecionar a branch e executar a ação desejada.

_OBS: Caso seja selecionado a ação de deploy, deve ser informado apenas a versão no campo "Nome do artefato/versão"_ 
