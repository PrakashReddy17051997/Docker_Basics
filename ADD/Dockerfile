FROM almalinux:8
RUN yum install nginx -y 
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://github.com/PrakashReddy17051997/300-python-Interview-questions-and-solutions/blob/main/350interview.txt /usr/share/nginx/html/index.html
CMD [ "nginx", "-g", "daemon off;" ]