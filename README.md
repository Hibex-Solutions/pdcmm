# PDCMM - Purely Digital Company Management Model

> Em português: Modelo de Gestão de Empresa Puramente Digital.

PDCMM é um padrão para documentar os processos de gestão de uma empresa
puramente digital, criado por _Hibex Solutions_ para documentar seus próprios
processos e disponibilizar a seus colaboradores, e de forma gratuita sobre os
termos da [Licença Apache - versão 2.0](./LICENSE) a quem desejar implementar o
padrão em suas próprias empresas.

## Definição de empresa puramente digital

Entendemos por uma empresa puramente digital, a que oferece produtos ou
serviços que não são físicos desde o nascimento, ou seja, já naceram como
serviços digitais. Portanto precisam gerenciar seus serviços e produtos tendo
como base as plataformas digitais de software.

Desde seus produtos e serviços, o gerenciamento de seus colaboradores, os
trabalhos realizados por eles, o processo de produção, entrega e suporte a
usuários finais, além da gestão de campanhas de marketing, e tudo mais que seja
necessário para funcionamento da empresa; tudo é feito através do uso de
software, sejam próprios ou de terceiros.

Isso nos revela que o mundo do software é real a essas empresas desde o seu
nascimento, e permanecerá dessa forma nos dias que se seguem. Para essas
empresas, o software não é um luxo ou complemento a necessidades, mas trata-se
da sua realidade e existência.

Essa é uma **"Empresa Puramente Digital"** _(Purely Digital Company)_.

## A proposta PDCMM

A proposta é que tais empresas devem não somente gerenciar seus artefatos de
softwares e documentos de forma digital, mas o seu próprio modelo de gestão
deve ser paupável digitalmente também. Basicamente toda a propriedade
intelectual é digital, e compreende seu inventário de softwares, processos e
todas as informações relevantes para a manutenção da empresa.

PDCMM é uma forma de estruturar essas as informações digitais e
disponibilizá-las de forma transparente, segura e bem documentada aos
colaboradores de uma _Empresa Puramente Digital_.

## Como implementar PDCMM?

A implementação de PDCMM em uma empresa consiste em seguir 3 (três) simples passos:

### 1. Concordar com o conjunto de definições PDCMM

Quando você disponibiliza este _Conjunto de Definições PDCMM_ de forma explícita
em sua estrutura, você está concordando com elas.

### 2. Disponibilizar a documentação PDCMM aos colaboradores

A documentação PDCMM é a junção deste guia, mais a documentação de
implementação das definições (que é próprio de cada empresa). Juntos formam
a _documentação PDCMM_, e essa documentação deve estar disponível a todos os
colaboradores, independente da função na empresa.

### 3. Seguir todas as definições da documentação PDCMM

O ato de seguir as definições é uma questão cultural da empresa, e a forma como
isso é validado também é próprio de cada empresa, porém isso estará definido na
documentação de implementação. Portanto, a documentação de implementação do
PDCMM deve expor as recomendações e regras de implementação, bem como a forma
de validar se tais recomendações e regras estão sendo seguidas adequadamente.

Quando é possível validar o seguimento das recomendações e regras, também é
possível validar que este passo 3 (três) está em conformidade, e isso é o que
certifica um PDCMM devidamente implementado.

## O Guia PDCMM

O PDCMM de uma empresa é o conjunto de documentos digitais, incluindo este guia,
mas também todas suas referências, histórico de mudança nos documentos,
histórico de registros de ações internas, além da própria cultura da empresa ao
seguir as as definições PDCMM.

> O PDCMM de uma empresa pode ser interpretado como seu _inventário de
> propriedade intelectual digital_.


Este guia definie o que é um PDCMM e contém 7 (sete) definições formais, cada
uma com um conjunto de asserções que certificam como validar uma implementação.

Porém, este guia, propositalmente não define como implementar as definições em
si. Ao invés disso, deixa a cargo de cada empresa complementar o PDCMM, com a
disponibilização de um documento de implementação para cada uma das 7 (sete)
definições. Esse conjunto de documentos de implementação são chamados de
**"documentação de implementação PDCMM"**.

Portanto uma empresa deve unir este guia a seus documentos de implementação, e
juntos formarão o que a **"documentação PDCMM"**.

## As definições PDCMM

A seguir temos a descrição de 7 (sete) definições, e para cada uma, um conjunto
de asserções que certificam a definição.

Na descrição de cada definição também temos os nomes dos documentos que devem
descrever sua implementação e a validação das asserções relacionadas na _documentação PDCMM_ final.

*Uma asserção* é uma frase que deve ser considerada verdade sempre.

*Um documento de validação de asserção* descreve os passos necessários para
validar se de fato a asserção é verdadeira no contexto validado, e portanto,
são os passos para certificação da definição.

Seguem as 7 (sete) definições.

### Definição 1 - Tudo é digital

Sejam documentos (fiscais ou não), código de software, registros e cadastros; todos devem ser
armazenados de forma digital. O armazenamento deve ser de propriedade da empresa, portanto
deve ser possível fazer backup para armazenamento periódico, pois uma empresa puramente digital
deve ter a propriedade de todos os seus artefatos.

Dê preferência a arquivos digitais legíveis, ou seja, onde seja possível abrir e visualizar o
conteúdo em um editor de textos simples, sem necessidade de auxílio de qualquer outra ferramenta,
seja ela paga ou gratuita. Ainda que a própria empresa desenvolva softwares específicos para
o fim de editar e visualizar seus próprios artefatos, recomendamos sempre o uso legível da
informação. Porém os formatos binários são inevitáveis, mas devem estar restritos a situações
onde não seja possível usar formatos legíveis. Em alguns casos você pode manter um formato legível
simples, e usar ferramentas para gerar versões binárias para distribuição. Quando possível
essa abordagem é recomendada.

#### Implementando a definição 1

**USE SEMPRE DOCUMENTOS DIGITAIS E MANTENHA SEUS ARQUIVOS EM UM LOCAL CENTRALIZADO**.

- Use um serviço de armazenamento em nuvem, e centralize os dados em um único local
- Faça backup periódico para mídias físicas que estejam sobre propriedade da empresa

### Definição 2 - Tudo deve ter histórico armazenado

Toda mudança nos arquivos e documentos que compreendem o inventário tecnológico deve ser
registrada. Isso permite não apenas uma auditoria futura, mas também identificar cenários
importantes que indiquem não só falhas, mas oportunidades. A qualquer momento pessoas com acesso
aos mecanismos de registro podem procurar por padrões ou encontrar falhas e assim corrigir
defeitos nos processos, produtos e outros. O histórico de evolução é um artefato digital valioso!

Toda criação, remoção e alteração em arquivos/documentos da empresa deve ser registrada.

#### Implementando a definição 2

**ARMAZENE TUDO EM REPOSITÓRIOS GIT**

> Use [Git Large File Storage](https://git-lfs.com) para arquivos grandes e binários

Você também pode usar outros mecanismos, por exemplo: Se usar Google Drive ou serviços de
armazenamento na nuvem, eles já tem o histórico de modificações embutidos. Porém nesses casos
você precisa garantir que seus backups também contenham o histórico e não só o conteúdo dos arquivos.

> A "Definição 2" depende da "Definição 1" e também a implementa

### Definição 3 - Toda propriedade da empresa deve estar catalogada

Assume-se que a propriedade é da empresa e não das pessoas que a gerenciam. Portanto, quando
a gestão muda, os dados devem estar disponíveis imediatamente e de forma transparente aos
novos gestores.

- Todas as assinaturas de serviços pertencentes a empresa são registradas com informações relevantes
- As informações sensíveis não estão disponíveis a todos, mas é referenciada no catálogo geral
  para que se saiba onde encontrar, pois também é uma informação de propriedade da empresa

#### Implementando a definição 3

A primeira propriedade da empresa é esta documentação PDCMM, e portanto fará parte de seu
inventário.

Precisamos de um repositório Git chamado `company`, ele conterá esta definição como documentação
além de outros documentos e todo o inventário digital, seja diretamente ou referenciado.

Esta definição estará armazenada como `docs/pdcmm-definition.md`.

Para inventário deve haver um arquivo nomeado `inventory/README.md`, que conterá um índice de
inventário digital. O inventário digital deve estar descrito de forma resumida ou indexada
neste arquivo porém devem existir outros arquivos que o complementem.

Como existem vários tipos de inventário, inclusive financeiros, fiscais, tecnológicos, etc.
Nem tudo deve estar totalmente legível a todos, pois podem existir dados "secretos". Para tal
podem haver dentro do diretório de inventário referência a outros repositórios Git como
submódulos, como: `inventory/accounting` para dados contábeis ou ainda `inventory/financial`
para dados financeiros.

Quando repositórios de inventário, tais devem ser nomeados com o prefixo `company-inventory`.
Ex: `company-inventory-accountin` e `company-inventory-financial`.

Exemplos de registros de inventário:

- Uma conta de serviço na AWS em nome da empresa
- Uma conta bancária aberta em uma instituição financeira em um CNPJ da empresa
- Um registro de domínio em um provedor DNS qualquer
- Assinatura no Google Workspace ou Azure DevOps
- Assinatura de softwares auxiliares
- Aquisição de computadores
- Balanço financeiro e fiscal anual/mensal

Quanto ao inventário, não apenas as informações de registro são importantes, mas também os
dados sensíveis relacionados a cada registro, como:

- Chaves de sistema operacionais para computadores adquiridos
- Nomes de usuários, senhas e segredos para serviços contratados

Caso existam softwares proprietário para gestão desses inventários, ou outros mecanismos para tal,
a aplicação deve residir no repositório do inventário, ou deve ser referenciado lá.

> A "Definição 3" depende da "Definição 2", pois espera-se que toda movimentação seja registrada.

### Definição 4 - A composição dos colaboradores deve estar catalogada

O registro das informações essenciais de todos os colaboradores deve estar disponível para consulta
por qualquer outro colaborador, tanto o presidente quanto a todos os demais. Nenhuma informação
além da identificação deve estar disponível, como dados estritamente pessoais, como número de
documentos, endereços, etc., mas apenas a identificação do colaborador e sua alocação nos diversos
times e departamentos da empresa, para que seja possível uma comunicação sempre que possível.
Isso é útil para evitar burocracias desnecessárias que podem impedir a fluidez do negócio.

Sempre que houver movimentação dos colaboradores entre os times, ou suas funções, além de qualquer
marco (memorandos) importante na passagem do colaborador pela empresa, isso deve estar registrado.

#### Implementando a definição 4

Deve existir um repositório Git para armazenar informações de colaboradores, e este repositório
deve ser referenciado como um submódulo Git em `collaborators/`. O repositório deve conter pelo
menos um arquivo `README.md` para esses registros, mas pode estar distribuídos em outros arquivos
e diretórios dentro do repositório, desde que sejam mapeados em `collaborators/README.md`.

Caso exista um software proprietário para essa gestão, ou outros mecanismos para tal, esses devem
residir no repositório de colaboradores, ou deve ser referenciado lá.

O repositório de colaboradores deve ser nomeado como `company-collaborators`.

### Definição 5 - Todos os produtos e serviços devem estar catalogados

O processo de criação dos produtos da empresa devem seguir padrões bem especificados e documentados.
Cada produto, já pronto ou em desenvolvimento, ou ainda em idealização, deve residir em um local
específico e ter todo seu histórico consultável.

#### Implementando a definição 5

Deve existir um repositório Git para armazenar informações de produtos, e este repositório
deve ser referenciado como um submódulo Git em `products/`. O repositório deve conter pelo
menos um arquivo `README.md` para descrever os produtos.

Cada produto pode ter seu próprio repositório, mas esses repositórios devem estar mapeados
como submódulos Git nesse repositório de produtos, e também devem ser mapeados no arquivo
`README.md`, portanto `/products/README.md`.

Espera-se que cada produto tenha suas especificações e documentações relevantes em si mesmo,
porém, essas documentações também podem ser referenciadas em um repositório global de
documentações `/docs` na raiz deste repositório central.

O repositório de produtos deve ser nomeado como `company-products`.

> Muitas vezes trata-se de uma plataforma de software, e neste caso o repositório de
> produtos é na verdade a descrição de um produto de plataforma.

Quando a empresa tiver apenas um produto principal, ele será sua plataforma de software,
então deve existir um repositório para o produto de plataforma, e este deve estar no
subdiretório de produtos com o nome `/products/platform`.

Quando existirem vários produtos de software distribuídos entre os times da empresa,
mesmo assim devem ser consolidados em um repositório de plataforma, de forma que
`/products/platform` sempre existirá como produto central, e ele deve referenciar todos
os demais produtos de software que compõem a plataforma.

> TODO: Incluir referência a documentação sobre "estrutura de projetos de plataforma"

### Definição 6 - Os colaboradores devem saber lidar com dados sensíveis

- Todo colaborador deve dominar a técnica de compartilhamento de dados sensíveis
- Toda a técnica de compartilhamento deve ser documentada
- Devem haver revisões de conhecimento periódicos sobre conhecimento dos colaboradores
- Os dados sensíveis devem ser armazenados de forma protegida
- O processo de proteção deve ser documentado
- Os dados devem ser encontrados pela documentação ainda que não possam ser acessados
- O acesso aos dados deve estar disponível em camadas
- Todo dado protegido deve ser acessível por pelo menos 1 (um) meio alternativo sobressalente
- Dados devem ser categorizados por níveis de sigilo
  - Cada nível de sigilo deve exigir passos extras para acesso/armazenamento
  - O último nível de acesso sobressalente "nunca deve ser digital", mas físico
  - Todo acesso sobresalente físico deve existir em mais de uma cópia
  - Todo dado chave de segurança/proteção deve passar por inspeções e validações periódicas

### Definição 7 - As asserções devem ser certificadas interna e periodicamente
