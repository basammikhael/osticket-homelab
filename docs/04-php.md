# 4. PHP

## Install

- Installed the Visual C++ 2015-2022 x64 runtime, which PHP requires.
- Downloaded PHP 8.3 **x64 Non Thread Safe**. osTicket 1.18 supports PHP 8.2 to 8.4, so 8.5 was too new.
- Extracted to `C:\PHP`.
- Copied `php.ini-production` to `php.ini`.

![PHP 8.3 x64 Non Thread Safe](../images/09-php-83-x64-nts.png)

## Register with IIS

Installed PHP Manager for IIS and registered `C:\PHP\php-cgi.exe`.

![PHP Manager](../images/10-php-manager.png)

## Extensions

Enabled: mysqli, gd, intl, mbstring, fileinfo, imap, curl, openssl, and ldap (for Active Directory login later).

![PHP extensions](../images/11-php-extensions.png)

## Verify

phpinfo loads through IIS and shows PHP 8.3.35 on TICKET01.

![phpinfo](../images/12-phpinfo.png)
