FROM ubuntu:latest

MAINTAINER gabrielrcouto <gabrielrcouto@gmail.com>

EXPOSE 5901

RUN apt-get update && apt-get install -y \
    wget \
    binutils \
    gcc \
    libgtk2.0-0 \
    libgtk2.0-dev \
    psmisc \
    vnc4server \
 && rm -rf /var/lib/apt/lists/*

RUN wget http://downloads.sourceforge.net/project/lazarus/Lazarus%20Linux%20amd64%20DEB/Lazarus%201.6.4/fpc_3.0.2-170225_amd64.deb && \
    dpkg -i fpc_3.0.2-170225_amd64.deb && \
    rm fpc_3.0.2-170225_amd64.deb

RUN wget http://downloads.sourceforge.net/project/lazarus/Lazarus%20Linux%20amd64%20DEB/Lazarus%201.6.4/fpc-src_3.0.2-170225_amd64.deb && \
    dpkg -i fpc-src_3.0.2-170225_amd64.deb && \
    rm fpc-src_3.0.2-170225_amd64.deb

RUN wget http://downloads.sourceforge.net/project/lazarus/Lazarus%20Linux%20amd64%20DEB/Lazarus%201.6.4/lazarus-project_1.6.4-0_amd64.deb && \
    dpkg -i lazarus-project_1.6.4-0_amd64.deb && \
    rm lazarus-project_1.6.4-0_amd64.deb
