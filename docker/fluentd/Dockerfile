FROM fluent/fluentd:v1.7-debian-1

# Use root account to use apk
USER root

# below RUN includes plugin as examples elasticsearch is not required
# you may customize including plugins as you wish
# RUN apt-get install -y vi 
# make gcc g++ libc-dev
COPY fluent.conf /fluentd/etc/
COPY entrypoint.sh /bin/

USER fluent
