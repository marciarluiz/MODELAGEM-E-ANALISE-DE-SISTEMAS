- Concepção: Qual problema o Conecta Campus pretende resolver e qual é seu principal objetivo?

__RESPOSTA:__
O problema que o Conecta Campus se propõe a resolver é a solução dos problemas do sistema/software anterior, tendo como objetivo acabar com problemas posteriores como a lentidão e dificuldade de usar, além de implementações novas como autenticação de usuário e inclusão de chat para comunicação entre professores e alunos.

- Elicitação: Quem são os principais stakeholders? Quais técnicas poderiam ser utilizadas para descobrir suas necessidades?

__RESPOSTA:__
As principais partes interessadas são os alunos, os professores e a parte administrativa da universidade, para descobrir as necessidades reais deles seria através de entrevistas com as partes que realmente vão usar o sistema, além da entrevista também poderiamos utilizar: questionários, observação, workshops, análise de documentos e protótipos.

- Análise/Modelagem: Identifique pelo menos 5 requisitos funcionais e 3 requisitos não funcionais.

__RESPOSTAS:__
RF1. Cadastrar alunos e professores para autenticação.
RF2. Consultar dados dos alunos/notas.
RF3. Divulgação de eventos e informações acadêmicas/avisos.
RF4. Chat entre professores e alunos.
RF5. Publicação de materiais de aula.

RNF1. Deixar o sistema mais rápido.
RNF2. Proteger as contas dos usuários com autenticação de multifator.
RNF3. Usabilidade do sistema.

- Negociação: Classifique as funcionalidades utilizando MoSCoW — Must, Should, Could e Won't.

__RESPOSTAS:__
RF1 - Must
RF5 - Must
RF2 - Should
RF3 - Should
RF4 - Won't

RNF1- Could
RNF2- Should
RNF3- Could

- Especificação: Transforme frases vagas, como “O aplicativo deve ser rápido, seguro e fácil de usar”, em requisitos claros e verificáveis.

__RESPOSTA:__
O aplicativo deverá ter tempo de resposta para os usuários em até 3 segundos, além de ter uma autenticação em multifator e uma interface amigável com os usuários.

- Validação: Como a equipe poderia confirmar com alunos, professores e coordenação que os requisitos levantados estão corretos?

__RESPOSTA:__
Utilizando a User Story, que é uma forma de confirmar com a parte interessada o que realmente interessa para o sistema, além de perguntas para validação como: "É isso mesmo que vocês precisam?", "Está faltando alguma funcionalidade?" "Existe alguma informação incorreta?" "Esse requisito pode ser testado?"


**Uma clínica veterinária deseja desenvolver o PetCare, um sistema para melhorar o atendimento aos animais e organizar as informações dos clientes.**

Atualmente, os agendamentos são realizados por telefone e WhatsApp. O histórico dos animais fica armazenado em fichas e arquivos separados, o que dificulta encontrar rapidamente informações sobre consultas anteriores, vacinas e medicamentos. Os tutores dos animais querem marcar consultas pelo celular e receber lembretes de vacinação. Os veterinários querem consultar o histórico do animal e registrar diagnóstico, tratamento e medicamentos. A recepção precisa controlar os horários disponíveis e confirmar ou cancelar consultas. O gerente gostaria de visualizar relatórios sobre quantidade de atendimentos realizados.
Durante a reunião, surgiram também algumas solicitações: permitir pagamento pelo aplicativo, disponibilizar chat com o veterinário e criar uma área para publicação de fotos dos animais. O proprietário afirmou que o sistema deve ser “rápido, seguro e muito fácil de usar” e quer uma primeira versão funcionando em quatro meses.

**Imagine que sua equipe foi contratada para realizar a Engenharia de Requisitos do PetCare.**
Identifique os stakeholders e explique quais técnicas utilizaria para realizar a elicitação. Determine pelo menos 5 requisitos funcionais e 3 requisitos não funcionais. Classifique as funcionalidades utilizando MoSCoW (Must, Should, Could e Won't) e Transforme a frase “O sistema deve ser rápido, seguro e muito fácil de usar” em requisitos que possam ser medidos e testados. Explique como sua equipe faria a validação dos requisitos antes de iniciar o desenvolvimento. Desafio: o proprietário informa que só existe orçamento para desenvolver cinco funcionalidades na primeira versão. Quais você escolheria e por quê?

__RESPOSTAS:__

As partes intreressadas são os trabalhadores da PetCare, como a recepcionista, o cuidador, o tosador, a parte administrativa e os tutores dos pets. 

Utilizaria como elicitação as técnicas de entrevistas, observação, questionário e protótipos. 

Os 5 requisitos funcionais e não funcionais que escolhi são:
RF1. Cadastro do tutor e pet. MUST
RF2. Colsuta sobre os dados do pet no próprio aplicativo. COULD
RF3. Consulta de horários. MUST
RF4. Pagamento pelo aplicativo. SHOULD
RF5. Relatório sobre quantidade de atendimentos realizados. SHOULD

RFN1. O sistema deve ser rápido, seguro e de fácil uso. WON'T
RNF2. Área pra foto do pet. WON'T
RNF3. Chat com veterinário. WON'T

O sistema deve ter tempo de resposta para os usuários em até 5 segundos, ter uma criptografia de dados e autenticação de multifator para os usuários e a usabilidade do sistema deve ser amigável feita pra experiência do usuário.

Minha equipe faria a validação com as perguntas básicas "É isso mesmo que vocês precisam?", "Está faltando alguma funcionalidade?" "Existe alguma informação incorreta?" "Esse requisito pode ser testado?" e também usariamos User Story para facilitar no desenvolvimento do programa.

__Resposta do desafio:__
Eu manteria as funcionalidades RF1, RF2, RF3, RF4 e RF5, pois elas são essenciais para o funcionamento do sistema num todo, com todo o básico, porém, essencial sendo feito. Como o cadastro de pet e tutor, os dados do pet fáceis no aplicativo para facilitar próximos agendamentos para o tutor, além de poder ver as medicações e vacinas do seu pet. A consulta de horários disponíveis para a parte da recepção, assim facilitando a captação de clientes, pagamento pelo aplicativo para facilitar/agilizar o atendimento no PetCare, onde você já poderia deixar pago e apenas deixar o seu pet sob cuidados dos cuidadores. E por fim o relátorio sobre os atendimentos para ajudar o gerente a desenvolver planos futuros a partir desses dados gerados.