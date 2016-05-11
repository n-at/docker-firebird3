Docker Firebird 3 Superserver
=============================

Image contains Firebird 3 with Superserver architecture.

Usage
-----

Set **SYSDBA** password via `FIREBIRD_PASSWORD` environment variable (default is `masterkey`).

Default directory for databases is `/sqlbase`.

    $ docker run -d \
        -p 3050:3050 \
        -v /sqlbase:/sqlbase \
        -e FIREBIRD_PASSWORD=secret \
        atnurgaliev/firebird3

License
-------

BSD
