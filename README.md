# MTA STS Policy

| Tag | Value |
| --- | --- |
| version | STSv1 |
| mode | testing |
| mx | resonaari-fi.mail.protection.outlook.com |
| max_age | 86400 |

The mx line(s) should always contain all the MX servers of the domain. They can be queried with the command:

```
% host -t MX resonaari.fi
resonaari.fi mail is handled by 50 resonaari-fi.mail.protection.outlook.com.
```
