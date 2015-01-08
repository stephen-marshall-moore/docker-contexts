FROM opensuse
MAINTAINER Stephen Moore, stephen.moore@linux.com

RUN zypper update
RUN zypper --non-interactive install mercurial

ENTRYPOINT ["hg"]

CMD ["--version"]
