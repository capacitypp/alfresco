FROM alfresco/alfresco-libreoffice:1.3

RUN yum install -y wget
RUN yum install -y unzip
RUN wget https://oscdl.ipa.go.jp/IPAexfont/IPAexfont00301.zip
RUN unzip IPAexfont00301.zip
RUN rm -f IPAexfont00301.zip
RUN mkdir -p /usr/share/fonts/ipa-ex-gothic/
RUN cp IPAexfont00301/*.ttf /usr/share/fonts/ipa-ex-gothic/
RUN chmod 0644 /usr/share/fonts/ipa-ex-gothic/*
RUN fc-cache -fv
