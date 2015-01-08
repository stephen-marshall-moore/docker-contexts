FROM opensuse:13.2
MAINTAINER Stephen Moore, stephen.moore@linux.com

RUN zypper --non-interactive --gpgp-auto-import-keys update
RUN zypper --non-interactive --gpgp-auto-import-keys install go

ADD golang/ /home/golang/

ENV GOPATH /home/golang/
ENV PATH $PATH:$GOROOT/bin:$GOPATH/bin

ENTRYPOINT ["go"]

CMD ["version"]
