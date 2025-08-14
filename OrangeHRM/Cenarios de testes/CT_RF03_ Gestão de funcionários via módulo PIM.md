## Cenário 03: Gestão de funcionários via módulo PIM.

### Caso de Teste 01: Adicionar novo funcionário com dados válidos.

| ID       | Descrição                                                          |
| :------- | :----------------------------------------------------------------- |
| C03-CT01 | O sistema deve permitir o cadastro de um funcionário com dados válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo PIM.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** clica em \"Add Employee\"                                  |
| **E** preenche \"John\" no campo First Name e \"Doe\" no Last Name |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o funcionário deve ser cadastrado e exibido na lista do PIM |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário deve aparecer corretamente listado no módulo PIM. |

Teste passou com sucesso.
https://jam.dev/c/208968ce-ba00-4d36-a8c6-2b4de870f002
---

### Caso de Teste 02: Tentar adicionar funcionário sem preencher campos obrigatórios.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C03-CT02 | O sistema deve exibir erros ao tentar salvar um funcionário sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa a tela de \"Add Employee\"          |
| **E** deixa os campos obrigatórios em branco                     |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas nos campos obrigatórios |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |

Teste passou com sucesso.
https://jam.dev/c/0b7daf92-7f06-4554-ae4b-74daa6f243bc
---

### Caso de Teste 03: Pesquisar funcionário já cadastrado.

| ID       | Descrição                                                  |
| :------- | :--------------------------------------------------------- |
| C03-CT03 | O sistema deve retornar corretamente o funcionário pesquisado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O funcionário deve já estar cadastrado no sistema.            |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** digita \"John Doe\" no campo de busca                      |
| **QUANDO** clicar no botão \"Search\"                            |
| **ENTÃO** o sistema deve exibir \"John Doe\" na lista de resultados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário correspondente deve ser listado corretamente.     |

Teste passou com sucesso.
https://jam.dev/c/def2ccf1-21f3-4385-8b1a-2e564d67f17b
