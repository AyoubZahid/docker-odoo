
FROM odoo:12

USER root
#RUN pip3 install pysftp
RUN set -x; \
        curl -o odoo.deb -SL http://nightly.odoo.com/12.0/nightly/deb/odoo_12.0.latest_all.deb \
        && dpkg --force-depends -i odoo.deb \
        && rm odoo.deb

USER odoo
