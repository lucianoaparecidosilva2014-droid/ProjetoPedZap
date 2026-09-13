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

### Instalação

Para instalar e executar o ProjetoPedZap, siga os passos abaixo:

1. Clone o repositório:

```bash

git clone https://github.com/lucianoaparecidosilva2014-droid/ProjetoPedZap.git

```

2. Navegue até o diretório do projeto:

```bash

cd ProjetoPedZap

```

3. Instale as dependências:

```bash

flutter pub get

```

4. Execute a aplicação:

```bash

flutter run

```

### Uso

Para utilizar o ProjetoPedZap, siga os passos abaixo:

1. Faça login na aplicação utilizando suas credenciais do Google.

2. Na tela de pedidos, você pode visualizar a lista de pedidos ativos e criar novos pedidos.

3. Na tela de detalhes do pedido, você pode visualizar os detalhes de um pedido específico e atualizar o status do pedido.

### Contribuição

Contribuições são bem-vindas! Para contribuir com o ProjetoPedZap, siga os passos abaixo:

1. Faça um fork do repositório.

2. Crie uma nova branch para a sua contribuição:

```bash

git checkout -b minha-contribuicao

```

3. Faça as alterações necessárias e commit as alterações:

```bash

git commit -m "Minha contribuição"

```

4. Envie as alterações para o seu fork:

```bash

git push origin minha-contribuicao

```

5. Abra um pull request no repositório original.

### Licença

O ProjetoPedZap é licenciado sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.

### Conclusão

O ProjetoPedZap é uma aplicação robusta e escalável que permite aos usuários criar e gerenciar pedidos de delivery. A aplicação é construída utilizando tecnologias modernas e segue uma arquitetura limpa e modular, tornando-a fácil de entender, manter e estender.

### Tela de Senha para Painel Admin

Para acessar o painel de administração, é necessário inserir uma senha. Isso garante que apenas usuários autorizados possam acessar e gerenciar os pedidos.

### Mensagem de Confirmação no WhatsApp

A aplicação agora gera automaticamente a mensagem de confirmação no WhatsApp para cada pedido usando AI Gateway. A mensagem é personalizada com base no tipo de pedido (entrega/retirada), itens e total, garantindo consistência e personalização.

### Segurança

Para garantir a segurança dos dados, a aplicação implementa medidas rigorosas de proteção de dados. A tabela `store_config` nunca retorna o campo `pix_key` e nenhum outro campo sensível está exposto sem autenticação.