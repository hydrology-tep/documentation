---
substitutions:
  manage: |-
    ```{image} ../includes/groups_manage.png
    ```
  minus: |-
    ```{image} ../includes/minus.png
    ```
  plus: |-
    ```{image} ../includes/plus.png
    ```
---

# WPS services management

The WPS services management page contains a list of all existing WPS services in DB, with the possibility for an Administrator to 

*Create*

 a new WPS service, 

*Update*

 or 

*Delete*

 an existing one.

When updating it, it is possible to set the Availability to "true" or "false" to make the service visible or not.

The Administrator can also 

*Manage*

 groups that can see each WPS provider (by clicking on 

{{ manage }}

). This will allow him to define if the WPS service is public (visible for all), private (visible only by the owner and administrators) or restricted only to a list of groups.

To add a group, click on 

{{ plus }}

 in front of the group's name in the 

*All Groups*

 panel.

To remove a group, click on 

{{ minus }}

 in front of the group's name in the 

*Allowed Groups*

 panel.

```{eval-rst}
.. req:: HEP-TS-DES-010
        :show:

        This section describes how an administrator can modify sharing authorization of a processing service.
```

```{eval-rst}
.. req:: HEP-TS-DES-011
        :show:

        This section describes how an expert can modify sharing authorization of a processing service.
```