# Forja de Fichas

Aplicação web para criação de fichas de personagens e organização de campanhas de RPG de mesa. Reúne modelos de fichas, editor de campos, rolagens de dados e painéis específicos para mestre e jogador.

## Tecnologias

- HTML5 e CSS3, com layout responsivo e temas claro e escuro.
- JavaScript e React 18, carregado via CDN.
- `localStorage` para persistência local de fichas e dados de campanhas.
- Navegação por hash (`#inicio`, `#campanhas`, `#mestre`, `#jogadores` e `#fichas`).

O protótipo atual está organizado em um único arquivo `index.html`. Não exige instalação de dependências nem processo de build. A conexão com a internet é necessária para carregar as bibliotecas e fontes externas.

## Como executar

1. Baixe ou clone o repositório.
2. Abra `index.html` em um navegador atualizado com conexão à internet.
3. Navegue pelas seções do site e experimente as campanhas e fichas de exemplo.

## Funcionalidades atuais

### Página inicial

- Apresentação do projeto e navegação entre as áreas.
- Rolador de d20 com animação, indicador do resultado e histórico das rolagens anteriores.
- Acesso aos modelos de ficha e prévia de até três campanhas.

### Campanhas

- Formulário de criação com título, descrição, sistema, tom, nível inicial, quantidade de vagas, frequência, status, data, horário e acordos da mesa.
- Identificação de participação como mestre ou jogador nas campanhas de exemplo.
- Filtros por participação: todas, mestre e jogador.
- Visualizações normal e compacta, com cartões de tamanho padronizado, texto truncado e paginação.
- Campanhas criadas no navegador integradas à listagem e ao painel do mestre.

### Área do mestre

- Listagem das campanhas em que o perfil de exemplo é mestre, com dois modos de visualização e paginação.
- Painel individual por campanha com visão geral, sessões, jogadores, NPCs, combates, roteiro, locais, anotações e configurações.
- Edição local de dados de sessões, participantes, personagens, NPCs e locais.
- Controle de iniciativa, turnos e pontos de vida para encontros.

### Área dos jogadores

- Listagem das campanhas em que o perfil de exemplo participa como jogador, com modos normal e compacto e paginação.
- Painel da campanha com ficha em três colunas, visão geral, sessões, grupo, diário e rolador de dados.
- Ficha de exemplo com identificação do personagem, retrato, atributos, recursos, perícias, ataques, habilidades, inventário e descrição.
- Rolagens de atributos, perícias e danos, com histórico na ficha.

### Fichas

- Criação de fichas com modelos de D&D 5e, Ordem Paranormal, Sobrevivendo ao Horror, Tormenta20 e ficha em branco.
- Editor de seções e campos, incluindo atributos, barras de recursos, perícias, tabelas, listas de opções e campos calculados.
- Preenchimento de fichas, duplicação, exclusão e salvamento automático local.
- Backup e importação das fichas em formato JSON.

## Armazenamento

Os dados editáveis são salvos no `localStorage` do navegador. Campanhas, mestres e jogadores de exemplo compõem uma demonstração local; não há autenticação de contas nem sincronização entre dispositivos. A organização de campanhas e permissões na interface não corresponde a um controle de acesso em servidor.

## Registro de entregas

O arquivo [ROADMAP.md](ROADMAP.md) relaciona apenas as etapas já implementadas no protótipo.