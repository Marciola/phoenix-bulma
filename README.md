# Phoenix-Bulma: Phoenix v1.4 and Bulma CSS

## How to use this repo:

1. Run `git clone https://github.com/Marciola/phoenix-bulma.git`

2. Run `mix deps.get` inside of the phoenix-bulma/ root

3. Run `npm install` inside of assets/ (`cd assets && npm install`)

4. Run `mix phx.server`

## How to set up Bulma in your own Phoenix v1.4 project (using webpack):

1. Install Phoenix v.1.4+ using `mix phx.new YourAppHere`

2. Download Bulma locally

3. Copy `bulma.sass` and the sass folder into `assets/css/`

4. Add `node-sass` and `sass-loader` to `assets/package.json` under "devDependencies"

5. Add `sass-loader` to css file section of `assets/webpack.config.js` and change file extension to `.scss`

6. Change import of `app.css` to `app.scss` in `assets/js/app.js`

7. Rename `app.css` to `app.scss` in `assets/css/`

8. Add `@import "./bulma.sass";` to `assets/css/app.scss`

9. Run `npm install` inside of `assets/`

Bulma should now be installed and ready to be used. 

## Errors:

If you are getting the "failed to connect" Postgrex.Error run `mix ecto.setup`

## Resources

  * Phoenix website: http://www.phoenixframework.org/
  * Bulma website: https://bulma.io/
  * Adding sass/scss to Phoenix's webpack: https://elixirforum.com/t/phoenix-1-4-webpack-4-and-bulma-bootstrap-4-sass/14354/7
