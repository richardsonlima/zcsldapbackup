## The zcsldapbackup tool that does hot backup and hot restore of ZCS Opensource LDAP (ldif files) accounts per DOMAIN. ##

**zcsldapbackup provides**

  * Full backup of ldap (ldif file) all accounts;
  * Full backup of ldap (ldif file) any account;
  * Full backup of ldap (ldif file) any account aliases;
  * Full backup of ldap (ldif file) any distribution lists;

  * Restore of ldap (ldif file) all accounts;
  * Restore of ldap (ldif file) any account;
  * Restore of ldap (ldif file) any account aliases;
  * Restore of ldap (ldif file) any distribution lists;

**History: Based on Zmbkpose created By Rubens Alonso Filho <rubens@harv.com.br> <rubens@4linux.com.br>**

**Rewritten and applied only for zimbra ldap backup by Richardson Lima <richardsonlimasurfjiujitsu@gmail.com>

---

## [zimbra@server ~]$ zcsldapbackup ##** Usage:

> ` zcsldapbackup --ldap `
  * Execute full backup ldif file, all accounts.
> ` zcsldapbackup --ldap mail1,mail2,...,mailn `
  * Execute backup ldif file for specific accounts.
> ` zcsldapbackup --backupDistributionList `
  * Make full backup of Distribution  Lists.
> ` zcsldapbackup --backupAlias `
  * Make full backup of Alias.


## [zimbra@server ~]$ zcsldaprestore ##
**Usage:**

> ` zcsldaprestore --ldap `
  * Execute full restore ldif file, all accounts.
> ` zcsldaprestore --ldap mail1,mail2,...,mailn `
  * Execute restore ldif file for specific accounts.
> ` zcsldaprestore --restoreDistributionList `
  * Restore all distribution lists from last backup.
> ` zcsldaprestore --restoreAlias `
  * Restore all alias from last backup.