# Configuration examples

These are small references from my deployment, not a one-command installer.

| File | Where I used it |
| --- | --- |
| `apache-prestashop.conf` | `/etc/apache2/sites-available/prestashop.conf` |
| `prestashop.ini` | `/etc/php/8.3/mods-available/prestashop.ini` |
| `doctrine-tls.example.yml` | Excerpt merged into `app/config/doctrine.yml` |

Replace the Apache hostname, preserve existing application configuration and back up files before editing. The Doctrine example deliberately omits credentials and is not a complete configuration file. The separate legacy PDO adjustment is explained in [Troubleshooting](../docs/troubleshooting.md).
