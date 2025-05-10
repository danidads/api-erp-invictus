# 🧪 Projeto de Testes Backend Sistema ERP - Qa.Coders

Bem-vindo ao repositório de **Sistema ERP testes backend**. Este projeto acadêmico tem como objetivo garantir a qualidade das APIs de um sistema **ERP**, através de testes automatizados criados no **Postman**, utilizando a linguagem **JavaScript** e executados via **Newman** para integração com pipelines de CI/CD.

---

## 📘 Descrição

Este repositório contém uma **coleção robusta de testes automatizados de API** voltada para validar funcionalidades críticas de um sistema ERP. Os testes foram desenvolvidos com foco em **reusabilidade**, **escalabilidade** e **facilidade de execução**, utilizando as melhores práticas de automação funcional para serviços RESTful.

---

## 🛠️ Tecnologias Utilizadas

| Ferramenta | Descrição |
|------------|-----------|
| **Postman** | Plataforma para desenvolvimento, teste e documentação de APIs. |
| **Newman** | CLI para execução de coleções Postman em ambientes CI/CD. |
| **JavaScript** | Linguagem usada nos scripts de teste para validações e manipulação de dados. |
| **Git** | Controle de versão e colaboração. |

---

## ✅ Pré-requisitos

Antes de executar os testes, verifique se possui os seguintes softwares instalados:

- [Postman](https://www.postman.com/downloads/)
- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/) (recomendado, caso deseje usar o Newman)
- [Newman](https://www.npmjs.com/package/newman) (instalável via `npm install -g newman`)

---

## 🚀 Como Executar os Testes

### 1. Clone este repositório

```bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
cd nome-do-repositorio
```
### 2. Importando para o Postman
Coleção de Testes:
Abra o Postman.

Clique em "Import" e selecione o arquivo .postman_collection.json.

Variáveis de Ambiente:
Ainda no botão "Import", selecione o arquivo .postman_environment.json.

Vá até a barra superior do Postman e selecione o ambiente importado.

### 3. Executando via Postman Runner
Clique em "Runner" no canto superior esquerdo.

Escolha a coleção desejada.

Configure o ambiente, número de iterações, delay (se necessário).

Clique em "Start Run".

### 4. Executando via Newman (Opcional)

```bash
newman run nome-da-colecao.postman_collection.json -e nome-do-ambiente.postman_environment.json -r cli,html
```
💡 Um relatório HTML será gerado para análise dos resultados.


### 🔍 Cobertura de Testes
Os testes automatizados cobrem:

Autenticação (login, token JWT)

CRUD de entidades (usuários, produtos, pedidos, etc.)

Validações de status HTTP

Validações de schema e estrutura do JSON de resposta

Testes com massa dinâmica (pré e pós-execução)

Testes de exceção e entradas inválidas

### 📊 Relatórios
Após a execução, é possível visualizar os resultados diretamente no Postman (aba "Test Results") ou, se estiver utilizando Newman com o reporter HTML, em um relatório gerado automaticamente, contendo:

Sucesso/falha por request

Tempo de execução

Mensagens de erro

Logs de console personalizados

### 🤝 Contribuições
Contribuições são muito bem-vindas! Se você deseja colaborar com melhorias, siga as etapas abaixo:

Fork o projeto.

Crie uma branch (git checkout -b minha-melhoria).

Faça suas alterações.

Submeta um Pull Request com uma descrição clara do que foi alterado.

### 📫 Suporte
Se encontrar problemas ou tiver dúvidas:

Consulte a documentação oficial do Postman

Entre em contato comigo!

### 🧠 Dica
Use variáveis dinâmicas (pm.environment.set, pm.variables.get) e scripts de pré-requisição para deixar seus testes mais inteligentes e adaptáveis a diferentes contextos (massa de dados, autenticação, endpoints parametrizados).


