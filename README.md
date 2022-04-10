# Checklist do react-redux

*Antes de começar*
- [x] pensar como será o *formato* do seu estado global
- [x] pensar quais actions serão necessárias na sua aplicação

*Instalação*
- [x] npx create-react-app my-app-redux;
- [x] npm install --save redux react-redux;
- [x] npm install.
- [x] npm install redux-thunk (opcional)

*Criar dentro do diretório src:*
- [x] diretório actions;
- [x] diretório reducers;
- [x] diretório store.

*Criar dentro do diretório actions:*
- [x] arquivo index.js.

*Criar dentro do diretório reducers:*
- [x] arquivo index.js.

*Criar dentro do diretório store:*
- [x] arquivo index.js.

*No arquivo App.js:*
- [x] definir o Provider, `<Provider store={ store }>`, para fornecer os estados à todos os componentes encapsulados em `<App />`.

*No arquivo store/index.js:*
- [x] importar o rootReducer e criar a store
- [x] configurar o [Redux DevTools](https://github.com/reduxjs/redux-devtools)
- [x] importar composeWithDevTools()(É importado da lib 'redux-devtools-extension')

*Na pasta reducers:*
- [ ] criar os reducers necessários
- [ ] configurar os exports do arquivo index.js

*Na pasta actions:*
- [ ] criar os actionTypes, por exemplo: `const ADD_TO_CART = 'ADD_TO_CART';`
- [ ] criar os actions creators necessários

*Nos componentes:*
- [ ] criar a função mapStateToProps(state) => ({}) (leitura de dados)
- [ ] criar a função mapDispatchToProps(dispatch) => ({ key: (...paramAct) => dispatch(action(...paramAct)) }) (escrita de dados)
- [ ] fazer o connect(mapStateToProps, mapDispatchToProps)(component) (importado da lib 'react-redux')
