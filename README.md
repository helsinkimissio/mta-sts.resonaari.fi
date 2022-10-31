## MTA STS Policy

Resonaari.fi's SMTP MTA Strict Transport Security Policy adds a security layer between the sending and receiving email server.

| Tag | Value |
| --- | --- |
| version | STSv1 |
| mode | testing |
| mx | resonaari-fi.mail.protection.outlook.com |
| max_age | 86400 |

Lines of MX tags should always list the current MX servers for the domain, one server per line. The servers can be queried with the command:

```
% host -t MX resonaari.fi
resonaari.fi mail is handled by 50 resonaari-fi.mail.protection.outlook.com.
```

## MTA STS Record

| Tag | Value |
| --- | --- |
| v | STSv1 |
| id | 202210310725 |

The id tag value should be updated on each policy change. The current value can be resolved using the command:

```
% host -t TXT _mta-sts.resonaari.fi
_mta-sts.resonaari.fi descriptive text "v=STSv1; id=202210310725;"
```
