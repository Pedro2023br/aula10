# Configuração react com reactstrap



## Configuração do Bootstrap no projeto

No arquivo `src/index.js`, foi adicionada a seguinte linha para aplicar os estilos globais do Bootstrap:

```javascript
import 'bootstrap/dist/css/bootstrap.min.css';
```

Isso garante que todos os componentes do Reactstrap sigam o estilo visual do Bootstrap.

---

## Adicionando uma Barra de Navegação

No arquivo `src/App.js`, adicionamos o seguinte código:

```javascript
import React from 'react';
import { Navbar, NavbarBrand } from 'reactstrap';

function App() {
  return (
    <div className="App">
      <Navbar dark color="primary">
        <div className="container">
          <NavbarBrand href="/">Ristorante Con Fusion</NavbarBrand>
          <div>Aluno: Pedro</div>
        </div>
      </Navbar>
    </div>
  );
}

export default App;
```

### Explicação do Código:
- **Navbar**: Cria uma barra de navegação estilizada com Bootstrap.
  - Propriedade `dark`: Aplica cores escuras ao texto.
  - Propriedade `color="primary"`: Define o fundo com a cor principal do Bootstrap (azul).
- **NavbarBrand**: Mostra o nome ou logo da aplicação e o link para a página inicial.
- **div**: Incluímos o nome do aluno para personalização.

---

## Atualização do README.md

O arquivo README foi atualizado com:
1. **Resumo dos passos realizados**.
2. **Imagem do resultado**.



---

## Resultado Final

Após seguir os passos, sua barra de navegação deve ficar assim:

![Navbar com nome](![Navbar com nome](<src/Captura de tela 2024-11-21 203713.png>))


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
