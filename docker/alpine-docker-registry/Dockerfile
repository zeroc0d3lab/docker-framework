FROM bhuisgen/alpine-base-consul:latest
MAINTAINER "Boris HUISGEN <bhuisgen@hbis.fr>"

COPY packages/*.apk /root/
RUN apk add --update --allow-untrusted \
        /root/docker-registry-2.6.0-r0.apk && \
    rm -f /root/*.apk && \
    rm -rf /var/cache/apk/*

COPY rootfs/ /

ENTRYPOINT ["/init"]
CMD []

EXPOSE 5000
VOLUME ["/var/lib/docker-registry"]
