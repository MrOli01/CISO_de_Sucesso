# 🗂️ Etapas para Avaliação de Riscos - ISO/IEC 27005

## 1. Definir o Contexto

- Escopo do SGSI  
- Missão e objetivos de negócio  
- Tolerância a riscos  
- Requisitos legais e regulatórios  

---

## 2. Inventário de Ativos

| Ativo              | Tipo       | Proprietário | Valor |
|--------------------|------------|--------------|-------|
| Servidor de banco  | Hardware   | Infra TI     | Alto  |
| Sistema RH         | Software   | RH           | Médio |
| Dados de clientes  | Informação | Jurídico     | Alto  |

---

## 3. Identificação de Riscos

| Ativo              | Ameaça           | Vulnerabilidade        | Consequência       |
|--------------------|------------------|------------------------|--------------------|
| Servidor de banco  | Malware          | Sistema desatualizado  | Roubo de dados     |
| Planilhas RH       | Envio acidental  | Falta de criptografia  | Vazamento de dados |

---

## 📏 Análise de Risco

### Fórmula (Risco = Probabilidade x Impacto)


---

### Matriz Qualitativa

|                     | Impacto Baixo | Impacto Médio | Impacto Alto |
|---------------------|---------------|---------------|--------------|
| Probabilidade Alta  | Médio         | Alto          | Crítico      |
| Probabilidade Média | Baixo         | Médio         | Alto         |
| Probabilidade Baixa | Aceitável     | Baixo         | Médio        |

---

## 🛠️ Tratamento de Riscos

### Estratégias de Tratamento

- **Mitigar**: Reduzir a probabilidade ou o impacto  
- **Aceitar**: Assumir o risco conscientemente  
- **Transferir**: Passar a responsabilidade (ex: seguro)  
- **Evitar**: Eliminar o risco (ex: desativar o serviço)  

---

### Exemplo de Classificação

| ID  | Descrição               | Classificação | Ação     | Justificativa              |
|-----|--------------------------|---------------|----------|----------------------------|
| R1  | Acesso não autorizado    | Crítico       | Mitigar  | Implementar MFA            |
| R2  | Vazamento por e-mail     | Alto          | Mitigar  | Restringir envio externo   |

---

## 📋 Plano de Tratamento de Riscos (PTR)

### Exemplo:

- **ID do Risco:** R1  
- **Descrição:** Acesso não autorizado ao banco de dados  
- **Probabilidade:** Alta  
- **Impacto:** Alto  
- **Classificação:** Crítico  
- **Ação:** Mitigar  
- **Controles Recomendados:** MFA, firewall, logging  
- **Prazo de Implementação:** 15 dias  

---

# Exemplo REAL

# Avaliação e Tratamento de Riscos segundo ISO/IEC 27005

## 🎯 Objetivo

Capacitar o leitor a compreender, aplicar e documentar um processo completo de avaliação e tratamento de riscos com base na ISO/IEC 27005. A abordagem será prática, com exemplos reais e estruturada como uma aula de pós-graduação.

## 🧩 Introdução

A avaliação e o tratamento de riscos fazem parte do coração de um Sistema de Gestão de Segurança da Informação (SGSI). Sem entender os riscos, não é possível proteger adequadamente os ativos da informação de uma organização.

A norma ISO/IEC 27005 fornece diretrizes para este processo, integrando os conceitos da ISO 27001 e ISO 31000.

## 🗂️ Etapas do Processo de Avaliação de Riscos

### 1. Definir o Contexto

É necessário definir o escopo e entender o ambiente onde os riscos serão avaliados:

- **Escopo do SGSI**: Ex: Toda a infraestrutura de TI da matriz e filiais.
- **Objetivos de negócio**: Ex: Garantir disponibilidade do e-commerce.
- **Tolerância a riscos**: Ex: Riscos com impacto maior que R$100 mil não são aceitáveis.
- **Requisitos legais e regulatórios**: LGPD, ISO 27001, Marco Civil da Internet, etc.

#### 👨‍💼 Exemplo realista:
João, gerente de segurança da informação, definiu que o SGSI abrangerá todos os sistemas que armazenam dados sensíveis dos clientes. A tolerância ao risco foi definida pela diretoria: qualquer evento que afete a imagem da empresa ou cause prejuízo financeiro acima de R$50 mil é inaceitável.

### 2. Inventário de Ativos

É preciso listar todos os ativos que fazem parte do escopo:

| Ativo                | Tipo      | Proprietário | Valor |
|----------------------|-----------|--------------|-------|
| Servidor de banco    | Hardware  | Infra TI     | Alto  |
| Sistema RH           | Software  | RH           | Médio |
| Dados de clientes    | Informação| Jurídico     | Alto  |

#### 🧠 Dica: 
A classificação de valor pode ser feita com base em impacto financeiro, regulatório e reputacional.

### 3. Identificação de Riscos

Aqui você cruza ameaças e vulnerabilidades para identificar possíveis cenários de risco.

| Ativo               | Ameaça          | Vulnerabilidade        | Consequência        |
|---------------------|-----------------|------------------------|---------------------|
| Servidor de banco   | Malware         | Sistema desatualizado  | Roubo de dados      |
| Planilhas RH        | Envio acidental | Falta de criptografia  | Vazamento de dados  |

#### 💡 Exemplo realista:
João identificou que o servidor de arquivos do setor financeiro estava exposto via SMB sem autenticação. Uma ameaça plausível seria o ransomware. A consequência? Inviabilização dos relatórios fiscais e multas por atraso.

### 📏 Análise de Risco

Fórmula clássica:

**Risco = Probabilidade x Impacto**

#### Matriz Qualitativa de Risco

|                      | **Impacto Baixo** | **Impacto Médio** | **Impacto Alto** |
|----------------------|-------------------|-------------------|------------------|
| **Probabilidade Alta** | Médio             | Alto              | Crítico          |
| **Probabilidade Média**| Baixo             | Médio             | Alto             |
| **Probabilidade Baixa**| Aceitável         | Baixo             | Médio            |

#### 🧠 Dica:
Você pode utilizar escalas de 1 a 5 ou escalas verbais (baixo, médio, alto) para facilitar a classificação.

### 🛠️ Tratamento de Riscos

Uma vez avaliado o risco, é necessário escolher uma estratégia de tratamento:

- **Mitigar**: Reduzir a probabilidade ou o impacto
- **Aceitar**: Assumir o risco conscientemente
- **Transferir**: Passar a responsabilidade (ex: seguro)
- **Evitar**: Eliminar a exposição ao risco (ex: desativar o serviço)

#### Exemplo de Classificação

| ID | Descrição               | Classificação | Ação     | Justificativa              |
|----|-------------------------|---------------|----------|----------------------------|
| R1 | Acesso não autorizado   | Crítico       | Mitigar  | Implementar MFA            |
| R2 | Vazamento por e-mail    | Alto          | Mitigar  | Restringir envio externo   |

#### 🧑‍💼 Exemplo Realista:
João identificou que o envio externo de planilhas sensíveis era uma falha grave. A medida tomada foi bloquear anexos de certos formatos no e-mail corporativo e treinar os usuários.

## 📋 Plano de Tratamento de Riscos (PTR)

O PTR é um documento que consolida os riscos, suas classificações e ações planejadas.

### Estrutura básica de um PTR

```markdown
# Plano de Tratamento de Riscos (PTR)

## Resumo
- **Responsável**: João Silva  
- **Data**: 15/04/2025  
- **Escopo**: Sistemas críticos de TI  

## Riscos Identificados
| ID  | Descrição              | Nível    | Ação Proposta       | Prazo   | Responsável   |
|-----|------------------------|----------|---------------------|---------|---------------|
| R1  | Acesso não autorizado  | Crítico  | Implementar MFA     | 30 dias | Segurança TI  |
| R2  | Vazamento por e-mail   | Alto     | Bloquear anexos     | 15 dias | Suporte TI    |

## Monitoramento
- Relatórios mensais
- Reavaliação semestral dos riscos
- Auditorias de conformidade
