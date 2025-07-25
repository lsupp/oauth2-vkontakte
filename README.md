# Vkontakte OAuth2 client provider
This package provides [Vk.com](https://vk.com/) integration for OAuth2 Client by the League.
## Installation
```
composer require lsupp/oauth2-vkontakte
```
## Add to config/packages/knpu_oauth2_client.yaml
```
  vkontakte_main:
      type: generic
      provider_class: Lsupp\OAuth2\Client\Provider\Vkontakte
      # add and set these environment variables in your .env files
      client_id: '%env(OAUTH_VKONTAKTE_CLIENT_ID)%'
      client_secret: '%env(OAUTH_VKONTAKTE_CLIENT_SECRET)%'
      # a route name you'll create
      redirect_route: connect_vkontakte_check
      redirect_params: {}
      # whether to check OAuth2 "state": defaults to true
      # use_state: true
```
