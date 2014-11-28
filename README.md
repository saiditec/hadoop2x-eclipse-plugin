hadoop2x-eclipse-plugin
=======================

eclipse plugin for hadoop  2.5.2
 

How to build
----------------------------------------

```bash
cd src/contrib/eclipse-plugin 

ant jar -Dversion=2.5.2 -Declipse.home=$ECLIPSE_HOME -Dhadoop.home=${HADOOP_HOME}

# final jar will be genaratd at 'build/contrib/eclipse-plugin/'
```

options required
--------------------------------------
  ECLIPSE\_HOME: path of eclipse home 

  HADOOP\_HOME: path of hadoop 2.x home
 

How to debug
--------------------------------------
  start eclipse with debug parameter:  

    /opt/eclipse/eclipse -clean -consolelog -debug
How to use
--------------------------------------
* Copy *hadoop-eclipse-Luna-plugin-2.5.2.jar* from *build/contrib/eclipse-plugin* to *ECLIPSE\_HOME/plugins*.
* Reboot your eclipse.
* Create a new project, select *Map/Reduce Project* from the list.
* Set your hadoop home .
* Append hbase lib to your build path if required.
