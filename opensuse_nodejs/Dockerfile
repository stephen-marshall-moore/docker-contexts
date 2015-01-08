FROM opensuse:13.2
MAINTAINER Stephen Moore, stephen.moore@linux.com

RUN zypper --non-interactive --gpg-auto-import-keys update
RUN zypper --non-interactive install nodejs

ENTRYPOINT ["node"]

CMD ["--version"]
