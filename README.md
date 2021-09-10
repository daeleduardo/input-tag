 ## Tag Input

 :us: 
 This is a simple Tag Input component, written on Vanilla JS, where you can use any custom Style or CSS framework, setting attributes and classes.


 :brazil:

Componente simples de Tag Input escrito em Javascript puro, onde pode-se inserir as classes e propriedades que desejar para fazer a customização de estilo.

#### How works (Como funciona):

 :us: 
Added a listener in a input text and/or button where when fire the event, get the value of input tag and create a custom badge (a div with added text and close button).

 :brazil:

 Adiciona um listener em um campo de input e/ou botão que quando disparado, coleta o valor do tag input e cria um badge customizado (uma DIV com o texto digitado e um botão de fechar).

#### Install (Como instalar):

 :us: 
Download/clone `inputTag.js` file and import on your project.

 :brazil:

 Baixar/clonar o arquivo `inputTag.js` e adiciona-lo em seu projeto.

 #### How to use (Como usar):

 :us: 
Starting the component:

`javascript

		inputTag(
			{
				inputTagId: '', # Required, the ID of input tag where text are tipped.
				badgesId:  '', # Required, the ID of div where the tags will be insert.
				btnTagId: '', # Optional, the ID of button to add the tags.
				callbackOnError: () => {}, # Optional, to trigger when a non suportted text tag are tipped.
				label: {
					classes: [], # Optional, array of classes to be applied on tag.
                    attributes: [{ name: '', value: '' }] # Optional, array of objects with attributes to be applied on tag.
				},
				btnClose: {
					classes: [], # Optional, array of classes to be applied on close button inside the tag.
					attributes: [{ name: '' value: '' }], # Optional, array of objects with attributes to be applied on close button inside the tag.
                    textContent: '' # Optional, string to put in textContent property on close button inside the tag.
				}
			}
		);
`

 :brazil:

Inicializando o componente.

`javascript

		inputTag(
			{
				inputTagId: '', # Obrigatório, ID do elemento input onde o texto será inserido.
				badgesId:  '', # Obrigatório, ID da Div onde as tags serão inseridas.
				btnTagId: '', # Opcional, ID do botão para adicionar as tags.
				callbackOnError: () => {}, # Opcional, função a ser executada quando os dados inseridos forem incorretos.
				label: {
					classes: [], # Opcional, array de classes a serem inseridas na Tag.
                    attributes: [{ name: '', value: '' }] # Opcional, array de objetos com os atributos para serem aplicados na tag.
				},
				btnClose: {
					classes: [], # Opcional, array de classes a serem inseridas no botão fechar.
					attributes: [{ name: '', value: '' }], # Opcional, array de objetos com os atributos para serem aplicados no botão fechar.
                    textContent: '' # Opcional, string para ser inserida na propriedade textContent do botão fechar.
				}
			}
		);
` 

  #### Notes (Observações):
  
   :us:
    *   The Id of badges tag is the text, only words *[a-Z]* are allowed.
    *   If has no one item, (no classes, attributes, textContent) in btnClose a textContent with "X" will be added.

    Any doubts, let me know, opening an issue.
    
   :brazil:

    *   Os Id's das tags são os textos digitados, por isso somente letras *[a-Z]* são permitidas.
    *   Se no botão de fechar, não tiver nenhum item informado (nenhuma classe, atributo ou textContent) um textContent com um "X" será adicionado.

    Qualquer dúvida, me avise, abrindo uma issue.