FROM alpine
RUN ["apk", "upgrade", "--no-cache"]
RUN ["apk", "add", "--no-cache", "build-base python3 python3-dev bash git vim"]
RUN ["pip3", "install", "--no-cache-dir", "--upgrade pip"]
RUN ["rm", "-rf /var/cache/*"]
RUN ["rm", "-rf /root/.cache/*"]

RUN cd /usr/bin \
  # && ln -sf easy_install-3.5 easy_install \
  && ln -sf python3 python \
  && ln -sf pip3 pip
