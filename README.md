# Pattern matching Next.js

This is an experiment to try to set up the babel plugin for [pattern
matching](https://github.com/babel/babel/pull/7633).

## Getting started

- First set up the fork that contains the plugin

  ```sh
  git clone https://github.com/JuanCaicedo/babel/
  cd babel
  git checkout vincent-tc39-juan
  make bootstrap
  cd packages/babel-plugin-syntax-pattern-matching/
  npm link
  cd ../babel-plugin-proposal-pattern-matching/
  npm link @babel/plugin-syntax-pattern-matching
  npm link
  cd ../..
  make watch
  ```

- Next set up this repo:

  ```sh
  git clone https://github.com/JuanCaicedo/pattern-matching-next-js
  npm link @babel/plugin-syntax-pattern-matching
  npm install
  npm run dev
  ```

- Go to <http://localhost:3000/>

## Why Next.js?

I like it 😄 But also it sets up a nice babel build for both the frontend and
backend, without having to do much work.
