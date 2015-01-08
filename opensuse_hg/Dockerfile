FROM opensuse:13.2
MAINTAINER Stephen Moore, stephen.moore@linux.com

RUN zypper --non-interactive install mercurial

ENTRYPOINT ["hg"]

CMD ["--version"]
