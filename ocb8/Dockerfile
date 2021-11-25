FROM odoo:8

USER root

RUN wget https://github.com/OCA/OCB/archive/8.0.zip; \
    echo '27307f308bb245ff408cef88c9f71d07c00c309a 8.0.zip' | sha1sum -c -; \
    unzip *.zip; \
    rm *.zip; \
    mv OCB-8.0/* ./; \
    rm -R OCB-8.0;


USER odoo
