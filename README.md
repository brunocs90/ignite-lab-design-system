<h1 align="center">
  <span>Design System with Storybook</span>
</h1>

<p align="center">
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-conceitos">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-instalação">Instalação</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<br>

<p align="center">
  <img alt="layout" src="./images/fluxo.PNG" width="50%">
</p>

<br>

## 💻 Projeto

Aplicação desenvolvida durante o Ignite Lab promovido pela Rocketseat O objetivo da aplicação é desenvolver um design system com tecnologias modernas de UI/UX.

## 🚀 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [Tailwindcss](https://tailwindcss.com/) - framework css que implementa classes prontas de estilização (Baixar sua extensão)

- [PostCss](https://postcss.org/) - bundler para o css, automatiza tarefas dentro do css (-p para criar seu arquivo de configuração, baixar sua extensão)
Autoprefixer - Plugin do postcss que adiciona alguns prefixos do css (mox, webkit),

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

```
- [Storybook](https://storybook.js.org/docs/react/get-started/introduction) - Biblioteca utilizada juntamente ao desenvolvimento do código para documentar os componentes, facilita a visualização dos componentes em todas as suas variações de forma documentada (vai criar uma pasta .storybook, baixar a extensão mdx, sempre que alguma informação de um arquivo.stories modificar as atualizações são feitas na documentação localhost)

```
npx sb init --builder @storybook/builder-vite --use-npm
npm run storybook

```
- [clsx](https://www.npmjs.com/package/clsx) - pacote que permite aplicar classes em componentes de maneira condicional

```
npm install --save clsx

```
- [radix-ui](https://www.radix-ui.com/) - biblioteca de componentes que fornece componentes de UI para a aplicação, utilizado para design systems (instalar o componente slot e checkbox)

```
npm install @radix-ui/react-slot @radix-ui/react-checkbox

```
- [Slot](https://www.radix-ui.com/docs/primitives/utilities/slot) - pega as propriedades de um componente e repasa para o primeiro componente que vem com o children.

- [Phosphor](https://phosphoricons.com/) - biblioteca de ícones para utilizar com react

```
npm i phosphor-react

```

## 📥 Instalação

Faça um clone desse repositório e acesse o diretório.

[Storybook deployer](https://github.com/storybookjs/storybook-deployer) - ferramenta que permite fazer deploy do storybook em serviços de hospedagem estáticos

```
npm i @storybook/storybook-deployer --save-dev

```

Adicionar o seguinte script no package.json para fazer deploy no GitHub Pages

```
"deploy-storybook": "storybook-to-ghpages"

```

Para gerar os arquivos estáticos de build

```
npm build-storybook

```

[CI/CD](https://www.redhat.com/pt-br/topics/devops/what-is-ci-cd) - metodologia baseada em worflow de integração contínua. É utilizado para que toda vez quando enviar atualizações para o repositório do github, o github pages também será atualizado com a documentação do storybook (instalar o storybook-deployer e criar arquivo deploy-docs.yml)

[a11y](https://storybook.js.org/addons/@storybook/addon-a11y) - addon do sb utilizado para tornar os componentes UI mais acessíveis (Abre uma aba de acessibilidade no storybook)

```
npm install @storybook/addon-a11y
```

[Transform tool](https://transform.tools/) - Utilizado para converter um svg em componente React


## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---
**Desenvolvido por [Bruno César](https://github.com/brunocs90).**