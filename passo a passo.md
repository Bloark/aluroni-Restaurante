# Passo á Passo

1. npx create-react-app aluroni --template typescript --use-npm
2. cd aluroni
3. npm run start
4. Criação da pasta pages dentro de src e Cardapio dentro de Pages
5. Instalçao do npm i typescript-plugin-css-modules sass
6. Criação do arquivo \src\pages\Cardapio
7. importação de logo.svg

```js
import styles from './Cardapio.module.scss'
import logo from '../../assets/logo.svg'

export default function Cardapio() {
    return (
        <main>
            <nav className={styles.menu}>
                <img src={logo} alt="logo do aluroni" />
            </nav>
        </main>
    )
}
```

8. npm run build
9. npm run start
10. Covertendo um componente para ReactComponente e utilizado no projeto.

```js
import styles from './Cardapio.module.scss'
import {ReactComponent as Logo } from '../../assets/logo.svg'

export default function Cardapio() {
    return (
        <main>
            <nav className={styles.menu}>
                <Logo />
            </nav>
        </main>
    )
}
```

11. configrando caminho absoluto no tsconfig.json como "baseUrl": "src"
12. Alterando caminhos de from '../../assets/logo.svg' para from 'assets/logo.svg'
13. aplicando reset.css no \srcs index.css
14. Adicionando fontes no index.css

```js
@import url('https://fonts.googleapis.com/css2?family=Italiana&display=swap');
* {
  box-sizing: border-box;
  font-family: 'Italiana', serif;
  }
```

15. Importando o Nomarlize @import-normalize; no src/index.css para reset do css
16. instalando o npm install normalize.css
17. importando o normalize no index.tsx

```js
    import React from 'react';
    import ReactDOM from 'react-dom/client';
    import "normalize.css"
    import './index.css';
    import Cardapio from './pages/Cardapio';

    const root = ReactDOM.createRoot(
    document.getElementById('root') as HTMLElement
    );
    root.render(
    <React.StrictMode>
    <Cardapio />
    </React.StrictMode>
    );
```

18. Criando o Header.
19. Criando o buscador.
20. importando e aplicado arquivos pronto de css.
21. importando pacotes de icons npm install react-icons
22. Criando filtros
23. implementando os filtros e seus funcionamnetos.
24. instalação do pacote className npm install classnames
25. Criando o ordenador
26. Craindo os itens
27. Populando cada item.
28. Atualizando itens por tipo.
29. implementando método de ordenar.
