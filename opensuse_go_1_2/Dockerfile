FROM nimbostrati/updated_13_1
MAINTAINER Stephen Moore, stephen.moore@linux.com

RUN zypper --non-interactive update
RUN zypper --non-interactive addrepo --no-gpgcheck http://download.opensuse.org/repositories/devel:/languages:/go/openSUSE_13.1/ languages:go
RUN zypper --non-interactive install go

ADD golang/ /home/golang/

ENV GOPATH /home/golang/
ENV PATH $PATH:$GOROOT/bin:$GOPATH/bin

ENTRYPOINT ["go"]

CMD ["version"]
