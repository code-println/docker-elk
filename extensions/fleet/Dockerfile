ARG ELASTIC_VERSION

FROM elastic/elastic-agent:${ELASTIC_VERSION:-9.0.2}

# Ensure the 'state' directory exists and is owned by the 'elastic-agent' user,
# otherwise mounting a named volume in that location creates a directory owned
# by root:root which the 'elastic-agent' user isn't allowed to write to.
RUN mkdir state
