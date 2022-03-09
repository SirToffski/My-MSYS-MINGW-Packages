# Configuring mibdirs

Package compiles and installs successfully on mingw64. Limited testing with `snmpget` showed no immediate issues. 

However - after installing, `MIBDIRS` are not working correctly. A workaround is defining `MIBDIRS` environment variable. For example:

```bash
$ echo 'MIBDIRS="$(cygpath -a -w "$HOME/.snmp/mibs")\;$(cygpath -a -w "/mingw64/share/snmp/mibs")"' \
  >> ~/.bashrc
$ echo 'export MIBDIRS' >> ~/.bashrc
```

