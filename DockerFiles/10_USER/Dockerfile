FROM almalinux:9
#CMD ["ping","google.com"]
RUN dnf install git -y
RUN useradd raghu
# raghu user will will run inside the container
USER raghu
CMD ["google.com"]
ENTRYPOINT ["ping"]