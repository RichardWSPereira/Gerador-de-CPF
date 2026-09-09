# Gerador de CPF

Aplicação web para geração de CPFs válidos para fins de estudo e testes. O projeto utiliza o código de cada estado brasileiro na composição do documento e calcula os dígitos verificadores de acordo com a regra oficial do CPF.

## Funcionalidades

- Geração de CPF com dígitos verificadores válidos.
- Seleção do estado brasileiro para definir o nono dígito.
- Exibição do CPF com ou sem pontuação.
- Interface simples, responsiva e executada diretamente no navegador.

## Tecnologias

- JavaScript (ES6+)
- Webpack
- Babel
- CSS3
- HTML5

## Como executar

### Pré-requisitos

- Node.js instalado.
- npm instalado.

### Instalação

Clone o repositório e instale as dependências:

```bash
git clone https://github.com/RichardWSPereira/Gerador-de-CPF.git
cd Gerador-de-CPF
npm install
```

### Desenvolvimento

Inicie o Webpack em modo de observação:

```bash
npm run dev
```

Depois, abra o arquivo `public/index.html` no navegador. A cada alteração nos arquivos da pasta `src`, o bundle será regenerado automaticamente.

Para gerar o bundle uma única vez:

```bash
npx webpack --mode development
```

## Estrutura do projeto

```text
src/
├── main.js                  # Interações com a interface
├── modules/
│   ├── geraCPF.js           # Geração do CPF
│   └── validaCPF.js         # Cálculo dos dígitos verificadores
└── assets/css/style.css     # Estilos da aplicação

public/
├── index.html               # Página principal
└── assets/js/bundle.js      # Arquivo gerado pelo Webpack
```

## Uso responsável

Os CPFs gerados são destinados exclusivamente a estudos, desenvolvimento e testes de software. Não utilize os dados para cadastro, fraude ou qualquer atividade que exija um documento real.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
