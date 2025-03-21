# Usa a imagem oficial do Nginx
FROM nginx:latest

# Remove a página padrão do Nginx e copia o site para a pasta correta do Nginx
COPY index.html /usr/share/nginx/html/index.html

# Expõe a porta 80 para acesso
EXPOSE 80

# Adiciona um comando HEALTHCHECK para monitorar a saúde do container
HEALTHCHECK --interval=30s --timeout=10s --retries=3 CMD curl -f http://localhost/ || exit 1

# Inicia o Nginx
CMD ["nginx", "-g", "daemon off;"]
