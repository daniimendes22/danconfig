<br/>
<p align="center">
  <h3 align="center">Dan ESLint Config</h3>

  <p align="center">
    ESLint config with typescript support
    <br/>
    <br/>
    <a href="https://github.com/daniimendes22/danconfig/issues">Report Bug</a>
    .
    <a href="https://github.com/daniimendes22/danconfig/issues">Request Feature</a>
  </p>
</p>

![Downloads](https://img.shields.io/github/downloads/daniimendes22/danconfig/total) ![Contributors](https://img.shields.io/github/contributors/daniimendes22/danconfig?color=dark-green) ![Stargazers](https://img.shields.io/github/stars/daniimendes22/danconfig?style=social) ![Issues](https://img.shields.io/github/issues/daniimendes22/danconfig) ![License](https://img.shields.io/github/license/daniimendes22/danconfig)

## Table Of Contents

- [About the Project](#about-the-project)
- [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Authors](#authors)

## About The Project

This project was created with the objective of having a config template for my projects

## Built With

This project was inspired AirBnB config, and it was build with eslint, prettier, husky, typescript and airbnb-config

## Getting Started

### Prerequisites

- yarn

### Installation

```sh
yarn add -D @dan28/danconfig typescript eslint prettier
```

## Usage

1. In the file `tsconfig.json`

```JSON
{
  "extends": "@dan28/danconfig",
  "compilerOptions": {
    "outDir": "./build",
    "rootDir": "./src"
  },
  "include": ["./src"]
}
```

2. In the file `.eslintrc`

```JSON
{
  "extends": "./node_modules/@dan28/danconfig/.eslintrc"
}
```

If you're using React:

```JSON
{
  "extends": [
    "./node_modules/@dan28/danconfig/.eslintrc",
    "./node_modules/@dan28/danconfig/.eslintrc.react"
  ]
}
```

3. In the file `.prettierrc`

```JSON
"@dan28/danconfig/.prettierrc"

```

4. In the file `.package.json`

```JSON
{
  "scripts": {
    "build": "tsc",
    "lint": "eslint ./src/",
    "format": "prettier . --write",
    "format:check": "prettier . --check"
  }
}

```

## Roadmap

See the [open issues](https://github.com/daniimendes22/danconfig/issues) for a list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

- If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/daniimendes22/danconfig/issues/new) to discuss it, or directly create a pull request after you edit the _README.md_ file with necessary changes.
- Please make sure you check your spelling and grammar.
- Create individual PR for each suggestion.
- Please also read through the [Code Of Conduct](https://github.com/daniimendes22/danconfig/blob/main/CODE_OF_CONDUCT.md) before posting your first idea as well.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See [LICENSE](https://github.com/daniimendes22/danconfig/blob/main/LICENSE.md) for more information.

## Authors

- [Daniel Mendes](https://github.com/daniimendes22)
