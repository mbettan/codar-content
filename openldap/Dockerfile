FROM dinkel/openldap

MAINTAINER Christian Luginbühl <dinkel@pimprecords.com>

ADD ./ldap /etc/ldap.dist/prepopulate

EXPOSE 389

VOLUME ["/etc/ldap", "/var/lib/ldap"]

ENTRYPOINT ["/entrypoint.sh"]

CMD ["slapd", "-d", "32768", "-u", "openldap", "-g", "openldap"]
