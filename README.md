# SM7---Engenharia-de-Software-e-IA-com-Bubble.io
link :https://projeto-engenharia.bubbleapps.io/version-test?debug_mode=true
Para documentar essa atividade de **Engenharia de Software em Low-Code** no seu GitHub, preparei um resumo estruturado que destaca o seu rigor técnico e a aplicação de boas práticas, indo além do simples uso da ferramenta.

---

# 🚀 Laboratório: Engenharia de Software com Bubble.io

Este projeto demonstra o ciclo completo de desenvolvimento de uma aplicação web de gestão, utilizando a Inteligência Artificial do **Bubble.io** como acelerador, mas aplicando rigorosos fundamentos de **segurança, escalabilidade e governança**.

## 📑 Resumo da Execução

O projeto seguiu um pipeline profissional de engenharia, dividido em 8 etapas críticas:

### 1. Análise Crítica e Planejamento
Antes da implementação, foi realizada uma auditoria sobre as limitações da IA. [cite_start]Compreendendo que a IA gera apenas um "rascunho", o foco do desenvolvedor foi atuar onde a automação falha: **lógica de permissão e refinamento de UX**[cite: 7].

### 2. Arquitetura de Dados (Pre-Build)
A modelagem foi feita fora da ferramenta para evitar *hardcoding*:
* [cite_start]**Mapeamento de Entidades:** Definição de Data Types (Usuário, Cliente, Orçamento)[cite: 7].
* [cite_start]**Otimização de Relações:** Uso de campos de referência em vez de listas extensas para garantir performance[cite: 7].
* [cite_start]**Option Sets:** Padronização de status (Ex: Pendente, Aprovado) para evitar erros sintáticos[cite: 7].

### 3. Desenvolvimento Assistido por IA & Refatoração
Utilizou-se o **Bubble AI** para gerar o blueprint inicial. [cite_start]A intervenção humana foi aplicada na **Refatoração Front-end** (ajustes de Flexbox e responsividade) e na substituição de lógicas "chumbadas" por fluxos dinâmicos[cite: 7].

### 4. Segurança (Privacy by Design)
A etapa mais crítica do projeto. Foram removidas as permissões públicas padrão da IA e implementadas **Regras de Privacidade Estritas**:
* **Regra:** `This Data's Creator is Current User`.
* [cite_start]**Objetivo:** Prevenir vazamento de dados e garantir que um usuário não acesse informações de outro, mitigando vulnerabilidades do **OWASP Top Ten** para LCNC[cite: 7].

### 5. Governança e Performance
* [cite_start]**Otimização de WUs:** As buscas (Search) foram concentradas em *Repeating Groups* para evitar consumo excessivo de unidades de carga de trabalho[cite: 7].
* [cite_start]**Documentação In-Platform:** Workflows organizados por cores e comentados via *Notes*, garantindo que o projeto não seja uma "caixa preta"[cite: 7].

---

## 🛠️ Entregáveis do Projeto

* **[Link do Aplicativo](https://projeto-engenharia.bubbleapps.io/version-test):** Protótipo funcional com isolamento de dados.
* **[Rascunho do Banco de Dados]:** Planejamento de tabelas e Option Sets.
* **[Evidências de Segurança]:** Prints das abas de *Privacy* e *Workflows* comentados.

---

## 🚪 Estratégia de Saída (Vendor Lock-in)

Como o Bubble retém o código-fonte, a estratégia de mitigação para **Vendor Lock-in** consiste em:
1.  **Exportação via JSON:** Habilitação da **Data API** para extração em massa das tabelas de dados.
2.  [cite_start]**Portabilidade:** Plano de reescrita em stack tradicional (React/Node.js), utilizando o mapeamento de entidades já documentado neste laboratório como guia de migração[cite: 7].

---
*Projeto realizado para a disciplina de Análise e Desenvolvimento de Sistemas - 2026.*
