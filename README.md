# Quasar App (memory-leak-test-v1)

A demo project to demonstrate no memory leak when using `vue-i18n` compared to [memory-leak-quasar-v2](https://github.com/Evertvdw/memory-leak-quasar-v2).

## Reproduction

1. Install the dependencies `yarn install`
2. Build the project `yarn run build`
3. Run the project `yarn run start`

The server will now run at `localhost:9000`. You can fire off 100 request in sequence by running `yarn run load`. The server will log the initial and current memory usage on every request.

## Packages used in this repo

- quasar - 2.14.6
- @quasar/app-vite - 1.7.4
- vue - 3.4.21
- vue-router - 4.3.0
- vite - 2.9.17
- @intlify/unplugin-vue-i18n - 2.0.0
- vue-i18n - 9.10.1

I ran this test myself using node version 18.17.0 on Windows 11.
