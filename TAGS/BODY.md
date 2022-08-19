# BODY

Created: July 25, 2022 3:40 PM

### **Tags**

- `<script src="ijs.js"></script>`
    - normalmente usado no fim do body
    - **Src** significa "source" [fonte]

---

- `<li>`
    - Cria uma lista com Default bulletpoint

---

- Lista Ordenada e não ordenada
    - `<ol>`
        - Ordenada
    - `<ul>`
        - não ordenada

---

- Citação
    - **`<blockquote>`**
        - O Elemento HTML `<blockquote>` (ou Elemento HTML de citação de bloco) indica que o texto incluído é uma longa citação. Normalmente, este é processado visualmente pelo recuo (ver [Notas](https://developer.mozilla.org/en-US/docs/HTML/Element/blockquote#Notes) sobre como mudá-lo). A URL para a fonte da citação pode ser dada usando o atributo **cite**, enquanto uma representação de texto da fonte pode ser dada usando o `[<cite>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/cite)` elemento.
    - `<cite>`
        - O **elemento** **HTML `<cite>`** representa uma referência a um trabalho artístico. Deve incluir o título do trabalho ou uma URL de referência, que pode ser em uma forma abreviada de acordo com as convenções usadas para a adição dos metadados de citação.
    
    ```jsx
    <blockquote>
        Havia um passaro,que voava. <cite>Fabiano</cite>
    </blockquote>
    ```
    
    - `<q>`
        - O elemento HTML `<q>` indica que o texto dentro da tag é uma pequena
         citação. Este elemento destina-se a citações curtas que não requerem 
        marcações de parágrafo; para citações maiores use o elemento `[<blockquote>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/blockquote)`
        .

---

- `<abbr>`
    - abreviação
    - é usanda quando o mouse é descansado
    
    ```html
    <abbr title="Hypertext Markup Lnaguage">HTML</abbr>
    ```
    

---

- `<address>`
    
    É usada como uma `<div>`, porém ele é feita para deixar o contato do criador da página por exemplo
    

---

- `<code>`
    - Uma `<div>` para explicar que é para códigos

---

- `<pre>`
    - Mantem a formatação que foi feita no arquivo, então espaços em brancos continuarão do jeito escrito

---

- `<a>`
    - `<a href="#hungry" target=”_blank”>Redirecionamento em outra janela</a>`
    
    ---
    
    - Navegação de fragmento
        
        ```html
        <ol>
                <li><a href="#about">Sobre mim</a></li>
                <li><a href="#name">Vitoria</a></li>
                <li><a href="#hungry">Come muito</a></li>
            </ol>
            <h2 id="about">Sobre Mimm</h1>
            <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. In maiores deleniti unde minima non, nemo veritatis aliquid, suscipit ducimus alias, doloremque harum. Minima illum iste sint accusamus incidunt repudiandae repellendus.
            </p>
            <h2 id="name">Nome</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam aperiam molestiae voluptatibus quo, dolor dolore, numquam enim saepe, qui voluptatum accusamus dignissimos veniam! Obcaecati repellat hic optio consectetur dolorem error?
            </p>
            <h2 id="hungry">Fome</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam aperiam molestiae voluptatibus quo, dolor dolore, numquam enim saepe, qui voluptatum accusamus dignissimos veniam! Obcaecati repellat hic optio consectetur dolorem error?
            </p>
        ```
        
    - em href podemos utilizar ainda da seguinte maneira
        - href=”mailto:fabiano03@gmail.com”
        - href=”tel:+5511951234567”

---

- `<tittle>`
    - Ao descansar o mouse em cima da palavra ele irá escreve o que há dentro desse tag

---

- `<table>`
    - Usada para a criação de uma tabela
    - `<tr>`
        - TableRow
    - `<th>`
        - TableHead
            - Cabeçalho
    - `<td>`
        - conteúdo da linha
    - `<thead>`
        - como um `<div>`
        - usado para englobar todo o cabeçalho
        - rowspan=”2”
            - ocupa 2 linha
        - colspan=”2”
            - ocupa 2 colunas
    - `<tbody>`
        - como um `<div>`
        - usado para englobar todo o corpo
    - `<colgroup>`
        - `<col>`
            - se refere a coluna
        - span=”2”
            - diz q ela ocupa duas colunas
    - scope
        - diz a que ela pertence
    
    ---
    
    - Exemplo
        
        ```html
        <table>
            <caption>Produzidos x Vendidos por Loja</caption>
         
            <colgroup>
                <col>
                <col span="2" style="background-color: red">
                <col span="2" style="background-color: blue;">
            </colgroup>
            
            <thead>
                <tr>
                    <th rowspan="2"></th>
                    <th colspan="2" scope="colgroup">Afonso Pena</th>
                    <th colspan="2" scope="colgroup">Antônia Pereira</th>
                </tr>
                <tr>
                    <th scope="col">Produzidos</th>
                    <th scope="col">Vendidos</th>
                    <th scope="col">Produzidos</th>
                    <th scope="col">Vendidos</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <th scope="row">Vassouras</th>
                    <td>50</td>
                    <td>30</td>
                    <td>20</td>
                    <td>20</td>
                </tr>
                <tr>
                    <th scope="row">Baldes</th>
                    <td>10</td>
                    <td>10</td>
                    <td>30</td>
                    <td>25</td>
                </tr>
            </tbody>
        </table>
        ```
        

---

- `<em>`
    - deixa em italianico

---

- `<form>`
    - Formulário
    - <form> comumente tem dois atributos
        - não é possível fazer um <form> dentro de outro <form>
        - action=”value”
            - recebe os valores do formulário para tal endereço
            - caso vazio ele retorna o valor para a mesma página
        - method=”value”
            - atribui o método que deve ser usado
            - caso em branco ele usará o método GET
    - Sintaxe:
        
        ```html
        <form action="value" method="value">
        	[...]
        </form>
        <!-- ou -->
        <form>
        	[...]
        </form>
        ```
        

---

- `<fieldset>`
    - Não precisa estar dentro do formulário
    - Agrupamento de campos
    - Semântico
    - Mais acessibilidade
    - Sintaxe:
        
        ```html
        <form>
        	<fieldset> <!-- é possível adicionar a propriedade *disable*-->
        		[...]
        	</fieldset>
        </form>
        <!-- ou -->
        <form id="identificado">
        </form>
        	<fieldset form="identificado">
        		[...]
        	</fieldset>
        ```
        
    
    ---
    
    - Exemplo
        
        ```html
        <form id="contato">
        </form>
        <fieldset form="contato" name="input-contato">
            <legend>Contato</legend>
        
            <label for="">Nome</label>
            <input type="text">
        </fieldset>
        ```
        

---

- `<label>`
    - Acessibilidade
    - Associa e identifica um ou mais tags de ENTRADA DE DADOS como <input>
    - Ao clicar, ele leva direto para a entrada de dados
    - Caso as tags de entrada de dados estejam fora, é possível associa-las com o for=”identificador” via id=”identificador”
        - é bom citar que o for=”value” não serve para todas as tags
        - Exemplo:
            
            ```html
            <label for="identificador">
            	Nome:
            </label>
            <input id="identificador">
            ```
            

---

- `<button>`
    
    <aside>
    💡 [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/button#attr-type](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/button#attr-type)
    
    </aside>
    
    - Ele já tem uma estilização própria do navegador
    - Atributos
        - autofocus
            - Esse atributo booleano permite-o especificar que o botão possuirá o foco de entrada assim que a página carrega, a menos que o usuário sobrecreva esse comportamento digitanto um controle diferente. Apenas um elemento de um documento associado a um formulário pode ter esse atributo específico.
        - button
            - O botão não possui comportamento padrão. Ele pode ter scripts do lado do cliente associado com os eventos do elemento, no qual são acionados quando o evento ocorrer.
        - disable
            - Esse atributo booleano indica que o usuário não poderá interagir com o botão. Se esse atributo não for especificado, o botão herdará a configuração do elemento que o contém,  por exemplo `[<fieldset>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/fieldset)`, se não existir nenhum elemento com o atributo **disabled** definido, então o botão estará habilitado.
            - Firefox irá, diferente de outros navegadores, por padrão, [persiste com o estado dinâmico desativado](https://stackoverflow.com/questions/5985839/bug-with-firefox-disabled-attribute-of-input-not-resetting-when-refreshing) de um `[<button>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/button)` sob as páginas carregadas. Use o atributo `[autocomplete](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/button#attr-autocomplete)` para controlar esse recurso.
        - reset
            - O botão restaura todos os controles para seus valores iniciais.
        - submit
            - O botão envia os dados do formulário para o servidor. Esse é o padrão se o atributo não for especifidado, ou se o atributo é dinamicamente mudado para um valor vazio ou inválido.

---

- `<datalist>`
    
    <aside>
    💡 [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/datalist](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/datalist)
    
    </aside>
    

---

- `<article>`
    - **Representa uma composição independente** em um documento, página, aplicação, ou site, ou que é **destinado a ser distribuido de forma independente ou reutilizável.**
    - Por exemplo, em sindicação. Este poderia ser o post de um fórum, um artigo de revista ou jornal, um post de um blog, um comentário enviado por um usuário, um gadget ou widget interativos, ou qualquer outra forma de conteúdo independente.
    - Um grande conjunto onde normalmente se encontra um único ou um conjunto de texto
    - Exemplo
        
        ```jsx
        <body>
            <main>
                <h1>Receitas</h1>
                <p>Essa é uma página de receitas</p>
        
                <article>
                    <h2>Receita de torta de maçã</h2>
                    <p>Essa é uma receita de torta de maçã</p>
                </article>
                <article>
                    <h2>Receita de torta de limão</h2>
                    <p>Essa é uma receita de torta de maçã</p>
                </article>
            </main>
        </body>
        ```
        

---

- `<section>`
    - **Representa uma seção genérica** contida em um documento HTML, **geralmente com um título**, quando não existir um elemento semântico mais específico para representá-lo.
        - é comum sempre ter um título.
    - Por exemplo, um menu de navegação deve estar dentro um elemento `[<nav>](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/nav)`
        - mas uma lista de resultados de pesquisa ou a exibição de um mapa e seus controles não possuem elementos específicos, e podem ser colocados dentro de uma <section>.

---

- `<input>`
    
    <aside>
    💡 [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)
    
    </aside>
    
    - Ele aceita deis de textos a arquivos
    - type=”value”
        
        <aside>
        💡 [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Input#attr-type](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Input#attr-type)
        
        </aside>
        
    - placeholder=”value”
        - "Sugestão”
        - escreve por trás da input, como uma sugestão de formulário
        - Exemplo
            
            ```html
            <input placeholder="Digite algo">
            ```
            
    - minlenght=”value”
        - mínimo de caracteres
        - Sintaxe
            
            ```css
            <input minlenght="4">
            ```
            
    - maxlenght=”value”
        - máximo de caracteres
        - Sintaxe
            
            ```css
            <input maxlenght="8">
            ```
            
    - size=”value”
        - tamanho do input
        - Sintaxe
            
            ```css
            <input size="8">
            ```
            
    - pattern=”value”
        - Padroniza o input
        - Sintaxe
            
            ```html
            <input type="password" pattern="[number-numbercharacter-character]{minlenght,maxlenght}">
            ```
            
            - Exemplo
                
                ```html
                <input type="password" pattern="[0-9a-fA-F]{4,8}">
                ```
                
    - autocomplete=”value”
        
        <aside>
        💡 [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Input#attr-autocomplete](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Input#attr-autocomplete)
        
        </aside>
        
    - required
        - Trata esse campo como obrigatório
    
    ---
    
    - Exemplo final
        
        ```html
        <form action="">
                <fieldset>
                    <legend>Contato</legend>
                    <label for="name">Nome</label>
                    <br>
                    <input id="name" type="text" name="name">
                    <br>
        
                    <label for="email">email</label>
                    <br>
                    <input type="email" name="email" id="email">
                    <br>
        
                    <label for="menssage">message</label>
                    <br>
                    <textarea name="menssage" id="menssage" cols="20" rows="10"></textarea>
                    <br>
        
                    <button type="submit">Enviar</button>
                </fieldset>
            </form>
        ```
        

### **Seções comuns / Tags semântica**

- Cabeçalho `<header>`
    - block
    - O cabeçalho do nosso site, o local onde geralmente fica a logo e o menu.

---

- Navegação `<nav>`
    - A navegação do site vai oferecer links para seções do site, o nosso menu.
        - Normalmente usada pala links importantes
    - Costuma ficar dentro da header, porém pode ficar em outros lugares, como em uma parte lateral, ou na parte de baixo.

---

- Conteúdo principal `<main>`
    - A parte do site aonde vai o conteúdo principal, no caso de um blog, teremos vários artigos, vários posts.
    - Deve-se utilizar apenas um `<main>` por vez

---

- Conteúdo relacionado `<aside>`
    - O conteúdo relacionado é algo que seja relacionado levemente ao nosso conteúdo principal, porém não tanto para ficar lá.
    - Normalmente é usada como barra lateral.
    - representa uma seção de uma página que consiste de conteúdo que é tangencialmente relacionado ao conteúdo do seu entorno, que poderia ser considerado separado do conteúdo. Essas seções são, muitas vezes, representadas como barras laterais. Elas muitas vezes contem explicações laterais, como a definição de um glossário; conteúdo vagamente relacionado, **como avisos**; a biografia do autor; ou, em aplicações web, informações de perfil ou links de blogs relacionados.

---

- Rodapé `<footer>`
    - Onde ficam as informações da parte de baixo da página.
        - Informações do autor
        - copyright
        - contato
        - sitemap

---

- Exemplo de um `<body>` bem feito
    
    ```jsx
    <body>
        <header>
            logomarca
    
            <nav>
                <ul>
                    <li>item</li>
                </ul>
            </nav>
        </header>
    
        <main>
            conteúdo principal
        </main>
    
        <aside>
            parte lateral
        </aside>
    
        <footer>rodapé</footer>
    </body>
    ```