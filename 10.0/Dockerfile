FROM odoo:10

USER root

RUN set -x; \
        curl -o odoo.deb -SL http://nightly.odoo.com/10.0/nightly/deb/odoo_10.0.latest_all.deb \
        && dpkg --force-depends -i odoo.deb \
        && rm odoo.deb

USER odoo
