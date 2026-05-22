#Arg instruaction can be used to provide values to Dockerfile only at build time
FROM almalinux:8
ARG username
RUN adduser $username
USER $username
CMD [ "sleep", "100" ]

# docker build -buildarg username=prakash -t arg:v1 .