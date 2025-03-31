# Curso OutSystemas Reactive Developer

## 1. Trilha Reactive

### 1.1. Introdução
- OutSystems é uma empresa de capital privado que ajudou a cunhar o termo low code.
- Ela está presente em mais de 87 países.
- Possui clientes no mundo inteiro, com mais de 20 indústrias atendidas.
- Possui mais de 340 parceiros globais espalhados no mundo.
- Sua comunidade já ultrapassou mais de 500 mil membros.
- Várias empresas no Brasil já adotaram o uso da plataforma.
- Até 2024, 65% de todo desenvolvimento de aplicações será feito em low code.
- É mais interessante para as empresas terceirizar a parte operacional.
- Os negócios enfrentam grandes barreiras na transformação digital:
	- Acúmulos de trabalhos nos projetos (backlogs).
	- Sem tempo para pensar em inovações.
	- Recursos caros e escassos.
- As empresas precisam digitalizar as informações e automatizar processos.
- Mais aplicações, plataformas, dados, tecnologias e mudanças a cada tempo.
- O desenvolvimento tradicional é mais lento e demanda mais pessoas.
- A OutSystemas automatiza os processos e torna o desenvolvimento mais ágil.
- Características da Plataforma OutSystems:
	- É uma plataforma escalável, entregando a performance que o cliente precisa.
	- É possível fazer um desenvolvimento full-stack através dela.
	- Ela oferece meios de integração e extensão com aplicações do mundo todo.
	- Ela favorece todo o desenvolvimento dentro do ciclo DevOps de forma fácil.
	- Ela fornece uma experiência rica no ponto de vista dos consumidores.

### 1.2. Visão Geral
- A plataforma OutSystems é formada por diversos componentes e ferramentas.
- O Platform Server é o primeiro destes componentes, sendo o principal.
	- Possui todas as informações que são armazenadas, junto com o banco.
	- Permite o gerenciamento e monitoramento das aplicações.
	- Permite a compilação e implantação das aplicações nos ambientes.
- O Service Studio é a ferramente de desenvolvimento visual da aplicação.
- O Integration Studio facilita a integração com APIs e bancos de dados.
- O Service Center permite gerir todo o ambiente das aplicações.
	- Permite também realizar configurações e monitorar logs da aplicação.
- O LifeTime permite gerenciar todo o ciclo de vida das aplicações.
	- Com poucos cliques, o deploy é feito em UAT e produção.
	- Permite também o versionamento e controle de usuários dos ambientes.
	- Permite gerenciar as infraestruturas dos ambientes de UAT e produção.
	- Permite realizar logs, gerenciamento de dados e performance.
- O OutSystems Forge disponibiliza ferramentas e componentes de terceiros.
- Os Community Forums permite o acesso à comunidade de OutSystems.
- Em resumo:
	- Desenvolvimento: Service Studio e Integration Studio.
	- Admin e Operações: LifeTime e Service Center.
	- Community: Forge e Community.

### 1.3. Service Studio
- É através dele que criamos nossas aplicações e os seus módulos.
- Definimos também o Data Model com ele.
- Criamos interfaces para aplicações web e mobile.
- Usamos ele para definir processos e timers.
- Usamos ele para depurar as aplicações desenvolvidas.

### 1.4. Tipos de Aplicações
- O OutSystems pode criar dois tipos de aplicações: Mobile e Reactive Web.
- Aplicações Mobile são voltadas para Smartphones e Tablets.
- Reactive Web são aplicações que se moldam ao Mobile e ao Desktop.
- Antigamente, as aplicações Web não eram reativas a estes dois ambientes.
- Independente do tipo, estas aplicações englobam as melhores práticas.
- Elas devem fornecer aos usuários as melhores experiências possíveis.
- O low code une em si uma experiência unificada de desenvolvimento.
- O que considerar ao escolher um tipo ou outro para desenvolver.
- Reusabilidade:
	- Aplicações responsivas reusam a lógica entre ambientes.
	- Aplicaões mobile reusam a lógica entre dispositivos.
- Público e Dispositivos:
	- Aplicações responsivas são acessadas em navegadores.
	- Aplicações mobile precisam ser instaladas no dispositivo.
- Experiência de Usuário:
	- Aplicações responsivas servem a vários tamanhos e tipos de telas.
	- Aplicações mobile servem aos padrões e experiências dos aparelhos.
- A performance é a mesma para ambas as aplicações.
- Acesso a Recursos de Hardware:
	- Aplicações responsivas o fazem através do HTML5.
	- Aplicações mobile o fazem através dos dispositivos.
- Capacidades Offline:
	- Aplicações responsivas são muito limitadas neste aspecto.
	- Aplicações mobile podem usar recursos do próprio aparelho.
- Implantação e Atualização:
	- Aplicações responsivas já trazem por meio do navegador.
	- Aplicações mobile trazem apenas por meio de atualizações.
- Distribuição:
	- Aplicações responsivas dispõem apenas de um link.
	- Aplicações mobile necessitam baixar o aplicativo desenvolvido.

### 1.5. Programação Modular
- Além de criar aplicações, somos capazes de dividí-las em Módulos.
- Com isso, encapsulamos partes das aplicações para reusá-las.
- Estas partes podem ser independentes e insubstituíveis.
- Ex: Módulo de Interface de Acesso e Módulo de Base de Dados.
- O código e a interface são desenvolvidos dentro do Módulo.
- Módulos são divididos por Tipo:
	- Aplicação (Reactive Web e Mobile)
	- Blank
	- Serviço
	- Biblioteca
	- Extensão
- Uma Aplicação agrupa um conjunto de Módulos.
- Os Módulos podem compartilhar elementos com outros Módulos.
	- Estes Módulos são chamados de Produtores.
	- Os Módulos que usam as features de outros são Consumidores.
- Produtores e Consumidores podem estar em diferentes Aplicações.
- Existem alguns Módulos que já são criados por convenção.
- O Módulo Core, de Tipo Serviço contém as bases da Aplicação.
	- Serviços só têm camadas de Processo, Lógica e de Dados.
- O Módulo Web, de Tipo Reactive, inclui a camada Interface.
- No Módulo Core, são criadas as Entidades das Tabelas:
	- Ao definí-la como Pública, é possível expor ela a outras.
	- Deve-se adicionar a ela Atributos além do Id.
- O botão Publish no Service Studio permite a publicação:
	- O Módulo passa a ficar disponível no ambiente OutSystems.
- Com isso, é possível consumir o Core em outro Módulo.
- O Manage Dependencies do Service Studio permite o consumo.
	- É possível selecionar quais informações serão consumidas.

### 1.6. Modelando Dados - Entidades e Atributos
- Em qualquer tipo de aplicação, precisamos manipular informações.
- Precisamos armazenar, processar e recuperar estas informações.
- As informações possuem valor para todo tipo de negócio.
- Estas informações geralmente são referenciadas como Entidades.
	- Clientes, Produtos, Pedidos, Tipo de Pedido, Status.
- As Entidades são organizadas em ambiente de desenvolvimento.
- Toda Entidade possui um conjutno de Dados ou Atributos.
- As Entidades também possuem Relacionamentos dentro do ambiente.
- Uma Entidade nada mais é que uma Tabela na Base de Dados.
	- Atributos -> Colunas
	- Id -> Chave Primária
	- Atributo de Referência -> Chave Estrangeira
	- Índice -> Índice
	- Registro ou Instância -> Linha ou Tupla
- Cada aspecto do negócio é representado por uma Entidade.
- As Entidades são armazenadas dentro do Banco de Dados.
- Dentro do OutSystems, as Entidades também possuem Ações.
	- Criar, Alterar, Deletar Tabela
- A Chave Primária é o registro único da Entidade.
- Os Atributos apresentam diferentes conceitos da Entidade.
- Cada Atributo possui um Tipo, definindo sua função e formatação.
	- Números, Textos, Telefone, E-mail, Monetário, Booleano, etc.
- Todos estes Atributos vêm com um valor padrão.
- O OutSystems possui uma IA que identifica o Tipo de um Atributo.
	- A identificação é feita através do nome do Atributo.

### 1.7. Modelando Dados - Ações e Entidades Estáticas
- Assim que a Entidade é criada, Ações padrão são automaticamente criadas.
- Estas Ações são o CRUD: Create, Retrieve, Update, Delete.
- Elas podem ser usadas diretamente na lógica de negócio da aplicação.
- No OutSystems, existem também as Entidades que são as Estáticas:
	- Ela cria uma lista pré-definida de valores que não se alteram.
	- Ex: Status, Cores, Tipos, Etapas, Moeda, Países, Estados, Cidades.
- Entidades Estáticas não são alteradas em tempo de execução.
- Para as Entidades Estáticas, somente a Ação Retrieve é possível.
- Apenas quatro Atributos Padrão são criadas para a Entidade Estática.
	- Apenas os necessários: Id, Label, Order e Is_Active.
- As Entidades Estáticas podem ser referenciadas pelas Labels na lógica.
- As Entidades Estáticas são muito mais leves e fáceis de se consumir.

### 1.8. Modelando Dados - Importação de Entidades e Dados
- Para realizar a modelagem de dados, uma Aplicação nova deve ser criada.
- Dentro da Aplicação, deve ser criado um Módulo que tenha a camada Data.
- Na camada Data, já há uma Entidade Default para os usuários (User).
- Em cima do item Database, podemos adicionar uma nova entidade Wine.
- As novas Entidades já são criadas com todas as Ações e somente o Id:
	- Deve ser adicionado pelo menos um Atributo para a nova Entidade.
- Os novos Atributos adicionados já vem com tamanho padrão:
	- Além do tamanho, o Tipo e a Obrigatoriedade são automáticos.
	- É possível também definir um valor padrão para o Atributo.
- Os Atributos vêm acompanhados de um dado chamado Label:
	- As Labels correspondem ao nome que será apresentado na Aplicação.
- Outra forma de se criar Entidades no OutSystems é pela importação:
	- O nome deste processo se chama Bootstrap.
- Um arquivo Excel pode ser utilizado para a importação de seus dados:
	- O nome do arquivo deve ser o nome da Entidade.
	- Para cada Atributo, deve haver uma coluna diferente.
	- A primeira linha é o nome do Atributo.
	- As demais linhas são os valores para cada registro inserido.
- Também é possível importar dados para uma Entidade:
	- O Excel deve ser também organizado em colunas.
	- A primeira linha corresponde aos nomes dos Atributos.
	- As demais linhas são os valores de cada registro inserido.
- Sempre que as importações forem feitas, deve ser feito um Publish.

### 1.9. Modelando Dados - Criando e editando via Interface
- Uma vez tendo criado e populado as Entidades, é possível editá-las manualmente.
- Edições via Service Studio só devem ser feitas em ambiente de desenvolvimento.
- Novos registros podem ser adicionados manualmente via Service Studio.
- Também é possível criar manualmente as Entidades Estáticas no Service Studio.
- Criar Atributos iguais aos nomes de outras Entidades gera referência automática.

### 1.10. Desenvolvimento de UIs Reativas - Conceito de Widgets
- Uma interface gráfica é um conjunto organizado de componentes gráficos.
- Através destes componentes, o usuário interage com a Aplicação.
- Um conjunto de interfaces gráficas compõem um fluxo de interações.
- As telas podem ser construídas vazias ou partindo de um Template.
- Dentro do OutSystems, os componentes são chamados de Widgets.
- Um Widget pode ser um campo texto, um botão, um check ou uma lista.
- Os Widgets podem ser responsivos, adaptando-se a mais de uma tela.
- Cada tela dentro do OutSystems engloba um conjunto de informações.
- Estas informações podem ser passadas via parâmetro dentro do fluxo.
- Através de uma tela, outra tela pode ser chamada recebendo dados.
- Estes dados são carregados na próxima tela por meio de variáveis.
- As telas também podem ter variáveis locais, consumidas dentro dela.
- Componentes como botões também podem chamar ações lógicas:
	- Um botão "Salvar", por exemplo pode chamr uma ação ou uma tela.
- Estas ações lógicas no OutSystems são chamadas de Screen Actions.
- O destino do botão ou link é configurado através do Service Studio:
	- Outra tela, URL externa, ações e eventos.

### 1.11. Desenvolvimento de UIs Reativas - Criando a primeira Tela
- No Service Studio, é possível criar as telas de um Módulo na camada Interface.
- A tela pode ser criada do zero, manualmente, ou a partir de um Template.
- As telas possuem espaços reservados para a adição e composição de Widgets.
- Os Widgets são adicionados na tela com um simples drag and drop.
- Cada Widget possui atributos e estilos que são configuráveis.
- É possível até mesmo utilizar conceitos de CSS para estilizar os componentes.
- É possível salvar em classes todos os CSS escritos dentro dos componentes.
- O OutSystems permite que o tema da Aplicação seja ajustado em um modal.
- Adicionando Widgets de visualização, deve-se escolher os dados a serem vistos:
	- O Widget já é carregado com uma lista dos registros daquela Entidade.
- Todo Widget de Botão deve estar associada a uma Ação ao ser clicada.
- O OutSystems cria por padrão uma tela de Login para autenticação.
