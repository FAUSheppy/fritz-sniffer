FROM alpine:3.17

RUN apk add wget curl perl bash && \
    mkdir /pcap
COPY pcap.sh /pcap.sh

#HEALTHCHECK --start-period=10s --retries=3 --timeout=5s CMD [ -f /ready ] || exit 1

ENTRYPOINT ["bash", "/pcap.sh"]
