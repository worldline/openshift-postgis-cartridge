openshift-postgis-cartridge
===========================

This cartridge provide Postgis, postgrsql need to be install first.

This cartridge do the folowing commands at install:

    psql $OPENSHIFT_GEAR_NAME -c "create language plpgsql;"
    psql -d $OPENSHIFT_GEAR_NAME -f /usr/share/pgsql/contrib/postgis-64.sql
    psql -d $OPENSHIFT_GEAR_NAME -f /usr/share/pgsql/contrib/spatial_ref_sys.sql

You also can connect to your app and execute this lines.
