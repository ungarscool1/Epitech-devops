FROM jenkins/jenkins:lts
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
ENV CASC_JENKINS_CONFIG /var/jenkins_home/my_marvin.yml
ENV USER_CHOCOLATEEN_PASSWORD chocolateen
ENV USER_I_DONT_KNOW_PASSWORD idk
ENV USER_NASSO_PASSWORD nasso
ENV USER_VAUGIE_G_PASSWORD vaugieg
COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
COPY my_marvin.yml /var/jenkins_home/my_marvin.yml
COPY job_dsl.groovy /var/jenkins_home/job_dsl.groovy