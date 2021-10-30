FROM nginx:1.15.6

ENV TZ Asia/Tokyo
RUN echo "${TZ}" > /etc/timezone \
   && dpkg-reconfigure -f noninteractive tzdata

RUN apt-get update && apt-get install -y \
    vim \
    unzip \
    zip \
    git \
    vim