# Modelo de Dados — SharePoint Lists

Este documento descreve a estrutura de dados do sistema OPS Manager.

---

## 1. Atividades_Base

| Campo              | Tipo        | Descrição                                  |
| ------------------ | ----------- | ------------------------------------------ |
| Titulo             | Texto       | Nome da atividade                          |
| Prioridade         | Escolha     | CRÍTICO / IMPORTANTE / NECESSÁRIO          |
| Frequencia_Semanal | Número      | Quantidade de execuções por semana (1 a 5) |
| Ativo              | Sim/Não     | Indica se a atividade está ativa           |
| Descricao          | Texto longo | Detalhes da atividade                      |

---

## 2. Agenda_Diaria

| Campo      | Tipo        | Descrição                                |
| ---------- | ----------- | ---------------------------------------- |
| Titulo     | Texto       | Nome da atividade                        |
| Data       | Data        | Data da execução                         |
| Prioridade | Escolha     | Nível da atividade                       |
| Status     | Escolha     | Não realizada / Em andamento / Concluída |
| Origem     | Escolha     | Recorrente / Pendência / Email / Manual  |
| ID_Origem  | Número      | Referência do item de origem             |
| Observacao | Texto longo | Notas adicionais                         |

---

## 3. Pendencias

| Campo        | Tipo        | Descrição              |
| ------------ | ----------- | ---------------------- |
| Titulo       | Texto       | Descrição da pendência |
| Prioridade   | Escolha     | Nível da atividade     |
| Status       | Escolha     | Status atual           |
| Data_Criacao | Data        | Data de criação        |
| Observacao   | Texto longo | Detalhes               |

---

## 4. Fechamentos

| Campo      | Tipo        | Descrição         |
| ---------- | ----------- | ----------------- |
| Titulo     | Texto       | Nome da atividade |
| Mes        | Texto       | Mês de referência |
| Ano        | Número      | Ano               |
| Prioridade | Escolha     | Nível             |
| Status     | Escolha     | Status            |
| Observacao | Texto longo | Detalhes          |

---

## 5. Desenvolvimentos

| Campo         | Tipo        | Descrição         |
| ------------- | ----------- | ----------------- |
| Titulo        | Texto       | Nome do projeto   |
| Resumo        | Texto       | Breve descrição   |
| Descricao     | Texto longo | Detalhamento      |
| Status        | Escolha     | Status do projeto |
| Prioridade    | Escolha     | Nível             |
| Data_Inicio   | Data        | Início            |
| Data_Prevista | Data        | Previsão          |
| Impedimentos  | Texto longo | Bloqueios         |

---

## 6. Manutencao_Moldes

| Campo         | Tipo        | Descrição         |
| ------------- | ----------- | ----------------- |
| Titulo        | Texto       | Nome              |
| Equipamento   | Texto       | Equipamento/molde |
| Status        | Escolha     | Status            |
| Prioridade    | Escolha     | Nível             |
| Data_Prevista | Data        | Previsão          |
| Observacao    | Texto longo | Detalhes          |

---

## 7. Indicadores

| Campo          | Tipo        | Descrição        |
| -------------- | ----------- | ---------------- |
| Data           | Data        | Data do registro |
| Nome_Indicador | Texto       | Nome             |
| Valor          | Número      | Valor registrado |
| Observacao     | Texto longo | Notas            |

---

## 8. Materias_Pos

| Campo       | Tipo        | Descrição                |
| ----------- | ----------- | ------------------------ |
| Titulo      | Texto       | Nome da matéria          |
| Data_Inicio | Data        | Início                   |
| Data_Fim    | Data        | Fim                      |
| Nota_Final  | Número      | Nota                     |
| Status      | Escolha     | Em andamento / Concluída |
| Observacao  | Texto longo | Detalhes                 |

---

## 9. Atividades_Academicas

| Campo        | Tipo        | Descrição                    |
| ------------ | ----------- | ---------------------------- |
| Titulo       | Texto       | Nome                         |
| Materia      | Lookup      | Referência para Materias_Pos |
| Data_Entrega | Data        | Prazo                        |
| Status       | Escolha     | Status                       |
| Observacao   | Texto longo | Detalhes                     |

---

## 10. Portfolio

| Campo       | Tipo        | Descrição                   |
| ----------- | ----------- | --------------------------- |
| Titulo      | Texto       | Nome do projeto             |
| Tipo        | Escolha     | Trabalho / Pessoal / Estudo |
| Descricao   | Texto longo | Detalhes                    |
| Link_GitHub | Link        | URL do projeto              |
| Status      | Escolha     | Status                      |
| Data        | Data        | Registro                    |

---

## 11. Ideias_Insights

| Campo     | Tipo        | Descrição                   |
| --------- | ----------- | --------------------------- |
| Titulo    | Texto       | Nome                        |
| Descricao | Texto longo | Conteúdo                    |
| Categoria | Escolha     | Trabalho / Estudo / Pessoal |
| Data      | Data        | Registro                    |

---

## 12. Controle_Ingles

| Campo      | Tipo        | Descrição                         |
| ---------- | ----------- | --------------------------------- |
| Data       | Data        | Registro                          |
| Tipo       | Escolha     | Aula / Estudo                     |
| Horas      | Número      | Quantidade                        |
| Nivel      | Escolha     | Básico / Intermediário / Avançado |
| Observacao | Texto longo | Notas                             |

---
