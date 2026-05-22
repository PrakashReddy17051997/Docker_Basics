#Arg instruaction can be used to provide values to Dockerfile only at build time. ENV variable have access inside container as well
# for best combination How can we use arg values inside the container- provide arg values to env variables so env values can be accesed in the container
FROM almalinux:8
ARG username
RUN adduser $username
USER $username
ARG Developer
ARG Project
RUN echo "Developer: ${Developer}, Project:${Project}"
ENV Developer=${Developer}
ENV Project=${Project}
CMD [ "sleep", "100" ]

# docker build  -t arg:v1 --build-arg username=prakash . 
# ARG can be use before FROM instracution before FROM, it only exeception and this arg before from cannot be accessed after from