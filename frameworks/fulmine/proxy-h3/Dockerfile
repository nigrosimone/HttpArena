# Stock Caddy, which ships h1/h2/h3 in the base image, so no custom build.
# gateway-h3 (QUIC over UDP) is what it serves; gateway-64 moved to the stock
# nginx in proxy-h2/. The Caddyfile still binds 8443 on tcp and udp both.
FROM caddy:2-alpine

COPY Caddyfile /etc/caddy/Caddyfile

EXPOSE 8443/tcp 8443/udp

CMD ["caddy", "run", "--config", "/etc/caddy/Caddyfile", "--adapter", "caddyfile"]
