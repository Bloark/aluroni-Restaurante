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
11. 

