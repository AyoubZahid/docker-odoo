FROM odoo:11

USER root
RUN pip3 install xlwt==1.1.2
RUN set -x; \
        curl -o odoo.deb -SL http://nightly.odoo.com/11.0/nightly/deb/odoo_11.0.latest_all.deb \
        && dpkg --force-depends -i odoo.deb \
        && rm odoo.deb

USER odoo
