MongoDB Init Script
=======

# This is Init Script for MongoDB.

Usage: mongod {start|stop|restart|status}


Please change below values for your environment.

* mongod

    -MONGOHOME
    -CONFIGFILE

* mongod.conf

    -dbpath

If you need you make 'data' dir on dbpath.

and execute command as root.


    # cp mongod /etc/init.d/
    # cp mongod.conf /etc/
    # chkconfig --add mongod
    
    # service mongod {start|stop|restart|status}
