MongoDB Init Script
=======

This is Init Script for MongoDB based on rpm.

rpm is here.
http://docs.mongodb.org/manual/tutorial/install-mongodb-on-redhat-centos-or-fedora-linux/

repository
https://github.com/mongodb/mongo/tree/master/rpm

Usage: 

    # mongod {start|stop|restart|status}


## Settings
Please change below values for your environment in each file.

in mongod

    MONGOHOME = "your mongo home path"

in mongod.conf

    dbpath = "your db path"

If you need you make 'data' dir on dbpath.


## Install and run

execute command as root.


    # cp mongod /etc/init.d/
    # chmod +x  /etc/init.d/mongod
    # cp mongod.conf /etc/
    # chkconfig --add mongod
    
    # service mongod {start|stop|restart|status}
