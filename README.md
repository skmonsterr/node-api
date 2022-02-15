# API Node.js Typescript SOLID + TDD

- @swc/core
- @swc/jest
- @types/jest
- jest
- ts-node
- typescript

> Usando Jest + Typescript ES2017 (ES6)

<pre>
  <code>
  transform: {
    "^.+\\.(t|j)sx?$": [
      "@swc/jest",
      {
        jsc: {
          parser: {
            syntax: "typescript",
            tsx: false,
            decorators: true,
          },
          target: "es2017",
          keepClassNames: true,
          transform: {
            legacyDecorator: true,
            decoratorMetadata: true,
          },
        },
        module: {
          type: "es6",
          noInterop: false,
        },
      },
    ],
  },
  </code>
</pre>

## Modelo de arquitetura aplicação Node com Typescript

> Aplicação que recebe desafios (Challenges) Faz a correção desse desafio e retorna um resultado.

- Domains Experts
- Use cases
- Repositories
- Tests (Jest)
- In Memory Repositories
