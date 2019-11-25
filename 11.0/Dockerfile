FROM odoo:11

USER root
RUN set -x; \
        curl -o odoo.deb -SL http://nightly.odoo.com/11.0/nightly/deb/odoo_11.0.20181114_all.deb \
        && dpkg --force-depends -i odoo.deb \
        && rm odoo.deb

USER odoo
