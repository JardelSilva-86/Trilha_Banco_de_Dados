# Primeiro Curso da Trilha - Modelagem de Dados

## Conceito
É uma metodologia utilizada para determinar as Regras de Negócio (RN) e a arquitetura de um Banco de Dados (BD), ou seja, descreve as estruturas lógicas e físicas do BD.

Modelo de tarefa do usuário - Definição de regras e tecnologia - Relatório descritivo do processo da tarefa do ponto de vista do usuário.

Modelo Conceitual - Regras de negócio - Ferramentas ou objetos, propriedades, técnicas, processos, mapeamentos do domínio do usuário

Modelo Lógico - Definição de regras e tecnologia - Definição de dados, funções e projetos de regras.

Modelo Físico - Implementação - Pode representar tanto o projeto como a própria interface gráfica, o banco de dados e os programas.

### Minimundo ou Regras de Negócio (RN)
É a criação de um documento com um adescrição textual curta, que acontece a partir de determinadas informações. Nele é descrito os dados de como as coisas devem funcionar. Ou seja, o minimundo é um primeiro modelo desenvolvido para entender os conceitos da realidade.
É um pedaço de realidade do qual o analista levantou certos detalhes. Ao revelar o interesse em realizar a gestão, seria possível fracionar o minimundo em porções menores, dependendo da sua complexidade, para melhor analisá-lo.

Minimundo é a esquematização da realidade


### Abstração
É a visão que surge mentalmente com base em qualquer realidade. Assim, o ato de abstrair consiste no processo mental para selecionar características de objetos e situações, sendo que algumas serão excluídas por não apresentarem relevência ao contexto.
É o modo de retratar os conceitos implícitos nos requisitos (tirados do minimundo) do projeto de BD de um software. 

Abstração é a representação mental dessa realidade.

## Sistema de Gerenciamento de Banco de Dados (SGBD)
É essencial que qualquer SGBD tenha, pelo menos, 4 elementos: Softwares, dados, usuários e hardware.

### Software
Está entre os usuários e o banco de dados físico (dados armazenados), há uma camada de software (programa de aplicação), sendo este o SGBD.

### Dados
São todas as informações armazenadas em um banco de dados.

### Hardware
Refere-se aos volumes de memória secundária (tambores, discos etc.) em que se encontra o banco de dados junto com os dispositivos a ele vinculados, como canais, unidades de controles, entre outros.

### Usuários
Existem três tipos principais, estando no topo o programador (usuário que escreve os programas de aplicação que utilizam o banco de dados); seguido de outro final (tem acesso a um terminal, podendo usar uma linguagem de consulta ou fazer uma chamada para uma aplicação, realizando todas as funções de recuperação, criação, eliminação ou alteração); e, para finalizar, há o usuário que é o administrador do banco de dados, também conhecido como DBA.

## Banco de Dados
É um repositório para armazenar informações (dados) de qualquer natureza. Ele retrata aspectos do mundo real - ou seja, o conceito visto anteriormente de minimundo - em que qualquer mudança que se faça no minimundo é diretamente replicada no banco de dados.

## Persistência
Consiste no armazenamento confiável e coerente das informações em um sistema de armazenamento de dados. Os dados persistem quando são aceitos pelo SGBD para a inserção no banco. Assim, somente será possível removê-los do banco, posteriormente, por meio de alguma solicitação explícita ao SGBD.

## Categoria de BD

### Centralizada
Arquitetura em um servidor em que as aplicações ou os clientes podem acessar o banco de dados. Logo, a responsabilidade pela capacidade de armazenamento e resposta será assumida. Para tal modelo, é necessário alto poder de processamento do servidor e um ótimo desempenho do SGBD.

### Descentralizada
Há mais de um servidor para o banco de dados, possibilitando que eles sejam descentralizados. Tem-se, então, garantia de autonomia local e auxílio na comunicação, que, por exemplo, pode ser melhor distribuída entre as aplicações que utilizam tabelas específicas.

### Distribuída
Arquitetura em que os dados estão compartilhados em muitos computadores ou servidores, com utilizações ou sincronismo para se certificar da integridade desses dados nos locais em que se encontram.

### Replicada 
Arquitetura em que o banco de dados é copiado para muitos computadores ou servidores, como em uma metodologia de espelhamento. Todos os bancos são idênticos e, conforme há alterações no primeiro banco, os demais são alterados em cascata.
Aliás, esse tipo de arquitetura garante a segurança das informações. No caso de haver falhas em algum host, outro poderá assumir seu lugar, visto que os dados são idênticos.

## Modelo Conceitual

Utiliza a análise de requisitos por base, sendo um grupo de hipóteses que leva em conta o mundo real, indicando as regras de negócio do sistema. Desse modo, consiste no detalhamento de alto nível, voltado a entender e descrever todos os detalhes de uma organização.
Este detalhamento das informações de negócio, por sua vez, é guardado no banco de dados. 

### Objetivo

- Implementar sistema com informações coerentes
- Relacionamentos
- Propriedades
- Objetos

# Modelo Lógico

Cria um modelo lógico somente quando a etapa anterior - Modelo Conceitual - for concluída. Desse modo, apresenta questões referente às possibilidades de abordagem tecnológicas do SGBD, para criar a lógica dos relacionamentos que há no modelo conceitual.