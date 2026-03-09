# 🔐 DevSecOps Security Pipeline

Este repositório demonstra a implementação de uma **pipeline DevSecOps** utilizando **GitHub Actions** para automatizar testes de segurança durante o processo de desenvolvimento.

A pipeline executa automaticamente verificações de segurança sempre que ocorre um **push** ou **pull request**, permitindo identificar vulnerabilidades antes que o código seja implantado em produção.

---

# 📌 Objetivo

O objetivo deste projeto é demonstrar como integrar práticas de **segurança no ciclo de desenvolvimento de software (DevSecOps)**.

A pipeline busca:

- Detectar vulnerabilidades no código-fonte
- Identificar bibliotecas vulneráveis
- Executar testes de segurança automatizados
- Melhorar a qualidade e segurança do software

---

# 🛠️ Ferramentas Utilizadas

## 🔎 SAST – Static Application Security Testing

Ferramenta utilizada:

**Semgrep**

O Semgrep realiza análise estática do código-fonte, identificando padrões que podem indicar vulnerabilidades de segurança.

### Exemplos de vulnerabilidades detectadas

- SQL Injection
- Cross-Site Scripting (XSS)
- Uso inseguro de funções
- Falta de validação de entrada

Essa análise ocorre sem a necessidade de executar a aplicação.

---

## 📦 SCA – Software Composition Analysis

Ferramenta utilizada:

**Snyk**

O Snyk analisa as dependências utilizadas pelo projeto e compara com bases de dados de vulnerabilidades conhecidas (CVE).

### Problemas identificados

- bibliotecas vulneráveis
- versões inseguras de frameworks
- dependências desatualizadas

Esse tipo de análise é importante para reduzir riscos na **cadeia de suprimentos de software (Software Supply Chain).**

---

## 🌐 DAST – Dynamic Application Security Testing

Ferramenta utilizada:

**OWASP ZAP**

O OWASP ZAP realiza testes de segurança com a aplicação em execução.

### Exemplos de testes realizados

- análise de headers HTTP
- verificação de configurações inseguras
- identificação de vulnerabilidades web

---

# ⚙️ Funcionamento da Pipeline

A pipeline é executada automaticamente nas seguintes situações:


# 🔐 DevSecOps Security Pipeline

Este repositório demonstra a implementação de uma **pipeline DevSecOps** utilizando **GitHub Actions** para automatizar testes de segurança durante o processo de desenvolvimento.

A pipeline executa automaticamente verificações de segurança sempre que ocorre um **push** ou **pull request**, permitindo identificar vulnerabilidades antes que o código seja implantado em produção.

---

# 📌 Objetivo

O objetivo deste projeto é demonstrar como integrar práticas de **segurança no ciclo de desenvolvimento de software (DevSecOps)**.

A pipeline busca:

- Detectar vulnerabilidades no código-fonte
- Identificar bibliotecas vulneráveis
- Executar testes de segurança automatizados
- Melhorar a qualidade e segurança do software

---

# 🛠️ Ferramentas Utilizadas

## 🔎 SAST – Static Application Security Testing

Ferramenta utilizada:

**Semgrep**

O Semgrep realiza análise estática do código-fonte, identificando padrões que podem indicar vulnerabilidades de segurança.

### Exemplos de vulnerabilidades detectadas

- SQL Injection
- Cross-Site Scripting (XSS)
- Uso inseguro de funções
- Falta de validação de entrada

Essa análise ocorre sem a necessidade de executar a aplicação.

---

## 📦 SCA – Software Composition Analysis

Ferramenta utilizada:

**Snyk**

O Snyk analisa as dependências utilizadas pelo projeto e compara com bases de dados de vulnerabilidades conhecidas (CVE).

### Problemas identificados

- bibliotecas vulneráveis
- versões inseguras de frameworks
- dependências desatualizadas

Esse tipo de análise é importante para reduzir riscos na **cadeia de suprimentos de software (Software Supply Chain).**

---

## 🌐 DAST – Dynamic Application Security Testing

Ferramenta utilizada:

**OWASP ZAP**

O OWASP ZAP realiza testes de segurança com a aplicação em execução.

### Exemplos de testes realizados

- análise de headers HTTP
- verificação de configurações inseguras
- identificação de vulnerabilidades web

---

# ⚙️ Funcionamento da Pipeline

A pipeline é executada automaticamente nas seguintes situações:



---

# 🔄 Etapas da Pipeline

### 1️⃣ Checkout do código

O pipeline obtém a versão mais recente do código no repositório.

---

### 2️⃣ Análise de código (SAST)

O **Semgrep** executa análise estática buscando vulnerabilidades no código-fonte.

---

### 3️⃣ Análise de dependências (SCA)

O **Snyk** verifica se bibliotecas do projeto possuem vulnerabilidades conhecidas.

---

### 4️⃣ Inicialização da aplicação

A aplicação é iniciada utilizando **Docker Compose** para permitir testes dinâmicos.

---

### 5️⃣ Testes dinâmicos de segurança (DAST)

O **OWASP ZAP** executa testes de segurança na aplicação em execução.

---

# 📂 Estrutura do Projeto



O arquivo **security-pipeline.yml** contém a configuração da pipeline executada pelo GitHub Actions.

---

# 🚀 Benefícios da Pipeline

A integração dessas ferramentas proporciona:

- Identificação precoce de vulnerabilidades
- Automação de testes de segurança
- Redução de riscos de segurança
- Implementação de práticas DevSecOps
- Melhoria contínua da qualidade do código

---

# 🧠 Conclusão

A integração de ferramentas de segurança em pipelines CI/CD permite que vulnerabilidades sejam detectadas e corrigidas durante o desenvolvimento.

Ao combinar:

- **SAST**
- **SCA**
- **DAST**

é possível implementar uma abordagem mais completa para segurança de aplicações e promover o desenvolvimento de software mais seguro.

---

# 👨‍💻 Autor

Projeto desenvolvido para demonstrar práticas de **DevSecOps e Segurança de Aplicações** utilizando GitHub Actions.