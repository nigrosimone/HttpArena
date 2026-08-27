# Stock nginx. gateway-64 is h2 over TCP only, so nothing here needs a module
# the official image does not ship - TLS, ALPN, http2 and gzip_static are all
# in it. The QUIC half of the gateway family runs on Caddy, in proxy-h3/.
FROM nginx:1.27-alpine

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 8443

CMD ["nginx", "-g", "daemon off;"]
