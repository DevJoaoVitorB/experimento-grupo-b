# Instruções de Segurança

## RS01 — Controle de acesso e autorização

> O acesso aos recursos protegidos da API deve ser negado por padrão e permitido somente quando o usuário possuir autorização para a operação solicitada, considerando sua identidade e sua relação com o recurso, impedindo o acesso ou alteração de recursos de outros usuários por meio da manipulação de identificadores ou parâmetros da requisição, além de garantir que os mecanismos de acesso sejam invalidados após o encerramento da sessão.

## RS02 — Configuração segura da aplicação

> A API não deve manter informações sensíveis, como credenciais, chaves ou segredos de autenticação, diretamente no código-fonte, devendo utilizar configurações adequadas ao ambiente de execução, manter desabilitados recursos, funcionalidades, contas e componentes desnecessários e evitar que mensagens de erro exponham detalhes da implementação, caminhos, stack traces ou outras informações internas da aplicação.

## RS03 — Gerenciamento seguro de dependências

> As dependências diretas e transitivas utilizadas pela API devem ser mantidas sob controle e verificadas quanto à existência de vulnerabilidades conhecidas, evitando versões vulneráveis, desatualizadas ou sem suporte quando houver versões corrigidas disponíveis e identificando e tratando os riscos relacionados aos componentes utilizados pela aplicação.


## RS04 — Gerenciamento seguro das credenciais

> As senhas dos usuários não devem ser armazenadas em texto puro, devendo ser protegidas por mecanismos criptográficos adequados que impeçam a obtenção direta de seu conteúdo original a partir dos dados armazenados, evitando mecanismos criptográficos fracos, obsoletos ou inadequados e impedindo que credenciais ou informações relacionadas às senhas sejam expostas nas respostas da API ou em outros dados disponibilizados ao cliente.

## RS05 — Validação dos dados de entrada

> Todos os dados recebidos pela API devem ser considerados não confiáveis até serem devidamente validados, incluindo dados presentes no corpo, parâmetros, cabeçalhos e demais entradas das requisições, de modo que entradas inválidas, inesperadas ou incompatíveis sejam rejeitadas e não possam alterar a estrutura ou o significado de consultas, comandos ou operações executadas pela aplicação.

## RS06 — Proteção da autenticação

> A API deve permitir a autenticação somente mediante credenciais válidas, protegendo o processo contra tentativas automatizadas e repetidas de acesso, evitando credenciais fracas, conhecidas ou comprometidas quando identificáveis, não revelando informações que permitam determinar indevidamente a existência de usuários ou credenciais e garantindo que funcionalidades protegidas dependam de uma autenticação válida e que o mecanismo de autenticação deixe de ser utilizável após o encerramento da sessão.

# RS07 — Tratamento seguro de condições excepcionais
> A API deve tratar adequadamente erros e condições excepcionais durante a execução, garantindo que falhas inesperadas sejam tratadas de forma controlada, sem expor informações internas da aplicação, como stack traces, detalhes de consultas ou mensagens sensíveis, e que as respostas de erro não comprometam a segurança, a consistência dos dados ou o funcionamento da aplicação.
