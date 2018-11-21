# Phoenix-Bulma: Phoenix v1.4 and Bulma CSS

## How to use this repo:

1. Run `git clone https://github.com/Marciola/phoenix-bulma.git`

2. Run `mix deps.get` inside of the phoenix-bulma/ root

3. Run `npm install` inside of assets/ (`cd assets && npm install`)

4. Run `mix phx.server`

## How to set up Bulma in your own Phoenix v1.4 project (using webpack):

1. Install Phoenix v.1.4+ using `mix phx.new YourAppHere` | [commit](https://github.com/Marciola/phoenix-bulma/commit/b426bddc7f93842487113417231c8619623f1098)

2. Download Bulma locally

3. Copy `bulma.sass` and the sass folder into `assets/css/` | [commit](https://github.com/Marciola/phoenix-bulma/commit/89e07a8481866e016d1dc2c1245c9fe6df1789ed)

4. Add `node-sass` and `sass-loader` to `assets/package.json` under "devDependencies" | [commit](https://github.com/Marciola/phoenix-bulma/commit/8820554cc7f36ef59756d04d036854b2350be191)

5. Add `sass-loader` to css file section of `assets/webpack.config.js` and change file extension to `.scss` | [commit](https://github.com/Marciola/phoenix-bulma/commit/748605e0ea8974264329fe46d708fa7b880402a8)

6. Change import of `app.css` to `app.scss` in `assets/js/app.js` | [commit](https://github.com/Marciola/phoenix-bulma/commit/81840adeb2547c2e9e7c33e3498a0e1e4275290a)

7. Rename `app.css` to `app.scss` in `assets/css/` | [commit](https://github.com/Marciola/phoenix-bulma/commit/133042c1b45d55034accf757d8fed7d6cbba655a)

8. Add `@import "./bulma.sass";` to `assets/css/app.scss` | [commit](https://github.com/Marciola/phoenix-bulma/commit/c9b57b92eb34530c9d8022804edd6528f10dcd3c)

9. Run `npm install` inside of `assets/`

Bulma should now be installed and ready to be used. 

## Errors:

If you are getting the "failed to connect" Postgrex.Error run `mix ecto.setup`

## Resources

  * Phoenix website: http://www.phoenixframework.org/
  * Bulma website: https://bulma.io/
  * Adding sass/scss to Phoenix's webpack: https://elixirforum.com/t/phoenix-1-4-webpack-4-and-bulma-bootstrap-4-sass/14354/7
