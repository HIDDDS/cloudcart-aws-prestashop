# My validation record

[Back to the project](../README.md)

I completed the following checks during the deployment, with the final browser tests on **12 October 2026**. These are historical results, not an uptime guarantee.

| Check | Recorded result | Evidence |
| --- | --- | --- |
| New EC2 application instance | Running | [EC2](screenshots/ec2.png) |
| Database hosted separately | RDS instance and endpoint | [RDS](screenshots/rds.png) |
| RDS public access | Set to No during provisioning | [Private access](screenshots/private.png) |
| Application MySQL login | Expected user and schema returned | [Database query](screenshots/dbproof.png) |
| Apache configuration | Syntax OK | [Apache check](screenshots/apacheproof.png) |
| Local installer endpoint | HTTP 200 | [Apache check](screenshots/apacheproof.png) |
| PrestaShop installation | All stages completed | Installer (image provided separately) |
| Administrator access | Dashboard opened | Dashboard (image provided separately) |
| Public storefront | Products, prices and images loaded in Incognito | [Storefront](screenshots/public.png) |
| Shopping cart | One product added | [Cart](screenshots/cart.png) |

## What I have not claimed

- I did not test a payment transaction or complete checkout.
- I did not deploy HTTPS, high availability or autoscaling.
- I have not included a final billing statement or a backup restoration test.
- My screenshots do not prove every final security-group source, storage-encryption setting or filesystem permission.
- Installer-directory removal and final post-install permissions still need explicit verification before wider use.
- The PDO TLS core-file adjustment needs review after application upgrades.

## Improvements I would make next

1. Configure HTTPS before handling real users or customer data.
2. Verify installer removal and tighten post-install filesystem permissions.
3. Review the TLS configuration against the application's supported extension/configuration options before upgrading.
4. Configure monitoring and test backup restoration.
5. Rebuild the infrastructure with version-controlled infrastructure as code.

## Project report

My 19-page implementation report (provided separately) contains the fuller sequence and 26 screenshot figures, including early configuration states and troubleshooting evidence.
