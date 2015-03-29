# jdbc2_fdw
This repo contains code that is a fusion between the postgresql_fdw that is distributed with PostgreSQL 9.4 and
JDBC_FDW (git://github.com/atris/JDBC_FDW.git) that was based on an older version of PostgreSQL and has not been
maitained.

The first goal with this code is to be able use the Query deparser to combine conditions from the submitted query and the
defintion of the the foreign table, so conditions are evaluated remotely, rather than ignored by the remote and applied
locally as is the case with JDBC_FDW.

Later on the DML support for Insert/Update/Delete over JDBC might be added.
