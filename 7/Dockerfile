ARG VERSION=7.2.2

FROM node:lts-alpine
ENV BS_PLATFORM_VERSION=$VERSION
# Adds bsb ninja build dependencies & bs-platform package
RUN apk add g++ make python && \
  npm install -g bs-platform@${BS_PLATFORM_VERSION} --unsafe-perm


FROM node:lts-alpine
ENV GLOBAL_NODE_MODULES_PATH=/usr/local/lib/node_modules

# Copies bs-platform package from builder image
COPY --from=0 ${GLOBAL_NODE_MODULES_PATH} ${GLOBAL_NODE_MODULES_PATH}

CMD ["bsb"]