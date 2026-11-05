Aluno - Davi Marinho Donato
Curso - Análise e Desenvolvimento de Sistemas
Professora - Marcia Ramos Luiz

Atividade 1

Estudo de caso — Conecta Campus

Uma universidade quer centralizar seus serviços acadêmicos.

Durante uma reunião inicial, foram levantadas as seguintes necessidades: Os alunos querem consultar notas, horários e receber avisos. Os professores querem publicar materiais e comunicados. A coordenação quer divulgar eventos e informações acadêmicas. Os alunos reclamam que o sistema atual é lento e difícil de usar. A universidade exige que informações acadêmicas sejam acessadas somente por usuários autenticados. Alguns professores querem incluir chat entre alunos e professores, mas a equipe acredita que isso pode atrasar a primeira versão.

Concepção: Qual problema o Conecta Campus pretende resolver e qual é seu principal objetivo?
Elicitação: Quem são os principais stakeholders? Quais técnicas poderiam ser utilizadas para descobrir suas necessidades?
Análise/Modelagem: Identifique pelo menos 5 requisitos funcionais e 3 requisitos não funcionais.
Negociação: Classifique as funcionalidades utilizando MoSCoW — Must, Should, Could e Won't.
Especificação: Transforme frases vagas, como “O aplicativo deve ser rápido, seguro e fácil de usar”, em requisitos claros e verificáveis.
Validação: Como a equipe poderia confirmar com alunos, professores e coordenação que os requisitos levantados estão corretos?

Uma clínica veterinária deseja desenvolver o PetCare, um sistema para melhorar o atendimento aos animais e organizar as informações dos clientes.

Atualmente, os agendamentos são realizados por telefone e WhatsApp. O histórico dos animais fica armazenado em fichas e arquivos separados, o que dificulta encontrar rapidamente informações sobre consultas anteriores, vacinas e medicamentos. Os tutores dos animais querem marcar consultas pelo celular e receber lembretes de vacinação. Os veterinários querem consultar o histórico do animal e registrar diagnóstico, tratamento e medicamentos. A recepção precisa controlar os horários disponíveis e confirmar ou cancelar consultas. O gerente gostaria de visualizar relatórios sobre quantidade de atendimentos realizados. Durante a reunião, surgiram também algumas solicitações: permitir pagamento pelo aplicativo, disponibilizar chat com o veterinário e criar uma área para publicação de fotos dos animais. O proprietário afirmou que o sistema deve ser “rápido, seguro e muito fácil de usar” e quer uma primeira versão funcionando em quatro meses.

Imagine que sua equipe foi contratada para realizar a Engenharia de Requisitos do PetCare. Identifique os stakeholders e explique quais técnicas utilizaria para realizar a elicitação. Determine pelo menos 5 requisitos funcionais e 3 requisitos não funcionais. Classifique as funcionalidades utilizando MoSCoW (Must, Should, Could e Won't) e Transforme a frase “O sistema deve ser rápido, seguro e muito fácil de usar” em requisitos que possam ser medidos e testados. Explique como sua equipe faria a validação dos requisitos antes de iniciar o desenvolvimento. Desafio: o proprietário informa que só existe orçamento para desenvolver cinco funcionalidades na primeira versão. Quais você escolheria e por quê?

Respostas caso 1

Concepção: O programa Conecta Campus tem como principal objetivo resolver os problemas demandados pelos alunos, docentes e Administradores funcionando como um sistema de gestão academica 

Elicitação: Os principais stakeholders são: Alunos, Docentes, e administradores. Poderia ser feito entrevistas com alunos e docentes veteranos, também por meio de questionários e Reunião com docentes.

Análise/Modelagem:
    RF01 Registro e Login(Registro feito pela administração)
    RF02 Consulta de boletim 
    RF03 consulta de horarios de aula 
    RF04 sistema de notificações 
    RF05 postagem de materiais da aula
    RNF01 Desempenho tentando manter o site o mais rapido possivel
    RNF02 Interface limpa e facil de utilizar 
    RNF03 segurança pra evitar vazamento e roubo de dados sensiveis.

Negociação: 
MUST HAVE:
• Autenticação de usuários e controle de acesso
• Consulta de notas e horários (Alunos)
• Publicação de comunicados/avisos (Professores)

SHOULD HAVE:
• Publicação e download de materiais didáticos (Professores)
• Divulgação de eventos e informações acadêmicas (Coordenação)

COULD HAVE:
• Notificações push e por e-mail em tempo real a cada novo aviso ou nota lançada
• Exportação da grade de horários para agenda do celular

WON´T HAVE:

• Chat em tempo real entre alunos e professores

Especifição:
Rapido: O sistema deve carregar a tela de consulta em até 2 segundos ou menos na maioria dos casos, suportando até 1000 usuarios simultaneos

facil de usar: Pelo menos a maioria dos professores e alunos devem publicar uma nota ou um aviso em até 3 cliques sem necessidade de treinamento previo

seguro: o sistema deve trafegar dados exclusivamente sobre protocolo HTTPS(TLS 1.3) Armazenar senhas com hash bycrypt, exigir autenticação JWT para todas as rotas privadas e encerrar sessões inativas por 15 min

Validação:
Com um prototipo do sistema, dessa forma o prototipo pode ser levado para alunos e professores fazerem testes e dar feedbacks.

Respostas caso 2

Principais Stakeholders:
    Proprietario da clinica, Medicos(as) veterinarios, atendentes, clientes, equipe de desenvolvimento

Tecnica de elicitação:
Observação direta:Dessa forma a equipe acompanha um turno de trabalho na recepção e nos consultorios para entender na pratica como funciona a gestão.

Analise e modelagem:
RF01: Prontuario eletronico do animal
RF02: Gestão de agenda pela recepção 
RF03: Agendamento online pelo Tutor
RF04: Envio de lembretes de vacinação e consultas
RF05: Emissão de relatorios gerenciais

RNF01: Restrição de prazo
RNF02: Segurança e privacidade(LGPD)
RNF03: Multiplataforma

negociação:
MUST HAVE:
• Prontuário eletrônico unificado (histórico, diagnóstico, vacinas, medicamentos)
• Gestão de horários, confirmação e cancelamento (Recepção)
• Agendamento de consultas pelo celular (Tutor)

SHOULD HAVE:

• Lembretes automáticos de vacinação para os tutores
• Relatórios gerenciais sobre quantidade de atendimentos (Gerente)

COULD HAVE:
• Pagamento pelo aplicativo

Won´t have:
• Chat com o veterinário
• Área para publicação de fotos dos animais

Especificações:
Rapido: O sistema deve exibir o histórico clínico completo de um animal em no máximo 1,5 segundo após a busca pelo CPF do tutor ou nome do pet

seguro: O sistema deve exigir autenticação individual com senha criptografada, aplicar controle de acesso baseado em perfil (impedindo que perfis de "Recepção" ou "Tutor" alterem registros médicos)

Usabilidade: Um tutor deve conseguir agendar uma consulta pelo celular em no máximo 4 passos

Validação dos requisitos antes do desenvolvimento:
Simulação com prototipos para apresentar aos clientes



