# Framework Frontend Responsivo Acessivel

Framework JavaScript para criação de páginas web responsivas com acessibilidade para deficientes visuais.

## Como usar? 

Para utilizar o framework siga os seguintes passos: 

1. Baixe os arquivos deste repositório em uma pasta de sua preferência. 
2. Crie uma página HTML. 
3. Importe os arquivos **framework.js** e **framework.css** dentro da tag ```<head>``` da página criada no passo anterior.
4. Crie um arquivo JavaScript separado e também o importe na tag ```<head>```, após o arquivo **framework.js**, para que seja possível ter acesso às variáveis e funções auxiliares.
5. Dentro do arquivo JavaScript criado anteriormente, implemente uma das seguintes funções:
   * **```didStartSetup```**: essa função será chamada pelo framework assim que a página terminar de carregar, e antes das tags começarem a ser criadas a partir dos objetos recebidos. Não recebe nenhum parâmetro e não possui retorno. Use-a para executar qualquer ação que desejar nesse momoento. **Implementação opcional**.
   * **```getHeaderObjects```**: essa função deve retornar os objetos que serão transformados nas tags HTML que vc quer que sejam inseridas na tag [\<header\>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/header), dentro do body da sua página. Não recebe nenhum parâmetro e deve retornar uma lista de objetos. Caso a função não tenha sido implementada ou retorno uma lista vazia, a tag ```<header>``` não é criada. 
   * **```getMainObjects```**: essa função deve retornar os objetos que serão transformados nas tags HTML que vc quer que sejam inseridas na tag [\<main\>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/main), dentro do body da sua página. Não recebe nenhum parâmetro e deve retornar uma lista de objetos. Caso a função não tenha sido implementada ou retorno uma lista vazia, a tag ```<main>``` não é criada. 
   * **```getFooterObjects```**: essa função deve retornar os objetos que serão transformados nas tags HTML que vc quer que sejam inseridas na tag [\<footer\>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/footer), dentro do body da sua página. Não recebe nenhum parâmetro e deve retornar uma lista de objetos. Caso a função não tenha sido implementada ou retorno uma lista vazia, a tag ```<footer>``` não é criada. 
   * **```didEndSetup```**: essa função será chamada pelo framework assim que terminar de processar os objetos que foram retornados nas três funções anteriores. Não recebe nenhum parâmetro e não possui retorno. Use-a para executar qualquer ação que desejar nesse momoento. **Implementação opcional**.
   
Este projeto possui um arquivo de **template**, no qual todos os passos acima já estão implementados, e partir do qual é possível criar as páginas desejadas.
    
## Como criar os objetos que serão transformados nas tags? 

Cada tag 
