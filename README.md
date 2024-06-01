# glFTPd-manage
Directly manage users and groups, outside of glftpd.

# REQUIRES: 
```
awk, cut, grep, sed, hashgen(hashgen.c), passchk(pzs-ng)
```

# HELP:
```
root@server:~# bash gl-manage.sh -h

glFTPd-manage: glftpd user management tool
-----------------------------

Directly manage users and groups, outside of glftpd

USAGE:
  ./gl-manage.sh -c <COMMAND> [options]

COMMANDS:

  ADDUSER LISTUSERS LISTGROUPS RAWUSERFILE RAWUSERS RAWGROUPS RAWPGROUPS
  RAWUSERSGROUPS RAWUSERSPGROUPS RAWUSERGROUP RAWTAG RAWFLAG RAWCREDS DELUSER
  ADDGROUP DELGROUP CHGRP ADDUSERGROUP DELUSERGROUP ADDUSERPGROUP DELUSERPGROUP
  USERGADMIN CHGADMIN LISTIP RAWIP ADDIP DELIP CHPASS
  CHTAG CHFLAG CHCREDITS CHLOGINS CHRATIO ADDFLAG DELFLAG
  RAWUSERSTATS LISTUSERSTATS RESETUSERSTATS LOGTAIL LOGSHOW

OPTIONS:

  -a GADMIN      (ADDUSERGROUP|USERGADMIN)
  -d GROUPDESC   (ADDGROUP)
  -f FLAGS       (CHFLAG)
  -g GROUP       (ADDGROUP|DELGROUP|CHGRP)
  -i MASK        (ADDIP|DELIP)
  -k CREDITS     (CHCREDITS)
  -l LOGINS      (CHLOGINS)
  -u USERNAME    (ADDUSER|DELUSER|AUTH|*IP|*USERGROUP|CH*)
  -p PASSWORD    (ADDUSER|CHPASS|AUTH)
  -r RATIO       (CHRATIO)
  -s PGROUP      (ADDPGROUP|DELPGROUP)
  -t TAGLINE     (CHTAG)

REQUIRES: awk, cut, grep, sed, hashgen(hashgen.c), passchk(pzs-ng)
```
