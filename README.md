# AtividadeProgSem5


# O que é o Cypress e para o que ele serve ?

Podemos dizer que ele é uma ferramenta de testes End to end para aplicações web mais modernas, ele foi projetado para tornar a execução, escrita e dupração de testes mais rapida e eficiente. Ele ajuda muito a automação de tarefas, como intetagir com elementos da pagina, simular comportamentos do usuario e entre outros.

# Vantagens

•⁠  ⁠Sua arquitetura excluisava, o que permite uma experiencia de testes bem consistente e confiavel. Ele opera no mesmo ciclo de execucao que a aplicacao.

•⁠  ⁠Execucao de testes de forma mais rapida se for comparado com outras ferramentas disponiveis no mercado

•⁠  ⁠Suporte a estruturas de javascript mais modernas, como angular, react e vue

# Desvantagens

•⁠  ⁠Possue um suporte limitado para execucao em multiplas janelas

•⁠  ⁠Limitação da sua linguagem, onde ele suporta apenas javascript, o que pode ser ruim caso outra linguagem seja utilizada

•⁠  ⁠Foco em testes E2E, para certos casos pode ser vantagem isso porem pode acabar limitando o seu uso em cenarios que exigem coisas além de end-to-end

# Arquitetura

A sua arquitetura é diferente das ferramentas de teste tradicionais, ele é executado dentro do navegador, o que fornece um controle direto sobre o DOM, armazenamento e eventos. A sua arquitetura é difeA sua arquitetura é baseado em uma arquitetura exclusiva chamada "Execution Runner" que consiste em tres partes : 

•⁠  ⁠Cypress Application: A interface gráfica do usuário que permite escrever, executar e depurar testes. 

•⁠  ⁠Cypress Test Runner: Um servidor Node.js que orquestra a execução dos testes.

•⁠  ⁠Cypress Browser: Uma instância dedicada do navegador onde os testes de fato executados.

# Seletores de elementos

O cypress ofecere uma quantidade muito grande de possiveis seletores para elementos na página, vou listar alguns deles : 

- Seletores de css, como .class ou #id
- seletores de atributos como [attr=value]
  
Entre outros como, cy.find(), cy.contains()

# Comandos e asserções

Os Comandos são utilziados para interagir com os elementos da pagina, como botoes, digitar campos de entrada e navagar entre as paginas, alguns comandos mais comuns como : 

-cy.visit(url): Navega para uma página
-cy.click(): Clica em um elemento
-cy.type(text): Digita texto em um campo de entrada

Já as asserções são usadas para verificar se um elemento ou uma aplicação está no estado que ela deveria estar, alguns comandos são : 

- should('exist'): Verifica se o elemento existe
- should('contain', text): Verifica se o elemento contém o texto especificado
- should('have.class', className): Verifica se o elemento possui uma classe específica

# Preparação, Execução e Verificação de Testes no Cypress

## Preparação 

- Criar um novo projeto ou integrar o Cypress em um projeto existente
- Definir a estrutura de pastas e arquivos para os testes
- Configurar ambientes (se necessário) e instalar dependências

## Execução

- Escrever testes descrevendo os cenários de teste
- Navegar para a página ou aplicação a ser testada
- Interagir com elementos da página usando comandos do Cypress
- Simular entradas de usuário e comportamentos
- Executar os testes com o Cypress Test Tunner

## Verificação

- Usar asserções para verificar o estado esperado da aplicação
- Validar a presença ou ausência de elementos, valores de campos, mensagens, etc
- Executar os testes e analisar os resultados

# Como estruturar testes de forma eficiente no Cypress?

Existem inumeras práticas recomendadas para estrutura os teste de uma maneira eficiente, vou listar as que julgo mais importantes : 

- Fazer a utlizacão de 'describe' para agrupar testes relacionados e 'it' para testes individuais, sempre com uma descricao clara sobre o que cada teste está verificando

- Sempre agrupar testes relacionados um ao outro em arquivos especificos e unicos

- Sempre promover a modularidade criando funções reutilizáveis para tarefas comuns, como login, navegação e preenchimento de formulários.



