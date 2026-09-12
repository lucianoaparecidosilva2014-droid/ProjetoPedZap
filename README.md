# ProjetoPedZap

## Explicação Técnica

### Visão Geral

O ProjetoPedZap é uma aplicação que permite aos usuários criar e gerenciar pedidos de delivery. A aplicação é construída utilizando tecnologias modernas e segue uma arquitetura limpa e modular.

### Arquitetura

A arquitetura da aplicação é baseada em camadas, com as seguintes camadas principais:

1. **Camada de Apresentação**: Responsável pela interface do usuário e pela interação com o usuário final. Esta camada é construída utilizando Flutter, um framework de desenvolvimento de aplicações multiplataforma.

2. **Camada de Negócio**: Contém a lógica de negócio da aplicação. Esta camada é responsável por processar os pedidos, gerenciar os usuários e interagir com a camada de dados.

3. **Camada de Dados**: Responsável pela persistência e recuperação de dados. Esta camada utiliza Firebase Firestore para armazenar e recuperar dados em tempo real.

### Fluxo de Dados

O fluxo de dados na aplicação é gerenciado utilizando o padrão BLoC (Business Logic Component). O BLoC é responsável por separar a lógica de negócio da interface do usuário, tornando o código mais modular e fácil de testar.

1. **Eventos**: Os eventos são ações que ocorrem na interface do usuário, como clicar em um botão ou digitar em um campo de texto. Os eventos são enviados para o BLoC.

2. **BLoC**: O BLoC recebe os eventos e processa a lógica de negócio. O BLoC pode emitir estados em resposta aos eventos.

3. **Estados**: Os estados representam o estado atual da aplicação. Os estados são enviados de volta para a interface do usuário, que os utiliza para atualizar a exibição.

### Componentes Principais

1. **Tela de Login**: Permite aos usuários fazerem login na aplicação utilizando suas credenciais do Google.

2. **Tela de Pedidos**: Exibe a lista de pedidos ativos e permite aos usuários criar novos pedidos.

3. **Tela de Detalhes do Pedido**: Exibe os detalhes de um pedido específico e permite aos usuários atualizar o status do pedido.

### Lógica de Negócio

A lógica de negócio da aplicação é responsável por processar os pedidos, gerenciar os usuários e interagir com a camada de dados. A lógica de negócio é implementada na camada de negócio e é acessada pela camada de apresentação através do BLoC.

### Conclusão

O ProjetoPedZap é uma aplicação robusta e escalável que permite aos usuários criar e gerenciar pedidos de delivery. A aplicação é construída utilizando tecnologias modernas e segue uma arquitetura limpa e modular, tornando-a fácil de entender, manter e estender.