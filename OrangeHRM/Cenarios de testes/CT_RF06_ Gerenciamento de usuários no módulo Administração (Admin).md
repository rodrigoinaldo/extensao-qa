## Cenário 06: Gerenciamento de usuários no módulo Administração (Admin).

### Caso de Teste 01: Adicionar um novo usuário com dados válidos.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C06-CT01 | O sistema deve permitir o cadastro de um novo usuário com informações válidas. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado com permissões de administrador.  |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o administrador acessa o menu \"Admin\"             |
| **E** clica em \"Add\"                                           |
| **E** preenche os campos obrigatórios como \"Employee Name\", \"Username\" e \"Password\" |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o novo usuário deve ser cadastrado e listado corretamente |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O usuário cadastrado deve aparecer na lista de usuários ativos. |

Teste aprovado e homologado

[Video](https://jam.dev/c/a63dffa1-0622-4eaa-9a8a-356f11b8f3f6)
---

### Caso de Teste 02: Tentativa de adicionar usuário com nome de usuário já existente.

| ID       | Descrição                                                                       |
| :------- | :------------------------------------------------------------------------------- |
| C06-CT02 | O sistema deve impedir o cadastro de um novo usuário com nome de usuário duplicado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Já deve existir um usuário com o mesmo nome de usuário.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o administrador acessa o menu \"Admin\"             |
| **E** clica em \"Add\"                                           |
| **E** insere um nome de usuário que já existe                   |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** uma mensagem de erro \"Already exists\" deve ser exibida |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve impedir o cadastro e exibir mensagem de duplicidade. |

Teste aprovado e homologado

[Video](https://jam.dev/c/1d786fb7-2006-4adf-87d4-b4a8e700fde3)
---

### Caso de Teste 03: Filtrar usuários por status "Enabled".

| ID       | Descrição                                                      |
| :------- | :------------------------------------------------------------- |
| C06-CT03 | O sistema deve exibir apenas usuários com status "Enabled" ao aplicar o filtro. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| Deve haver usuários com diferentes status (Enabled e Disabled). |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o administrador acessa o menu \"Admin\"             |
| **E** seleciona \"Enabled\" no campo \"Status\"                 |
| **QUANDO** clicar em \"Search\"                                  |
| **ENTÃO** apenas usuários com status \"Enabled\" devem ser exibidos na lista |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A lista deve conter apenas usuários com status "Enabled".       |

Teste aprovado e homologado

[Video](https://jam.dev/c/4ff08bc4-677e-46d2-8bc5-78f154931b32)
