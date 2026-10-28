# Resolução do Estudo de Caso — Conecta Campus

**Disciplina:** Engenharia de Requisitos / Análise de Sistemas  
**Aluno:** Ian Enilson dos Santos Silva  
**Data:** 28 de Outubro de 2026  

---

## 1. Concepção

* **Qual problema o Conecta Campus pretende resolver?**  
  Atualmente, a comunicação e o acesso aos serviços acadêmicos estão espalhados ou dependem de um sistema antigo que é lento e complicado de navegar. Isso gera frustração nos alunos, dificulta a rotina dos professores na hora de enviar materiais e atrapalha a coordenação na hora de divulgar avisos importantes.

* **Qual é o seu principal objetivo?**  
  O objetivo principal é criar uma plataforma única (centralizada), simples e ágil que permita a alunos, professores e coordenação acessar e gerenciar dados acadêmicos (notas, horários, comunicados e materiais) de forma segura e rápida.

---

## 2. Elicitação

* **Quem são os principais stakeholders?**
  * **Alunos:** Usuários finais que consultam notas, horários e avisos.
  * **Professores:** Usuários que postam notas, comunicados e materiais de aula.
  * **Coordenação Acadêmica:** Responsáveis por publicar eventos e comunicados gerais.
  * **Equipe de TI / Desenvolvedores:** Responsáveis por construir e manter a plataforma.
  * **Administração da Universidade:** Stakeholder institucional que exige segurança e eficiência no sistema.

* **Quais técnicas poderiam ser utilizadas para descobrir suas necessidades?**
  1. **Questionários / Formulários online:** Ótimo para aplicar com os alunos e pegar uma quantidade grande de respostas sobre dores de usabilidade e rotina.
  2. **Entrevistas semiestruturadas:** Conversar diretamente com representantes da coordenação e alguns professores para entender o fluxo de publicação de notas e conteúdos.
  3. **Workshops de Requisitos / Reuniões em grupo:** Reuniões rápidas de alinhamento entre a equipe de desenvolvimento e os professores/coordenação para priorizar o que entra na primeira versão.
  4. **Observação:** Acompanhar um professor tentando postar um material no sistema atual para ver na prática onde estão os gargalos.

---

## 3. Análise / Modelagem

### Requisitos Funcionais (RF)
* **RF01:** O sistema deve permitir que os alunos visualizem suas notas e médias por disciplina.
* **RF02:** O sistema deve permitir que os alunos consultem a grade horária das aulas.
* **RF03:** O sistema deve permitir que os professores publiquem materiais didáticos (PDFs, links, etc.).
* **RF04:** O sistema deve permitir que professores e coordenação enviem avisos/comunicados para turmas específicas ou para toda a instituição.
* **RF05:** O sistema deve exigir autenticação (login e senha) para conceder acesso às informações acadêmicas.
* **RF06 (Bônus):** O sistema deve permitir que a coordenação cadastre e divulgue eventos acadêmicos na plataforma.

### Requisitos Não Funcionais (RNF)
* **RNF01 (Desempenho):** As páginas de consulta devem carregar em no máximo 2 segundos sob condições normais de rede.
* **RNF02 (Usabilidade):** O sistema deve ter uma interface responsiva e permitir que o aluno encontre suas notas em até 3 cliques a partir da tela inicial.
* **RNF03 (Segurança):** O sistema deve criptografar senhas no banco de dados e encerrar a sessão do usuário após 15 minutos de inatividade.

---

## 4. Negociação (Matriz MoSCoW)

* **Must Have (Indispensável para o MVP / Lançamento):**
  * Autenticação e login seguro de usuários.
  * Consulta de notas e frequências pelos alunos.
  * Visualização da grade horária pelos alunos.
  * Publicação de materiais e avisos por parte dos professores.
  * Divulgação de comunicados e eventos pela coordenação.

* **Should Have (Importante, mas dá para lançar sem se o prazo apertar):**
  * Notificações *push* no celular ou aviso por e-mail quando uma nota/material for publicado.
  * Filtro de busca para materiais e comunicados antigos.

* **Could Have (Desejável para versões futuras):**
  * Modo escuro na interface.
  * Integração com calendário pessoal (ex: Google Agenda) para salvar horários de aula e eventos.

* **Won't Have (Fora do escopo da primeira versão):**
  * Chat em tempo real entre alunos e professores (descartado no MVP para não atrasar a entrega inicial, conforme decidido pela equipe).

---

## 5. Especificação

Transformando termos genéricos em requisitos mensuráveis:

* **Vago:** "O aplicativo deve ser rápido."  
  * **Especificado:** "O tempo de resposta do sistema para o carregamento da tela de notas e horários não deve ultrapassar 2 segundos para 95% das requisições simultâneas."


* **Vago:** "O aplicativo deve ser fácil de usar."  
  * **Especificado:** "Um usuário novo (aluno ou professor) deve ser capaz de realizar a consulta de notas ou publicação de um aviso em no máximo 3 cliques sem necessidade de treinamento prévio, alcançando taxa de sucesso de pelo menos 90% em testes de usabilidade."

---

## 6. Validação

Para garantir que o levantamento reflete o que os usuários realmente precisam, a equipe pode adotar as seguintes estratégias:

1. **Protótipos de AltaFidelidade:** Montar telas navegáveis da aplicação e apresentar para grupos de alunos, professores e coordenação. Pedir para eles executarem tarefas simples e coletar feedback.
2. **Reunião de Homologação dos Requisitos:** Apresentar a documentação refinada para os representantes da coordenação e professores, revisando item por item para aprovação formal.
3. **Testes :** Liberar uma versão *Beta* para um pequeno grupo de alunos e professores testarem por uma semana antes do lançamento oficial para a universidade inteira.
