<h1 align="center">Tradeinsights Challenge</h1>

<p align="center">Desafio técnico para a vaga de Desenvolvedor FullStack na Tradeinsights</p>

## Objetivo

Criar um model chamado ativos onde teremos o código do ativo da B3 e o nome. (ativos da B3 são ações)
Cria uma controller onde podemos listar todos os ativos existentes no banco de dados
Gerar um view em vuejs / inertia / tailwind com essa lista de ativos.

## Instalação

- Pré-requisitos:
<a href="https://www.docker.com/">Docker</a>

1. Clone o projeto

```bash
git clone https://github.com/LeonardoRibas/tradeinisights-challenge.git
```
2. Inicie os containers

```bash
cd tradeinsights-challenge
./vendor/bin/sail up
```

3. Rode as migrações e seeds

```bash
php artisan migrate
php artisan db:seed
```

4. Rode o servidor

```bash
php artisan serve
```

5. Em outro terminal, instale e rode a aplicação

```bash
cd vue
npm install
npm run dev
```
