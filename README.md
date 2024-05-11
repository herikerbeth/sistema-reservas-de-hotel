# Sistema de Reservas de Hotel

## Descrição

Sistema de software para a gestão de reservas de quartos online, incluindo a precificação das diárias e produtos disponíveis para consumo, bem como o pagamento dessas diárias e produtos consumidos pelos respectivos clientes.

## Requisitos

### Requisitos funcionais (RF)

|||
| --- | --- |
| RF 1  | O sistema deve permitir que os clientes realizem reservas de quartos online ou por contato telefônico com a recepção da pousada.  |
| RF 2  | O sistema deve permitir que um cliente realize uma reserva somente se estiver cadastrado, podendo o referido cadastro ocorrer de forma online ou por contato telefônico.  |
| RF 3 | Quando o cliente realiza uma reserva online, o sistema realiza a cobrança de uma diária no cartão de crédito para confirmação da reserva. |
| RF 4 | Quando o cliente realiza uma reserva por meio telefônico, o sistema exige uma pré-reserva para confirmação da reserva. Nesse caso, a recepção realiza a validação (inclui o registro do valor depositado) ou cancelamento da pré-reserva. |
| RF 5 | O cliente pode cancelar uma reserva. |
| RF 6 | O sistema deve permitir a precificação das diárias dos quartos das pousadas pelo setor administrativo da empresa. |
| RF 7 | O sistema deve permitir a precificação dos produtos disponíveis para consumo pelos clientes pelo setor administrativo da empresa. |
| RF 8 | O sistema deve interagir com um sistema terceirizado (operadora de cartão crédito) para pagamentos com cartão de crédito. |
| RF 9 | Os consumos de produtos por parte dos clientes devem ser registrados pelos atendentes de bares e cozinha das pousadas. |
| RF 10 | Os funcionários do setor administrativo da empresa mantêm atualizados os registros necessários à realização de reservas, ou seja, funcionários, pousadas, quartos. |
| RF 11 | A quitação da reserva, realizada pela recepção da pousada e somente com cartão de crédito, deve ocorrer no check-out. |
| RF 12 | O setor administrativo gera relatórios periódicos das ocupações dos quartos das pousadas. |
| RF 13 | O gerente da pousada gera relatórios periódicos de ocupação dos quartos da pousada. |

### Requisitos Não Funcionais (RNF)

|||
| --- | --- |
| RNF 1 | O sistema deve utilizar tecnologia WEB. |
| RNF 2 | O SGBD adotado é o PostgreSQL. |
| RNF 3 | A linguagem de programação para desenvolvimento adotada é Java, sendo a IDE IntelliJ. |
| RNF 4 | O framework para o mapeamento objeto-relacional é o Hibernate. |
| RNF 5 | O framework para o desenvolvimento de aplicações web adotado é o Spring Boot. |
| RNF 6 | O padrão de arquitetura adotado é o MVC (model-view-controller). |
| RNF 7 | O processo de desenvolvimento de software adotado é o Scrum. |
| RNF 8 | O prazo estimado do projeto de software é de 04 (quatro) meses. |
| RNF 9 | Atributo de qualidade crítico a ser considerado na seleção de um provedor de serviço na nuvem e de internet: confiabilidade. |

### Regras de Negócio (RN)

|||
| --- | --- |
| RN 1 | Uma reserva é realizada por um único cliente. |
| RN 2 | Uma reserva pode incluir no mínimo 01 (um) quarto e no máximo 03 (três) quartos disponíveis no momento da reserva. |
| RN 3 | A pré-reserva exigida na reserva por meio telefônico impõe um depósito bancário, por parte do cliente, correspondente a 40% do total da reserva na conta da respectiva Pousada. Nesse caso, a validade ou cancelamento da reserva é realizada pela recepção. O cliente tem o prazo de 24h para envio do recibo de depósito via WhatsApp ou SMS. |
| RN 4 | O cancelamento de uma reserva pode ser realizado até 24h antes da data de check-in estabelecida na reserva. |
| RN 5 | No caso de cancelamento da reserva realizada por telefone, o valor da pré-reserva é estornado ao cliente. |
| RN 6 | No caso de cancelamento por período menor que 24h, ou não comparecimento, será cobrada uma diária. |
| RN 7 | Uma reserva realizada online somente é confirmada após a autorização da operadora de cartão (sistema terceirizado). |
| RN 8 | Os consumos de produtos por parte dos clientes são pagos no momento do check-out, com o valor restante das diárias. |
| RN 9 | O check-in é realizado a partir de 15h e o check-out, até 12h. |
| RN 10 | O sistema deve permitir o pagamento da reserva online e no check-out somente com cartão de crédito. |

## Diagramas UML

### Diagrama de Casos de Uso


