MongoDB Init Script
=======

This is Init Script for MongoDB based on rpm.

rpm is here.
http://docs.mongodb.org/manual/tutorial/install-mongodb-on-redhat-centos-or-fedora-linux/

Usage: 

    # mongod {start|stop|restart|status}


Please change below values for your environment.

mongod

    MONGOHOME
    CONFIGFILE

mongod.conf

    dbpath

If you need you make 'data' dir on dbpath.

and execute command as root.


    # cp mongod /etc/init.d/
    # cp mongod.conf /etc/
    # chkconfig --add mongod
    
    # service mongod {start|stop|restart|status}
