FROM alpine:3.4

RUN apk add --update nodejs tini && \
    npm install aws-es-kibana@1.0.5 -g

EXPOSE 9200

ENTRYPOINT ["/sbin/tini", "--", "aws-es-kibana", "-b", "0.0.0.0"]

# see http://label-schema.org/rc1/
LABEL org.label-schema.name="aws-es-kibana" \
      org.label-schema.version="1.0.5" \
      org.label-schema.description="aws-es-kibana" \
      org.label-schema.vendor="Claranet UK" \
      org.label-schema.schema-version="1.0" \
      org.label-schema.vcs-url="https://github.com/claranet/docker-aws-es-kibana" \
      author1="Ray Butcher<ray.butcher@claranet.uk>"
