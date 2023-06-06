---
substitutions:
  update: |-
    ```{image} ../includes/update.png
    ```
---

# WPS providers management

The WPS providers management page contains a list of all existing WPS providers in DB, with the possibility for an Administrator to 

*Create*

 a new WPS provider, 

*Update*

 or 

*Delete*

 an existing one.

The Administrator can 

*Update*

 a WPS provider (by clicking on 

{{ update }}

). This action will do a request to the WPS provider (GetCapabilities) to check wethere there are new WPS services available. If so, these services will be automatically added to the list of existing WPS services in DB.

The Administrator can enable the Auto synchronization of a wps provider. This mean that new available processes will be automatically discovered and made available to the platform.

```{eval-rst}
.. req:: HEP-TS-DES-010
        :show:

        This section describes how an administrator can manage users.
```
