# Admin Tools

</br>

## Subjects and Roles

Information on how to use security on this [dedicated page](../security).  

</br>

## Database Maintenance

Your Database will require maintenance as nothing in Nightscout is setup to perform cleanup and unless you planned for a larger size database it will eventually [fill-up](../../troubleshoot/troublehoot/#database-full). Make sure you leave [`dbsize`](../setup_variables/#dbsize-database-size) visible on your page to keep it under control.

</br>

This panel will give access to basic maintenance actions on various database collections as defined in your site [core](../../nightscout/setup_variables/#core) variables.

</br>

### Mongo `status` Database

</br>

Your status database contains battery, pump, ... extra information as those defined in [devicestatus](../setup_variables/#devicestatus-device-status) that you can safely delete when necessary.

<img src="../img/Admin07.png" style="zoom:80%;" />

</br>

When it comes to `treatments` and `entries`, deleting data is something you need to carefully evaluate if you like Nightscout to be the main repository for your history.

### Mongo `treatments` Database

</br>

<img src="../img/Admin08.png" style="zoom:80%;" />

</br>

### Mongo `entries` Database

</br>

<img src="../img/Admin09.png" style="zoom:80%;" />

</br>

### Remove future items from Database

</br>

Future treatments and entries generated by an incorrect time zone, daylight saving time change, or any other mistake can completely block your site. Using this feature will purge the database of these unwanted values automatically. Detected issues will appear in `Database contains `*`x`*` future records` and should be fixed.

</br>

<img src="../img/Admin10.png" style="zoom:80%;" />

</br>
