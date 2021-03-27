FROM      centos
RUN       yum install openssh-server passwd shadow-utils java-11-openjdk -y &&\
          mkdir -p /root/workspace &&\
          echo docker | passwd --stdin root &&\
          ssh-keygen -A
CMD       /usr/sbin/sshd -D
