# ponderada-prog-s5

É de conhecimento geral que a realização de testes no código é essencial para garantir que o produto será entregue com qualidade, porém, realizar umt este bem feito e com cobertura total não é uma tarefa de fácil entendimento. Pensando nisso, um homem resolveu criar o Cypress, com o intuito de que ele facilitasse o processo de realizar testes no código.

Pensando nisso, o Cypress é uma ferramenta de teste para front-end criada para a web moderna, que serve para testar de forma simples os possíveis caminhos que um usuário pode percorrer dentro da sua aplicação.

Só o fato do Cypress ser uma ferramenta mais simples e focada em ser fácil de implementar, já é uma grande vantagem, mas ele não se limita a ela. Ele possui muitas outras vantagens, como por exemplo:
- Velocidade de execução: possui uma execução rápida de testes, pois opera diretamente no navegador e tem acesso direto ao DOM. Isso elimina a necessidade de aguardar requisições de rede ou atrasos que podem ocorrer em outras ferramentas.
- Debugging Simples: oferece uma experiência de debug eficiente, permitindo que os desenvolvedores visualizem e interajam com o estado da aplicação durante a execução do teste. Isso facilita a identificação e correção de problemas.

Por outro lado, o Cypress também possui algumas desvantagens, sendo elas:
- Testes apenas no navegador: a ferramenta se concentra principalmente em testes no navegador, o que pode ser uma desvantagem se você precisar realizar testes de API ou testes de integração que envolvem componentes fora do navegador.
- Asserções limitadas: tem um conjunto limitado de asserções em comparação com algumas outras ferramentas de teste. Isso pode ser um problema se você precisar de assertividade mais avançada em seus testes.

A arquitetura do Cypress é totalmente inovadora, uma vez que a maioria das ferramentas de teste funciona fora do navegador e executa comandos remotos pela rede, enquanto o Cypress é exatamente o oposto, pois ele é executado no mesmo loop de execução do seu aplicativo. Pensando nisso, o Cypress controla todo o processo de automação, de cima a baixo, o que o coloca na posição única de poder entender tudo o que acontece dentro e fora do navegador. Isso significa que ele é capaz de fornecer resultados mais consistentes do que qualquer outra ferramenta de teste.

O Cypress, possui uma funcionalidade muito boa chamada “setores de elementos”. Esses, são áreas específicas da página web que apresentam um conjunto de elementos relacionados. Em outras palavras, ao escrever os testes, é possível agrupar comandos relacionados a elementos específicos em “setores”. Isso pode ser útil para organizar seu código de teste de maneira mais clara e modular. Cada setor pode representar uma parte funcional da sua aplicação e conter comandos Cypress para interagir com os elementos específicos dentro desse setor.

Outros dois fatores presentes no Cypress são os comandos e asserções, que são basicamente o que faz os testes funcionarem. Os comandos são palavras que indicam à ferramenta o que ela deve fazer com certo elemento, por exemplo, existe o “cy.visit()” para visitar uma página específica ou o “cy.click()“, para clicar em um elemento específico. Já as asserções, complementam os comandos, uma vez que são declarações que verificam se uma condição é verdadeira e, se não for, geram um erro.

Indo para uma parte um pouco mais prática, abaixo está um passo a passo de como de como preparar, executar e verificar um teste no Cypress:
1. Instale o Cypress na root do seu projeto e configure o que for necessário;
2. Dentro da pasta Cypress criada, existe uma subpasta chamada “e2e”. É lá que os testes serão realizados, sempre com a extensão .cy.ts;
3. Para criar o teste, siga o pensamento comumente usado de describe, condição inicial e “it”;
4. Para executar o teste, rode o comando “ng serve” (caso esteja usando o angular);
5. Ao rodar, o Cypress irá iniciar e será solicitado que você escolha o navegador para visualizar o fluxo dos testes;
6. Depois de ser iniciado, rode o seu arquivo de testes dentro do Cypress. Ele irá mostrar passo a passo dos caminhos do seu teste, junto com a sua interface ao lado;
7. Observe o resultado do seu teste ao lado esquerdo da tela;

Pensando nisso, para realizar um bom teste no Cypress pense em todos os caminhos possíveis que um usuário pode percorrer na sua aplicação, e não só isso, mas também todos os caminhos no qual ele pode burlar funções principais da aplicação para realizar alguma vontade sua específica.
