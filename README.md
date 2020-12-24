# Traefik X-Forwarded-For, X-Real-Ip OverWriter Plugin

If Traefik is behind a cloudflare proxy, it won't be able to get the Real IP from the external client by checking
the remote IP address. 

This plugin solves this issue by overwriting the `X-Forwarded-For` and `X-Real-Ip` with an IP from the `Cf-Connecting-Ip` header.
