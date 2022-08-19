# HEAD

Created: July 25, 2022 3:39 PM

- `<meta>`
    - [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta)
    - O elemento **HTML `<meta>`** define qualquer informação de metadados que não podem ser definidos por outros elementos **HTML**
    - `<meta charset=”UTF-8”>`
        - Seta os caracteres
            - Aconselhável usar o UTF-8 (representa qualquer caractere universal)
    
    ---
    
    - `<meta name=”viewport” content=”width=device-width, initial-scale=1.0”>`
        - name=”viewport”
            - o viewport é usado para a parte visual da web página
        
        ---
        
        - width=device-width
            - iguala a largura do layout à largura do dispositivo
        
        ---
        
        - initial-scale=1.0
            - zoom inicial da páina
    
    ---
    
    - `content`
        - [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-content](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-content)
        - Esse atributo fornece o valor associado ao atributo `[http-equiv](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-http-equiv)` ou `[name](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-name)`, dependendo do contexto.
    - `http-equiv`
        - [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-http-equiv](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-http-equiv)
        - Este enumerado atributo define a pragma isso pode alterar o 
        comportamento de servers e user-agents. o valor do pragma é definido 
        usando `[content](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-content)` e pode ser um dos seguintes:
    - `name`
        - É bem importante utiliza-ló para o SEO do google
            - SEO == SEARCH ENGINE OPTIMIZATION
        - Dando bastante destaque para os elementos
            - `author`
                - definindo, em formato livre, o nome do author do documento
            - `description`
                - contém uma curta e precisa descrição do conteúdo da página. vários browsers, como o Firefox e o Opera, usam este meta como descrição padrão da página quando é marcada.
            - `robots`
                
                <meta name="robots" content="index, follow">
                
                - Diz o que o robo da google deve fazer
        - [https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-name](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-name)
        - Este atributo define o nome do document-level metadata. Isso não deve ser marcado se um dos atributos `[itemprop](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-itemprop)`, `[http-equiv](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-http-equiv)` ou `[charset](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-charset)` já estiver preparado.
         este document-level metadata name é associado a um valor, contido pelo atributo `[content](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-content)`. os possíveis valores para o elemento name são, com seu valor associado, guardado via `[content](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta#attr-content)`

---

- `<link>`
    - `<link rel="stylesheet" text="text/css" href="style.css">`
        - **rel** vem de relationship serve para você dizer qual o relacionamento do arquivo que você quer utilizar com o arquivo atual
            - Quando você coloca **rel**="**stylesheet**" , você está dizendo que o arquivo importado é o arquivo responsável pelo estilo da sua página
            - style == estilo
            - sheet == folha
            - stylesheet == folha de estilo
        
        ---
        
        - text diz que é um texto do tipo css
            - href vai linkar para um diretório
    - `<link rel="icon" href="diretorio">`
        - FavoriteIcon