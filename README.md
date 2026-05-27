# Rustlings - Jornada de Aprendizado em Rust

Este repositorio reune exercicios praticos do Rustlings para apoiar o estudo progressivo da linguagem Rust. A proposta e aprender escrevendo codigo, corrigindo erros de compilacao, lendo mensagens do compilador e evoluindo gradualmente pelos principais conceitos da linguagem.

## Objetivos

- Praticar os fundamentos de Rust com exercicios pequenos e objetivos.
- Entender o ciclo de feedback do compilador e usar seus erros como guia de aprendizado.
- Desenvolver familiaridade com variaveis, funcoes, condicionais, tipos primitivos, ownership, borrowing, structs, enums, traits, lifetimes, testes, iteradores, threads, macros e conversoes.
- Criar uma base solida para escrever codigo Rust idiomatico, seguro e de facil manutencao.
- Registrar a evolucao do estudo em um repositorio organizado e reproduzivel.

## Como o Rustlings Funciona

O Rustlings e uma colecao de exercicios intencionalmente incompletos ou com erros. Cada arquivo contem instrucoes, comentarios `TODO` e testes ou verificacoes de compilacao que indicam o que precisa ser corrigido.

O fluxo principal e:

1. Abrir o proximo exercicio em `exercises/`.
2. Ler o enunciado e os comentarios do arquivo.
3. Corrigir o codigo ate que ele compile e passe nos testes.
4. Usar as mensagens do compilador como orientacao.
5. Consultar a solucao em `solutions/` somente depois de tentar resolver o exercicio.

O arquivo `.rustlings-state.txt` guarda o progresso atual do Rustlings. Ele e usado pela ferramenta para saber qual exercicio deve ser executado em seguida.

## Estrutura do Projeto

```text
.
|-- exercises/              # Exercicios a serem resolvidos
|   |-- 00_intro/           # Introducao ao fluxo do Rustlings
|   |-- 01_variables/       # Variaveis, mutabilidade e constantes
|   |-- 02_functions/       # Declaracao e uso de funcoes
|   `-- ...                 # Demais topicos da linguagem
|-- solutions/              # Solucoes oficiais desbloqueadas conforme o progresso
|-- Cargo.toml              # Configuracao dos binarios dos exercicios
|-- Cargo.lock              # Versoes travadas das dependencias
|-- rust-analyzer.toml      # Configuracao do Rust Analyzer
`-- .rustlings-state.txt    # Estado local de progresso
```

## Pre-requisitos

Antes de executar os exercicios, instale:

- Rust e Cargo via `rustup`: <https://rustup.rs>
- Rustlings via Cargo:

```bash
cargo install rustlings
```

Para confirmar a instalacao:

```bash
rustc --version
cargo --version
rustlings --version
```

## Como Executar

Na raiz do projeto, use o modo interativo do Rustlings:

```bash
rustlings
```

Comandos uteis:

```bash
rustlings watch
rustlings run functions1
rustlings hint functions1
rustlings list
```

Tambem e possivel executar exercicios diretamente pelo Cargo, pois o `Cargo.toml` registra cada exercicio como um binario:

```bash
cargo run --bin functions1
cargo test --bin functions1
```

## Fluxo Recomendado de Estudo

1. Resolva os exercicios em ordem, comecando por `00_intro`.
2. Leia o erro do compilador antes de alterar o codigo.
3. Faca mudancas pequenas e execute novamente.
4. Use `rustlings hint <nome-do-exercicio>` quando travar.
5. Consulte `solutions/` apenas para comparar abordagens ou revisar depois de resolver.
6. Faca commits pequenos por topico ou conjunto de exercicios concluidos.

## Topicos Cobertos

| Modulo | Conteudo |
| --- | --- |
| `00_intro` | Introducao ao ambiente e ao fluxo dos exercicios |
| `01_variables` | Variaveis, mutabilidade, constantes e shadowing |
| `02_functions` | Funcoes, parametros, retorno e expressoes |
| `03_if` | Controle de fluxo com `if` e expressoes condicionais |
| `04_primitive_types` | Tipos primitivos, arrays, tuplas e slices |
| `05_vecs` | Vetores e operacoes basicas com colecoes |
| `06_move_semantics` | Ownership, moves, borrowing e referencias |
| `07_structs` | Structs, instancias e metodos |
| `08_enums` | Enums, variants e pattern matching |
| `09_strings` | `String`, `&str` e manipulacao de texto |
| `10_modules` | Modulos, visibilidade e organizacao |
| `11_hashmaps` | Mapas associativos com `HashMap` |
| `12_options` | Uso de `Option` para ausencia de valor |
| `13_error_handling` | `Result`, propagacao e tratamento de erros |
| `14_generics` | Tipos genericos |
| `15_traits` | Traits, bounds e comportamento compartilhado |
| `16_lifetimes` | Lifetimes e validade de referencias |
| `17_tests` | Testes automatizados |
| `18_iterators` | Iteradores, adaptadores e consumo |
| `19_smart_pointers` | Ponteiros inteligentes |
| `20_threads` | Concorrencia com threads |
| `21_macros` | Macros em Rust |
| `22_clippy` | Lints e melhoria de qualidade com Clippy |
| `23_conversions` | Conversoes entre tipos |

## Boas Praticas

- Prefira entender a mensagem de erro antes de buscar a resposta pronta.
- Mantenha as alteracoes focadas no exercicio atual.
- Evite editar `.rustlings-state.txt` manualmente.
- Use nomes claros e codigo simples; os exercicios favorecem solucoes idiomaticas.
- Rode `cargo fmt` periodicamente para manter a formatacao consistente.
- Use `cargo clippy` quando quiser revisar sugestoes de qualidade do codigo.

## Referencias

- The Rust Programming Language: <https://doc.rust-lang.org/book/>
- Rust by Example: <https://doc.rust-lang.org/rust-by-example/>
- Rustlings: <https://github.com/rust-lang/rustlings>

## Contato Profissional

**Danilo Couto Pereira Santos**

- LinkedIn: <https://www.linkedin.com/in/danilocoutopsantos/>

## Status

Projeto em andamento para estudo e pratica de Rust. O progresso atual e controlado pelo Rustlings e pode ser acompanhado pela execucao dos comandos da ferramenta na raiz do repositorio.
