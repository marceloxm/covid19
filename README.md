# 🦠 Painel de Monitoramento COVID-19 (PWA)

## 📖 Sobre o Projeto

Este projeto consiste em uma **Progressive Web Application (PWA)** desenvolvida em **React** para o acompanhamento e monitoramento de dados sobre os casos de **COVID-19** ao redor do mundo. A aplicação foi construída como parte de um desafio prático de bootcamp da **[Digital Innovation One (DIO)](https://dio.me)**.

O foco principal do projeto é demonstrar como transformar uma aplicação web tradicional em um **PWA**, permitindo que ela seja executada no navegador e também instalada em dispositivos móveis ou desktops para funcionar de forma semelhante a um aplicativo nativo (incluindo cache de recursos e suporte offline via Service Workers).

---

## ✨ Funcionalidades

- **Monitoramento Global por País:** Seleção de diferentes países (como Brasil, Estados Unidos, China, Itália, Alemanha, entre outros) para visualização de estatísticas atualizadas.
- **Indicadores Detalhados:** Exibição clara de:
  - Total de casos confirmados;
  - Óbitos registrados hoje;
  - Casos registrados hoje;
  - Total de óbitos;
  - Total de pacientes recuperados.
- **Recursos de PWA (Progressive Web App):**
  - Possibilidade de instalação na tela inicial do dispositivo;
  - Uso de Service Workers e `manifest.json` para comportamento nativo e carregamento rápido;
  - Compartilhamento rápido de informações.
- **Interface Responsiva:** Layout adaptado para diferentes tamanhos de tela, ideal tanto para smartphones quanto para desktops.

---

## 🛠️ Tecnologias Utilizadas

Com base na estrutura de arquivos do repositório (`package.json`, `yarn.lock`, `config-overrides.js` e `jsconfig.json`), o projeto utiliza:

- **[React](https://react.dev):** Biblioteca JavaScript para construção da interface de usuário baseada em componentes.
- **JavaScript (ES6+):** Linguagem principal da aplicação.
- **Material-UI / Styled Components:** Estilização e componentes visuais da interface.
- **React App Rewired (`config-overrides.js`):** Personalização das configurações do Create React App sem a necessidade de executar `eject`.
- **Service Workers & Web App Manifest:** Recursos nativos da web para funcionamento como PWA.
- **[Yarn](https://yarnpkg.com) / npm:** Gerenciamento de pacotes e dependências.

---

## 📂 Estrutura de Arquivos

```text
covid19/
├── public/               # Arquivos estáticos, ícones do PWA, index.html e manifest.json
├── src/                  # Código-fonte React (componentes, containers, serviços de API, assets e serviceWorker)
├── config-overrides.js   # Sobrescrita de configurações do build do Create React App
├── jsconfig.json         # Configurações de caminhos absolutos e inteligência do editor JS
├── package.json          # Dependências do projeto e scripts de execução
├── yarn.lock             # Árvore exata de versões das dependências instaladas via Yarn
└── README.md             # Documentação do projeto
```

---

## 🚀 Como Executar o Projeto na Sua Máquina

### Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:
- **[Node.js](https://nodejs.org)** (versão LTS recomendada)
- **[Yarn](https://yarnpkg.com)** (recomendado, pois o projeto possui `yarn.lock`) ou **npm**
- **[Git](https://git-scm.com)**

### Passo a passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com
   ```

2. **Acesse o diretório do projeto:**
   ```bash
   cd covid19
   ```

3. **Instale as dependências:**
   Utilizando o Yarn:
   ```bash
   yarn install
   ```
   *(Ou, caso prefira utilizar o npm: `npm install`)*

4. **Inicie o servidor de desenvolvimento:**
   Utilizando o Yarn:
   ```bash
   yarn start
   ```
   *(Ou com npm: `npm start`)*

5. **Acesse a aplicação no navegador:**
   O projeto será aberto automaticamente ou ficará disponível em `http://localhost:3000/`.

---

## 📦 Gerando Build de Produção (Testando o PWA)

Recursos completos de PWA (como Service Workers funcionando em modo offline e o botão de instalação no navegador) são ativados na versão de produção. Para gerar e testar o build localmente:

1. **Gere os arquivos otimizados de produção:**
   ```bash
   yarn build
   ```
   *(Ou `npm run build`)*

2. **Sirva a pasta `build` localmente:**
   ```bash
   npx serve -s build
   ```
   Acesse o endereço local exibido no terminal (geralmente `http://localhost:5000` ou `http://localhost:3000`) para testar a instalação do PWA no navegador.

---

## 🤝 Contribuição

Contribuições são sempre bem-vindas! Se você quiser melhorar este projeto:

1. Faça um **Fork** do repositório.
2. Crie uma **Branch** para sua melhoria (`git checkout -b feature/NovaFuncionalidade`).
3. Faça o **Commit** das suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Faça o **Push** para a branch (`git push origin feature/NovaFuncionalidade`).
5. Abra um **Pull Request**.

---

## 👨‍💻 Autor

Desenvolvido por **[marceloxm](https://github.com/marceloxm)** durante os estudos na **Digital Innovation One (DIO)**.
