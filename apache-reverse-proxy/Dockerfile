# Dockerfile
FROM httpd:2.4

# Copy only your proxy rules; do NOT overwrite the built-in httpd.conf!
COPY proxy.conf /usr/local/apache2/conf/extra/proxy.conf

# Instruct httpd.conf to include your extra file
RUN echo "Include conf/extra/proxy.conf" \
    >> /usr/local/apache2/conf/httpd.conf
