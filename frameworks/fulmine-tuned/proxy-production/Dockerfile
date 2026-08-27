# Stock nginx again, same as the gateway edge, with the production-stack
# routing and the auth subrequest.
FROM nginx:1.27-alpine

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 8443

CMD ["nginx", "-g", "daemon off;"]
