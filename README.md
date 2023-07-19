# EIDF Status Repository

## Update status

Edit File for Service

```json
{
  "schemaVersion": 1,
  "label": "Unavailable",
  "labelColor": "red",
  "message": "Under Investigation",
  "color": "grey"
}
```

Change label to a short status wording - Active, At Risk, Down or similar to this.

Change labelColor to a suitable colour - brightgreen,green, yellowgreen, yellow, orange, red, blue, lightgrey, blueviolet

Change message to a short description wording - Under investigation, Repair, Beta Test

Leave color at grey unless important.

Commit Update to the repository

Update of status will take effect on the gh-pages update for the repository - can take up to 10-20minutes in some cases.

Status will be updated when a user refreshes the documentation.

## Update Portal Alert on the main page

Update [Data/portal-alert.json](Data/portal-alert.json):

```json
{
  "highlight": "danger",
  "header": "Openstack/DSC Full Maintenance 20 July 2023 between 0900 and 1700 BST",
  "text": "This session will involve some outage to services (EIDF Portal, SSH Gateway, Guacamole) as we apply necessary patches and upgrades to the service and underlying infrastructure. We do not envisage that VMs will stop during that time, but they may be inaccessible for the duration."
}
```

Change `highlight` to a suitable colour - danger (red), warning (yellow), success (green).

Change `text` to the detailed description wording.

Change `header` to the header of the alert, include start and end date and time if available

Status will be updated when the user refreshes the main page.

To remove the alert change to empty:
```json
{}
```
