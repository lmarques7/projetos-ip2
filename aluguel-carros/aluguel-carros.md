# Sistema de Aluguel de Carros

## Descrição
O sistema será um serviço de aluguel de carros que permitirá aos usuários alugar veículos por períodos definidos (diário, semanal, etc.), de acordo com as condições e disponibilidade. O administrador do sistema poderá cadastrar os carros disponíveis para aluguel, especificando informações como modelo, preço, características e disponibilidade.

O sistema deve ser intuitivo, permitindo que os usuários escolham o carro desejado, faça a reserva e o pagamento. Além disso, os usuários poderão gerenciar as reservas realizadas, visualizar histórico de alugueis e efetuar cancelamentos. Para o administrador, o sistema oferecerá ferramentas de gerenciamento de carros, incluindo a opção de adicionar, editar ou remover veículos, assim como visualizar as reservas realizadas e a renda gerada.

O aluguel de carros incluirá funcionalidades como o cálculo do preço total com base no tempo de aluguel, possíveis taxas extras, seguro e condições de devolução.

**Exemplo de sistemas reais**: Esse tipo de sistema é amplamente utilizado por empresas como **Localiza**, **Movida** e **Hertz**, que oferecem uma plataforma online para que os clientes reservem carros, escolham o modelo, o tempo de aluguel e realizem o pagamento.

## Requisitos Funcionais

### Gerenciamento de Entidades
- **REQ01**: Gerenciamento de administradores, que podem cadastrar, editar ou remover carros do sistema.
- **REQ02**: Gerenciamento de carros disponíveis para aluguel, com informações sobre modelo, tipo de carro, preço, características (ex.: número de portas, capacidade, etc.) e status de disponibilidade.
- **REQ03**: Gerenciamento de usuários, que podem criar contas, realizar login, fazer reservas e visualizar o histórico de alugueis.
- **REQ04**: Registro de reservas feitas pelos usuários, com dados sobre o carro, data de início e fim, preço e status de pagamento.

### Operações de Aluguel
- **REQ05**: Busca de carros disponíveis para aluguel com filtros por tipo, modelo, preço e data de disponibilidade.
- **REQ06**: Realização de reserva de carros, incluindo o cálculo do preço total baseado na duração do aluguel, possíveis taxas adicionais e seguro.
- **REQ07**: Pagamento de reservas, com suporte para diferentes formas de pagamento (cartão de crédito, débito, etc.).
- **REQ08**: Cancelamento de reservas, com possibilidade de reembolso parcial ou total dependendo das políticas de cancelamento definidas.

### Gerenciamento de Carros
- **REQ09**: Adição, edição e remoção de carros do sistema pelo administrador, com informações sobre o carro, preço, disponibilidade e características.
- **REQ10**: Acompanhamento de reservas de carros em tempo real, incluindo controle de devoluções de veículos.

### Consultas e Relatórios
- **REQ11**: Consulta de carros disponíveis para aluguel em uma data específica.
- **REQ12**: Relatório de reservas realizadas, incluindo dados sobre os carros alugados, valores pagos e clientes.
- **REQ13**: Relatório de rendimento do sistema com detalhes sobre o faturamento gerado pelo aluguel dos carros.

### Validações e Controle
- **REQ14**: Validação de disponibilidade de carros para o período solicitado, com atualização automática de status quando o carro for reservado ou devolvido.
- **REQ15**: Controle de estado de devolução do carro, com verificação de danos ou irregularidades durante a devolução.

## Possíveis APIs/Bibliotecas a serem usadas
- **Google Maps API**: Para exibição de locais de retirada e devolução de carros, oferecendo geolocalização precisa dos pontos de aluguel.
- **iText ou Apache POI**: Para geração de relatórios em PDF ou Excel, como históricos de reservas e faturamento.
