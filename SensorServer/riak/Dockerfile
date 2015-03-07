# Weary Examiner Riak Instance
#
#

FROM proegssilb/riak
MAINTAINER David Bliss proegssilb@gmail.com

RUN sed -i.bak 's/search = off/search = on/' /etc/riak/riak.conf && \
    sed -i.bak 's/## strong_consistency = on/strong_consistency = on/' /etc/riak/riak.conf

EXPOSE 8098 8087

CMD ["/sbin/my_init", "--quiet"]
