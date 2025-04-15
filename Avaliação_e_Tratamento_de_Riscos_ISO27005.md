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
