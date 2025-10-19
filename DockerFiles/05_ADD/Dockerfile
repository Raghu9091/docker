FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/daws-84s/notes/refs/heads/main/session-01.txt /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
# untar and keep this is the beauty in ADD feature
ADD sample-1.tar /tmp/ 
CMD ["nginx", "-g", "daemon off;"]