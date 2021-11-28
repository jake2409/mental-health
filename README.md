<div align="center">
  <img src="/img/Logo_sem_fundo_-_Mental_Health.png">
</div>

Este material é um guia para o desenvolvimento do projeto Mental-Health. Dentro dos aprendizados, destacamos os seguintes pontos como principais aprendizados:

<ul>
  <li>Entender o proposito do nosso projeto Mental-Health através dos requisitos listados e escolhidos, e o nosso caso de uso;</li>
  <li>Entender a estrutura de desenvolvimento que seguiremos para desenvolver nosso projeto;</li>
  <li>Entender como mediremos a qualidade do nosso projeto;</li>
  <li>Entender como testaremos o projeto.</li>
</ul>

___


🗂 **A organização do documento se dá nas seguintes seções:**

<ul>
  <li>Introdução</li>
  <ul>
    <li>Tema</li>
    <li>Objetivos a Serem Alcançados</li>
    <li>Escopo Principal</li>
  </ul>
  <li>Definição do Modelo de Processo</li>
  <li>Requisitos do Sistema de Software</li>
  <ul>
    <li>Requisitos Funcionais</li>
    <li>Requisitos Não-Funcionais</li>
    <li>Casos de Uso</li>
  </ul>
  <li>Projeto</li>
  <ul>
    <li>Arquitetura Lógica</li>
    <li>Arquitetura Física</li>
  </ul>
  <li>Protótipo de Interface</li>
  <ul>
    <li>Página Inicial</li>
    <li>Página de Login</li>
    <li>Cadastro de Paciente</li>
    <li>Cadastro de Profissional</li>
    <li>Cadastro de Entregador Delivery</li>
    <li>Agendamento de Consultas</li>
    <li>Compra de Medicamentos</li>
    <li>Visão da Consulta</li>
    <li>Tela de Administrador</li>
    <li>Tela de Profissional (Médico)</li>
    <li>Tela de Entregador Delivery</li>
    <li>Tela de Paciente</li>
  </ul>
  <li>Critérios de Qualidade de Software</li>
  <li>Testes</li>
  <ul>
    <li>Plano de Testes</li>
    <li>Roteiro de Testes</li>
  </ul>
  <li>Anexo I</li>
</ul>

___

# 1. Introdução
O principal desafio deste projeto referente ao segundo semestre de 2021 era que os grupos desenvolvessem toda a documentação de um produto de software abordando todo o conteúdo passado em sala de aula.
As UCs (Unidades Curriculares) responsáveis pelo acompanhamento e apoio no desenvolvimento do mesmo foram:
<ul>
  <li>Modelos, Métodos e Técnicas da Engenharia de Software;</li>
  <li>Gestão e Qualidade de Software.</li>
</ul>
Professores responsáveis:
<ul>
  <li>Pedro Yuri Araujo Lima Alves (Mentor);</li>
  <li>Fernando Marcio Bettine.</li>
</ul>

___

✨ **1.1. Tema:**

O software proposto é para prestar atendimentos de forma remota em psicologia, hipnoterapia e psiquiatria, para ajudar as pessoas que necessitam desse auxílio. Além dos atendimentos, haverá a possibilidade de compra e entrega de medicamentos.

✨ **1.2. Objetivos a Serem Alcançados:**

O objetivo do software a ser desenvolvido é criar uma plataforma paga onde os psicólogos, psiquiatras e hipnoterapeutas interessados possam se cadastrar, montar um perfil profissional, prestar o atendimento à distância, seja via chat ou vídeo chamada. Os mesmos receberão os pagamentos pela própria plataforma. 
Os pacientes que desejarem atendimento poderão se cadastrar na plataforma, receber o atendimento desejado e realizar o pagamento pela própria plataforma. Em cima do valor total, parte será descontado para os custos da plataforma e transações, o restante do valor será repassado ao profissional (psicólogo/psiquiatra/hipnoterapeuta).
Iremos melhorar um processo já existente em outras plataformas para atendimento psicológico, porém iremos trazer o diferencial de disponibilizar consultas de hipnoterapia e ter convênio com farmácias já cadastradas no sistema.
O convênio com as farmácias já cadastradas além de fornecer descontos exclusivos, poderá enviar o medicamento para a residência do paciente de forma automatizada após a autorização do mesmo. Caso o paciente recuse a opção de compra, o mesmo terá sua via do pedido médico assinado digitalmente pelo profissional, para que realize a compra do medicamento onde ele preferir.
Iremos também disponibilizar o sistema de entrega de medicamentos delivery. Motoboys que estiverem na região e cadastrados no sistema, serão notificados e aquele que aceitar primeiro ficará responsável pela entrega do item, desta forma recebendo o valor da entrega realizada.
O público alvo para este projeto são: clientes, psicólogos, psiquiatras, hipnoterapeutas, pessoas que necessitam de atendimentos psicológicos, farmácias e motoboys interessados em realizar entregas.

✨ **1.3. Escopo Principal:**

O foco principal do software é facilitar o processo para o público que deseja atendimentos psicológicos e aos profissionais da área, tendo em vista o cenário atual de pandemia.
Para que seja possível a implementação do projeto, será necessário ter profissionais do ramo e farmácias cadastradas para atingir o principal objetivo, atender pacientes.
Contudo, queremos deixar o paciente totalmente confortável em um ambiente que vai estar totalmente preparado para ajudá-lo da melhor forma em seu tratamento, visto a importância do tema que abordamos no projeto. Pensando nisso, queremos que o paciente e o profissional estejam confortáveis em suas residências, pois todo o tratamento será remoto e ambos terão todo o suporte necessário.

___

# 2. Definição do Modelo de Processo 

O modelo de processo que será utilizado para o desenvolvimento deste projeto será o Incremental, pois é uma metodologia ágil, onde serão criadas várias versões até que o sistema fique completo e adequado, para assim ser lançada a versão final do software. Obtendo uma integração simples com o cliente final. Além de ser um modelo que oferece fácil manutenibilidade, um dos requisitos importantes para se poder medir qualidade de um sistema e trazer novas ferramentas para nossa aplicação que pode englobar grandes áreas da saúde mental.

___

# 3. Requisitos do Sistema de Software 

✨ **3.1. Requisitos Funcionais:**
<ul>
  <li>Realizar pré cadastro (profissional e motoboys);</li>
  <li>Aprovar cadastros (profissional e motoboy);</li>
  <li>Realizar cadastros de pacientes;</li>
  <li>Cadastrar novos admins;</li>
  <li>Criar perfil do profissional;</li>
  <li>Agendar horários;</li>
  <li>Disponibilizar histórico de consultas para o paciente e profissional;</li>
  <li>Disponibilizar agenda de consultas agendadas para o paciente e profissional;</li>
  <li>Realizar consultas médicas/salas de consultas;</li>
  <li>Incluir medicamentos no carrinho do paciente;</li>
  <li>Realizar compra de remédios de forma automática, após autorização;</li>
  <li>Realizar pagamentos;</li>
  <li>Liberar comissões;</li>
  <li>Disponibilizar históricos de entregas para motoboys;</li>
  <li>Emissão de documentos (receitas médicas e atestados);</li>
  <li>Realizar transferências de pagamentos (do app para a conta dos profissionais);</li>
  <li>Emissão de relatórios financeiros para o Admin do sistema;</li>
  <li>Consultar status do pedido;</li>
  <li>Localizar farmácias e motoboys próximos ao cliente;</li>
  <li>Ter opção de comunicação de chat e vídeo chamada.</li>
</ul>

✨ **3.2 Requisitos Funcionais:**
<ul>
  <li>O software deverá atender os sistemas operacionais Android, IOS e Web;</li>
  <li>Banco de dados SQL (Structured Query Language);</li>
  <li>Interação com ferramentas de consulta de medicamentos de farmácias;</li>
  <li>Conexão com a internet;</li>
  <li>Utilização da API Google para localização;/li>
  <li>Autenticação de dois fatores;</li>
  <li>Deve ser criptografado.</li>
</ul>

✨ **3.3 Caso de Uso:**
<div align="center">
  <img src="/img/casodeuso.png">
</div>

___

# 4. Projeto

🗽 **4.1 Arquitetura Lógica:**

A arquitetura que será usada no projeto é a Cliente-Servidor. Esta arquitetura nos favorece no fato de possuir  divisão entre as manutenções de informações (servidores) e outra parte pela obtenção de dados (cliente).
O cliente sempre solicitará um determinado serviço ao servidor e enquanto o mesmo trabalha com seus processos, o cliente está livre para fazer outras tarefas. Já o servidor somente terá o papel de oferecer os serviços ao cliente, executar e responder de acordo com essas tarefas.
O ponto positivo é que podemos evitar redundâncias em um banco de dados centralizado para todos utilizadores.
<ul>
  <li> <b> Linguagem de Programação </b> </li>
  Utilizaremos a linguagem de programação PHP e seus frameworks como principal linguagem do back-end, além de algumas ferramentas de desenvolvimento front-end como JavaScript e a linguagem de marcação HTML.
Já para a parte remota para IOS e Android, utilizaremos a linguagem JAVA.
</ul>
<ul>
  <li> <b> Banco de Dados </b> </li>
  O Banco de Dados que utilizaremos é o sistema gerenciador MySQL para armazenar informações na parte do servidor. O sistema MySQL se relaciona muito bem com a linguagem PHP, esta linguagem possui algumas funções próprias de tratamento de dados para utilizarmos com mais segurança em nossa aplicação. Além disso, o MySQL é compatível com as plataformas de desenvolvimento que disponibilizamos para nossa aplicação.
Nossa equipe está muito bem preparada para utilizar essa ferramenta, já que já desenvolvemos aplicações utilizando essas tecnologias.
</ul>
<ul>
  <li> <b> Componentes Externos </b> </li>
  Os componentes externos que iremos utilizar são APIS para integrar com a nossa aplicação para evitar a repetição de regras de negócios que já existem e estão lá para serem consumidas. Além disso, com objetivo de facilitar a integração e evolução posterior do nosso sistema, desenvolvemos nossas próprias APIS.
Algumas APIS externas que já estão estabelecidas que serão utilizadas são: API do google maps para lugares e para trajetos.
Também precisaremos de uma comunicação com as farmácias para obter informações de estoque e valor.
</ul>

🗽 **4.2 Arquitetura Física:**

Quando nos referimos a aplicação mobile, o hardware não precisaria ser muito robusto, pelo motivo de estarmos utilizando tecnologias mais simples.
Quanto à tecnologia web, para utilizar nossa aplicação será necessário que pelo menos a ferramenta utilizada rode algum dos tipos de browsers disponíveis para a nossa aplicação.

<ul>
  <li> <b>Configuração de Rede </b> </li>
  Iremos oferecer um serviço que contém a comunicação entre chat e vídeo-chamada, e para a melhor experiência tanto do profissional quanto do cliente, o ideal é que ambos tenham uma internet estável.
</ul>
<ul>
  <li> <b>Diagrama de Implantação </b> </li>
  <img src="/img/diagramadeimplantacao.png">
</ul>

___

# 5. Protótipo de Interface:

Segue abaixo os prints das principais telas do software.
<ul>
  <li>Página Inicial</li>
  <img src="/img/paginainicial.png">
</ul>

<ul>
  <li>Página de Login</li>
  <img src="/img/paginadelogin.png">
</ul>

<ul>
  <li>Cadastro de Paciente</li>
  <img src="/img/cadastrodepaciente.png">
</ul>

<ul>
  <li>Cadastro de Profissional</li>
  <img src="/img/cadastrodeprofissional.png">
</ul>

<ul>
  <li>Cadastro de Entregador Delivery</li>
  <img src="/img/cadastrodeentregadordelivery.png">
</ul>

<ul>
  <li>Agendamento de Consultas</li>
  <img src="/img/agendamentodeconsultas.png">
</ul>

<ul>
  <li>Compra de Medicamentos</li>
  <img src="/img/comprademedicamentos.png">
</ul>

<ul>
  <li>Visão da Consulta</li>
  <img src="/img/visaodaconsulta.png">
</ul>

<ul>
  <li>Tela de Administrador</li>
  <img src="/img/teladoadministrador.png">
</ul>

<ul>
  <li>Tela de Profissional (Médico)</li>
  <img src="/img/teladeprofissional.png">
</ul>

<ul>
  <li>Tela de Entregador Delivery</li>
  <img src="/img/teladoentregador.png">
</ul>

<ul>
  <li>Tela de Paciente</li>
  <img src="/img/teladopaciente.png">
</ul>

___

# 6. Critérios de Qualidade de Software

De modo geral, a qualidade de um software pode ser avaliada seguindo algumas métricas, e possui objetivos exclusivos a serem alcançados tanto para o usuário e/ou cliente, quanto para desenvolvedores.
Destacamos a norma ISO 9126, que define parâmetros com o objetivo de padronizar a avaliação da qualidade de software. A norma conta com os seguintes atributos de qualidade:

<img src="/img/qualidade.png">

A nossa equipe de desenvolvimento decidiu destacar três atributos:
<b>Confiabilidade:</b> Nos testes realizados pela equipe, o software apresentou boa recuperação em relação a falhas, o software possui um sistema de logs em cache onde armazena as falhas frequentes provocadas pelos usuários, para a equipe de desenvolvimento analisar e procurar as soluções.

<b>Eficiência:</b> A utilização de ferramentas, frameworks e api’s foram escolhidas pela equipe a fim de melhorar a conformidade do sistema, oferecendo dados a uma interface extremamente fluida, trazendo um comportamento em relação ao tempo otimizado. Ainda, a equipe de desenvolvimento teve o cuidado de planejar a base de dados de forma a evitar sobrecargas não necessárias, afinal por se tratar de uma aplicação externa, temos em mente que podemos receber milhares de requisições em nossos servidores em um leque de tempo baixo.

<b>Manutenabilidade:</b> A equipe de QA (Quality Assurance) oferece apoio aos desenvolvedores, efetuando durante o desenvolvimento diversos testes a fim de identificar problemas no código, funcionamento e nos tópicos em manutenabilidade, com o objetivo de solucionar as falhas e consequentemente serem as mínimas possíveis, até que o software entre em produção.
Contudo, por escolhermos o método de desenvolvimento incremental, temos em mente um software que estará em constante evolução trazendo assim, manutenções e updates constantemente.

___

# 7. Testes

Segue abaixo os prints das tabelas que foram desenvolvidas com a finalidade de realizar os devidos Testes.
Vale ressaltar que as informações aqui contidas são apenas uma simulação, pois a plataforma não foi desenvolvida da prática e portanto, não teria como testá-la.

📜 **7.1 Plano de Testes:**

Segue abaixo os prints da tabela que foi desenvolvida para esta finalidade (Plano de Testes), preenchida com as devidas informações.
<img src="/img/planodeteste1.jpg">
<img src="/img/planodeteste2.jpg">
<img src="/img/planodeteste3.jpg">
<img src="/img/planodeteste4.jpg">
<img src="/img/planodeteste5.jpg">
<img src="/img/planodeteste6.jpg">

📜 **7.2 Roteiro de Testes:**

Segue abaixo os prints da tabela que foi desenvolvida para esta finalidade (Roteiro de Testes), preenchida com as devidas informações.
<img src="/img/roteirodeteste1.jpg">
<img src="/img/roteirodeteste2.jpg">
<img src="/img/roteirodeteste3.jpg">
<img src="/img/roteirodeteste4.jpg">
<img src="/img/roteirodeteste5.jpg">
<img src="/img/roteirodeteste6.jpg">
<img src="/img/roteirodeteste7.jpg">
<img src="/img/roteirodeteste8.jpg">

___

# Anexo I
🎬  **Transcrição da Entrevista:**

- Esta entrevista está sendo realizada para que possamos fazer um breve levantamento dos requisitos do seu sistema.
- Vale ressaltar que esta entrevista é sigilosa e em anonimato, não será em hipótese alguma divulgada publicamente.

**-Primeiramente, gostaria que me explicasse qual é o principal objetivo deste projeto.**
-Nós já atuamos com as áreas de psicologia, psiquiatria e hipnoterapia, porém apenas no atendimento presencial. Com o avanço da pandemia nós enxergamos a oportunidade de unir os três tratamentos em um único sistema online, além de trazer melhorias como a parceria com farmácias e entregas via delivery.

**-Fale sobre quais são as suas principais atividades na organização, explique como é atualmente o processo do escopo principal.**
-Sou o diretor e fundador da empresa, mas participo ativamente de todas as rotinas. Hoje tenho uma clínica especializada em psicologia, psiquiatria e hipnoterapia. Os atendimentos atualmente são apenas presenciais.
Com o avanço da pandemia, enxergamos a oportunidade de inovar e com isso queremos um software que nos permita realizar atendimentos remotos, criar parcerias com farmácias para compra de remédios de forma automatizada, e ter o sistema de entrega de medicamentos via delivery.

**-Quais são as vantagens e desvantagens do processo atual na organização?**
-Atualmente temos uma única unidade e com estrutura apenas para atendimentos presenciais. O lado positivo nisso tudo é que temos bons profissionais e uma ótima gama de clientes.

**-Quem poderia usar este produto na organização?**
-Na organização quem poderá utilizar o software a ser desenvolvido são os profissionais e administradores do sistema.

**-Quais são as necessidades que este produto atenderá?**
-A expansão dos negócios, podendo captar clientes de diversas regiões sem que o mesmo tenha que comparecer presencialmente, e o atendimento flexível para que os clientes possam agendar suas consultas no horário desejado sem ter que encarar filas.

**-Quais são os objetivos deste produto?**
-Atuar como facilitador para o agendamento de consultas, realizar atendimentos de forma remota e venda de medicamentos pela própria plataforma de acordo com o pedido médico.

**-Como este produto irá adicionar valor para a empresa?**
-Uma vez que estamos na era digital e as empresas estão se reinventando cada vez mais, não podemos ficar para trás. A expansão de nossos serviços para o meio online irá potencializar nosso negócio.

**-Quais atributos deste produto são críticos para atender às necessidades da empresa e portanto, para o sucesso do projeto?**
-Um requisito imprescindível para o projeto é a Eficiência. Visto que nossa principal função será a consulta de profissionais com clientes. O recurso de videochamadas, por exemplo, deverá apresentar alta eficiência.

**-Como o produto proposto se compara aos produtos existentes dos concorrentes ou da mesma empresa? O que você sabe sobre produtos similares?**
-As consultas remotas hoje já são uma realidade. Nossa proposta é unir consultas online dos profissionais das áreas citadas (Hipnoterapia, Psicologia e Psiquiatria). O nosso diferencial do mercado atual serão as parcerias com farmácias que iremos realizar, além da entrega de medicamentos via delivery.
Encontramos empresas que realizam consultas online em psiquiatria e psicologia apenas, mas nenhuma delas incluíam os três tratamentos juntos, parceria com farmácias e entregas via delivery.

**-Quais os critérios de qualidade para o produto (software) proposto?**
-Prezamos pela eficiência, portabilidade e confiabilidade. Portabilidade, pois nosso software deve apresentar pleno funcionamento em diversas plataformas (Web, desktop, mobile). Confiabilidade pois não podemos correr o risco de perder os dados, por exemplo, de clientes, consultas, pagamentos e entre outros. 

**-Quais sugestões você teria para melhorar o produto proposto?**
-No momento, acredito que nada. Mas no futuro talvez seja interessante incluirmos outros tipos de consultas da área da saúde, para podermos tratar em conjunto um único paciente.

**-Quais os dados que você acredita que devem ser fornecidos para acessar o sistema?**
-Acredito que logar com CPF e senha seja o mais seguro.

**-Como os profissionais interessados poderão se cadastrar na plataforma?**
-Neste caso, o mesmo poderá fazer um pré-cadastro em nosso sistema, podendo atuar de fato, apenas após a avaliação e aprovação do administrador.

**-O que acha que é necessário para que você considere o projeto finalizado?**
-Eu prefiro que o sistema seja entregue apenas quando estiver completo e apto para fazer seu papel. Como estamos tratando com dados pessoais e sensíveis não podemos correr o risco de falhas. De qualquer forma me disponho a participar de todas as etapas caso seja necessário.

**-Você teria algo a acrescentar sobre o que conversamos?**
-No momento não, obrigado.

