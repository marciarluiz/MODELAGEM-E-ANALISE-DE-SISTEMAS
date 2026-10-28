# Resolução do Estudo de Caso — Sistema PetCare

**Disciplina:** Engenharia de Requisitos / Análise de Sistemas  
**Aluno:** Ian Enilson dos Santos Silva 
**Data:** 28 de Outubro de 2026  

---

## 1. Identificação de Stakeholders e Técnicas de Elicitação

### Stakeholders
* **Tutores dos Animais (Clientes):** Querem facilidade para agendar consultas e acompanhar a rotina de vacinas.
* **Veterinários:** Precisam acessar rapidamente o histórico médico e registrar novos atendimentos de forma prática.
* **Recepcionistas:** Precisam gerenciar a agenda diária, confirmando e desmarcando horários sem conflitos.
* **Gerente / Proprietário da Clínica:** Busca relatórios para acompanhamento do negócio e quer a entrega do sistema no prazo de 4 meses.

### Técnicas de Elicitação
1. **Entrevistas Individuais:** Conversas diretas com veterinários, recepcionistas e o gerente para entender em detalhes como funciona a rotina da clínica e onde estão os gargalos do papel e do WhatsApp.
2. **Questionário Online:** Formulário enviado aos tutores cadastrados para mapear preferências de agendamento e o uso de celulares.
3. **Análise de Documentos:** Análise das fichas físicas, carteiras de vacinação atuais e planilhas usadas na recepção para entender as informações que precisam ser digitalizadas.
4. **Análise de Tarefas:** Acompanhar o passo a passo da recepção ao marcar uma consulta e o tempo que um veterinário leva procurando fichas de papel.

---

## 2. Requisitos Funcionais e Não Funcionais

### Requisitos Funcionais (RF)
* **RF01 (Agendamento):** O sistema deve permitir que os tutores solicitem agendamentos de consultas escolhendo data, horário e veterinário disponível.
* **RF02 (Gestão da Agenda):** O sistema deve permitir que a recepção visualize, confirme ou cancele consultas agendadas.
* **RF03 (Prontuário Eletrônico):** O sistema deve permitir que o veterinário registre diagnósticos, tratamentos, prescrições e vacinas aplicadas no perfil do animal.
* **RF04 (Histórico do Animal):** O sistema deve permitir a consulta do histórico médico completo do animal antes ou durante a consulta.
* **RF05 (Lembretes Automáticos):** O sistema deve enviar avisos e lembretes sobre vacinas e consultas aos tutores (por e-mail, SMS ou notificação no aplicativo).
* **RF06 (Relatórios Gerenciais):** O sistema deve gerar relatórios com a quantidade e o tipo de atendimentos realizados em um determinado período.

### Requisitos Não Funcionais (RNF)
* **RNF01 (Desempenho):** A busca por qualquer histórico do animal deve ser concluída e exibida na tela em no máximo 2 segundos.
* **RNF02 (Usabilidade):** A interface deve ser simples para que um tutor consiga agendar uma consulta em até 3 passos a partir da tela inicial.
* **RNF03 (Segurança):** O sistema deve restringir o acesso às fichas médicas apenas a usuários autenticados e criptografar as senhas no banco de dados.

---

## 3. Classificação das Funcionalidades (MoSCoW)

* **Must Have (Obrigatório para o sistema funcionar):**
  * Cadastro de tutores, animais e veterinários.
  * Agendamento e cancelamento de consultas.
  * Prontuário eletrônico para registro de diagnósticos, vacinas e tratamentos.
  * Login e controle de acesso por perfil de usuário.

* **Should Have (Muito importante, mas não impede a abertura do sistema):**
  * Lembretes automáticos de vacinação e consultas para os tutores.
  * Relatórios de quantidade de atendimentos para o gerente.

* **Could Have (Desejável para próximas atualizações):**
  * Pagamento das consultas diretamente pelo aplicativo.
  * Notificações *push* customizadas na tela do celular.

* **Won't Have (Fora do escopo para a entrega em 4 meses):**
  * Chat em tempo real entre tutor e veterinário (exige acompanhamento constante e pode atrasar o projeto).
  * Feed/Área para publicação de fotos dos animais (não agrega valor direto ao atendimento clínico inicial).

---

## 4. Especificação de Requisitos Limpos e MENSURÁVEIS

Transformando frases subjetivas em critérios testáveis:

* **Em vez de "O sistema deve ser rápido":**
  * *Requisito:* "O sistema deve processar a confirmação de agendamento e a abertura de prontuários em no máximo 2 segundos sob conexão padrão de internet."


* **Em vez de "O sistema deve ser muito fácil de usar":**
  * *Requisito:* "Um tutor novo deve conseguir concluir o agendamento de uma consulta em menos de 2 minutos no primeiro acesso, sem necessitar de suporte ou instrução prévia."

---

## 5. Validação dos Requisitos

Para confirmar que os requisitos atendem ao que a clínica e os clientes realmente precisam antes de começar a codificar, serão adotadas as seguintes estratégias:

1. **Protótipos de Tela:** Apresentar a navegação visual das telas para o proprietário, recepcionistas e veterinários, simulação passo a passo dos agendamentos e cadastros para checar a usabilidade.
2. **Revisão da Documentação:** Fazer uma leitura acompanhada do documento de requisitos com o gerente e com a equipe médica para ajustar termos técnicos ou faltas de informação.
3. **Listas de Verificação:** Avaliar se cada requisito listado é realmente necessário, viável em 4 meses e se pode ser testado após a construção.

---

## 6. Escolha das 5 Funcionalidades Essenciais para o MVP (Prazo de 4 Meses e Orçamento Limitado)

Caso seja necessário escolher estritamente **5 funcionalidades principais** para a primeira versão, a seleção priorizará o fluxo completo de atendimento e operação da clínica:

1. **Cadastro de Tutores e Animais:** Base indispensável para vincular os pet aos donos e organizar as fichas.
2. **Agendamento e Controle de Consultas (Tutor e Recepção):** Resolve a dor central de organizar a agenda, acabando com a dependência exclusiva do papel e do WhatsApp.
3. **Prontuário Eletrônico e Registro de Vacinas:** Substitui as fichas físicas, permitindo que o veterinário registre diagnósticos, receitas e vacinas em um só lugar.
4. **Consulta do Histórico Médico do Animal:** Permite ao veterinário acessar rapidamente dados de consultas anteriores, melhorando a velocidade e a qualidade do atendimento.
5. **Envio de Lembretes Automáticos de Vacinas/Consultas:** Garante o retorno dos clientes e reduz a taxa de esquecimento, trazendo retorno financeiro direto para a clínica.

### Justificativa da Escolha:
Com essas 5 funcionalidades, o PetCare resolve 100% dos problemas operacionais prioritários: agendamento, organização do atendimento médico, fim do papel e fidelização dos clientes. Recursos como relatórios, pagamentos no app e chat podem ser adicionados em versões futuras assim que a clínica levantar novo orçamento.
