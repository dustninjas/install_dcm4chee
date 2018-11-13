# install_dcm4chee
way ninja the install dcm4chee

# Commands

## docker-compose -p dcm4chee up -d
## docker-compose -p dcm4chee stop
## docker-compose -p dcm4chee start
## docker-compose -p dcm4chee down

1.  ##### Create and start the 3 containers by invoking

    ```text-shell-session
    $ docker-compose -p dcm4chee up -d
    Creating network "dcm4chee_default" with the default driver
    Creating dcm4chee_ldap_1 ...
    Creating dcm4chee_db_1 ...
    Creating dcm4chee_ldap_1
    Creating dcm4chee_db_1 ... done
    Creating dcm4chee_arc_1 ...
    Creating dcm4chee_arc_1 ... done
    ```

    in the directory containing `docker-compose.yml` and `docker-compose.env`.

2.  ##### You may stop all 3 containers by:

    ```text-shell-session
    $ docker-compose -p dcm4chee stop
    Stopping dcm4chee_arc_1  ... done
    Stopping dcm4chee_db_1   ... done
    Stopping dcm4chee_ldap_1 ... done
    ```

    and start all 3 containers again by:

    ```text-shell-session
    $ docker-compose -p dcm4chee start
    Starting db   ... done
    Starting ldap ... done
    Starting arc  ... done
    ```

3.  ##### You may stop and delete all 3 containers by

    ```text-shell-session
    $ docker-compose -p dcm4chee down
    Stopping dcm4chee_arc_1  ... done
    Stopping dcm4chee_db_1   ... done
    Stopping dcm4chee_ldap_1 ... done
    Removing dcm4chee_arc_1  ... done
    Removing dcm4chee_db_1   ... done
    Removing dcm4chee_ldap_1 ... done
    Removing network dcm4chee_default
    ```
