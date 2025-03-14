# Usa a imagem oficial do Nginx
FROM nginx:latest

# Remove a página padrão do Nginx
RUN rm -rf /usr/share/nginx/html/*

# Copia o site para a pasta correta do Nginx
COPY index.html /usr/share/nginx/html/index.html

# Expõe a porta 80 para acesso
EXPOSE 80

# Inicia o Nginx
CMD ["nginx", "-g", "daemon off;"]
