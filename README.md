
# Menu Dinâmico com React (Aula 10)

## Breve descrição das alterações feitas na aula

- Implementação de um menu dinâmico usando **React** e **reactstrap**.
- Exibição de pratos em formato de cartão (Card).
- Funcionalidade para selecionar um prato e exibir seus detalhes.

## MenuComponent.js

**Breve descrição:** Este arquivo contém o componente que exibe a lista de pratos e os detalhes do prato selecionado.

### Respostas às perguntas

1. **Quais os imports utilizados? (breve explicação)**
   - `useState`: Gerencia o estado do prato selecionado.
   - Componentes do **reactstrap**:
     - `Card`, `CardImg`, `CardImgOverlay`, `CardText`, `CardBody`, `CardTitle`: Exibem os pratos e seus detalhes em um formato visual estilizado.

2. **Há componentes? O que fazem?**
   - Sim, o principal componente é o `Menu`, que:
     - Renderiza a lista de pratos.
     - Exibe os detalhes do prato selecionado.

3. **Para que serve o `onDishSelect` no projeto?**
   - Atualiza o estado `selectedDish` com o prato clicado pelo usuário.

4. **Para que serve o `renderDish`?**
   - Renderiza os detalhes do prato selecionado em um componente `Card`. Se nenhum prato estiver selecionado, retorna um elemento vazio.

5. **Para que serve o `props.dishes.map`?**
   - Itera sobre a lista de pratos (`dishes`) para renderizar um card para cada prato.

---

## dishes.js

**Breve descrição:** Este arquivo contém a lista de pratos, com todas as informações necessárias para exibi-los.

### Respostas às perguntas

1. **Quais as propriedades?**
   - `id`: Identificador único do prato.
   - `name`: Nome do prato.
   - `image`: Caminho da imagem do prato.
   - `category`: Categoria do prato (ex.: `mains`, `appetizer`).
   - `label`: Rótulo do prato (ex.: `Hot`, `New`).
   - `price`: Preço do prato.
   - `description`: Breve descrição do prato.
   - `comments`: Lista de comentários com:
     - `rating`: Nota dada ao prato.
     - `comment`: Texto do comentário.
     - `author`: Autor do comentário.
     - `date`: Data do comentário.

2. **Que tipo de date é utilizado?**
   - Datas no formato ISO, como `2012-10-16T17:57:28.556094Z`.

---

## App.js

**Breve descrição:** Este arquivo contém a estrutura principal do aplicativo e integra os componentes.

### Respostas às perguntas

1. **Para que serve o `const [dishes]`?**
   - Armazena a lista de pratos (`DISHES`) utilizando o `useState`, permitindo o gerenciamento de estado.

2. **Explicar como funciona o `<Menu dishes={dishes} />`:**
   - Passa a lista de pratos como uma propriedade (`props`) para o componente `Menu`, permitindo que este renderize os pratos dinamicamente.

---
