# Shiny + Auth0

Demonstration of using Auth0 integration in Shiny ✨ 

## Background

In this simple example, we use [Auth0](https://auth0.com) to authenticate and authorize users in a Shiny application. To make use of the Auth0 API, we're using the [auth0](https://github.com/curso-r/auth0) package. 

## Steps

To sucessfully integrate Auth0 into your Shiny application, you'll need to do the following:

1. Create an Auth0 account, tenant, and application
2. Configure your Auth0 application: configure callback URLs, allowed logout URLs, and allowed web origins. Optionally configure look and feel of the login page, by adding your own logo, fonts, and colors.
3. Add your first user to your Auth0 application.
4. Configure your Shiny application: add the `auth0` package, create a config file with `auth0::use_auth0()` and replace `shinyApp()` with `auth0::shinyAppAuth0()`.
5. Add the necessary environment variables to your Shiny application: `AUTH0_USER`, `AUTH0_KEY`, and `AUTH0_SECRET`.
6. Restart your R session 😉
7. Set your Shiny port to the port that you allowed in the callback URLs in the Auth0 dashboard (in this example, it is `8080`), you can do that with `options(shiny.port = 8080)`.
8. You get redirected to the Auth0 login page, where you can login with your user credentials.

## Watch this demonstration on YouTube

Coming soon! 👀 
