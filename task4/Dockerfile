FROM nginx:1.23.3

RUN apt-get update && \
    apt-get install git -y && \
    apt-get install make && \
    curl -L https://github.com/gohugoio/hugo/releases/download/v0.111.2/hugo_extended_0.111.2_linux-amd64.deb -o hugo.deb && \
    apt install ./hugo.deb && \
    git clone https://github.com/chazapis/hy548.git && \
    cd hy548 && \
    git submodule init && \
    git submodule update && \
    make && \
    cp -R html/public/* /usr/share/nginx/html
EXPOSE 8080