---
title: "Systems"
weight: 10
---

{{< toc >}}

## Connecting Systems to TrueCommand

To connect a system to TrueCommand, open the **Configure** <i class="material-icons" aria-hidden="true" title="Settings">settings</i> menu and click *Systems*.
This menu is organized into two tabs: **Systems** and **System Groups**.
The **Systems** and **System Groups** tabs contain all the options to connect and organize systems in TrueCommand.
All added systems are listed in the **Systems** tab with the current connection status.

![Systems List](/images/TrueCommand/2.0/SystemsPage.png "Systems List")


### Adding a System Manually

To connect a new system, click **+ NEW SYSTEM**.

Enter the system IP address or DNS hostname, the nickname, and the password.
If you make a mistake, you can reset the form by clicking *RESET FORM*.

![Systems Add](/images/TrueCommand/2.0/SystemsAddNew.png "Systems Add")

### Adjusting Systems

Each system has its own control area with what options are available.

+ Pause Data Polling : <i class="material-icons" aria-hidden="true" title="Pause Data Polling">pause</i>
+ Start Data Polling : <i class="material-icons" aria-hidden="true" title="Start Data Polling">play_arrow</i>
+ Edit System : <i class="material-icons" aria-hidden="true" title="Configure">edit</i>
+ Update System : <i class="material-icons" aria-hidden="true" title="System Update">system_update_alt</i>
+ Reconnect System : <i class="material-icons" aria-hidden="true" title="Refresh">refresh</i>
+ Delete System : <i class="material-icons" aria-hidden="true" title="Delete">delete</i>

{{< tabs "System Control Options" >}}
{{< tab "Pause" >}}

If the pause button <i class="material-icons" aria-hidden="true" title="Pause Data Polling">pause</i> is visible, TrueCommand is actively polling data from the NAS.  Clicking this button will stop data collection until it is manually restarted.

![Systems Pause Polling](/images/TrueCommand/2.0/SystemsPausePollingSystem.png "Systems Pause Polling")

{{< /tab >}}
{{< tab "Start" >}}
If the play button <i class="material-icons" aria-hidden="true" title="Start Data Polling">play_arrow</i> is visible, TrueCommand is not collecting any data from the NAS.  To start data polling, click the play button.

![Systems Start Polling](/images/TrueCommand/2.0/SystemsStartPollingSystem.png "Systems Start Polling")

{{< /tab >}}
{{< tab "Edit" >}}
Clicking the edit button <i class="material-icons" aria-hidden="true" title="Configure">edit</i> opens a side bar menu.  Adjustments can be made to the system in this meny.  Click **Save Changes** to update the system to the new values entered. 
Clicking **Reset Form** will reset the form to the previous saved settings for the NAS.

![Systems Edit](/images/TrueCommand/2.0/SystemsEditSystem.png "Systems Edit")

{{< /tab >}}
{{< tab "Update" >}}
If updates are available on the system, the Update column will say *Available* and the update button <i class="material-icons" aria-hidden="true" title="System Update">system_update_alt</i> will be visible. 
Clicking the update button will open a popup window requiring you to confirm your desire to update the system.

![Systems Update](/images/TrueCommand/2.0/SystemsUpdateNAS.png "Systems Update")

{{< /tab >}}
{{< tab "Reconnect" >}}
If a system has lost its connection to TrueCommand either through maintainence or being powered off, click the reconnect button <i class="material-icons" aria-hidden="true" title="Refresh">refresh</i> to trigger TrueCommand to reconnect with the NAS.  Reconnecting may take several minutes.  If data polling was paused before the system was disconnected, data polling will remain paused. Data polling must be manually restarted with the play button.

{{< /tab >}}
{{< tab "Delete" >}}
Clicking the <i class="material-icons" aria-hidden="true" title="Delete">delete</i> button will initiate a popup confirmation box to delete a system.

![Systems Delete](/images/TrueCommand/2.0/SystemsDeleteSystem.png "Systems Delete")

{{< hint warning >}}
Deleting a system will purge all collected data from the database.
{{< /hint >}}
{{< /tab >}}
{{< /tabs >}}

## Organizing Systems into Groups

Groups are collections of systems that are organized by TrueCommand administrators.
Grouping systems allows you to efficiently manage system permissions and reporting.

Open the **System Groups** tab to view the list of created groups and the systems they contain.

![SystemsGroups](/images/TrueCommand/2.0/SystemsGroups.png "System Groups")

Create a Group by clicking **Configure <i class="material-icons" aria-hidden="true" title="Settings">settings</i>&nbsp; > Systems > + NEW GROUP**.
Enter a name for the new group and click *ADD SYSTEM* to add a system to the group.
When you've added all the desired systems to the group, click *CREATE GROUP*.

![SystemsNewGroup](/images/TrueCommand/2.0/SystemsGroupsNewGroup.png "New System Group")

### Adjusting Groups

Each group has its own control area with what options are available.

+ Edit System : <i class="material-icons" aria-hidden="true" title="Configure">edit</i>
+ Delete System : <i class="material-icons" aria-hidden="true" title="Delete">delete</i>

{{< tabs "Group Control Options" >}}
{{< tab "Edit" >}}
Clicking the edit button <i class="material-icons" aria-hidden="true" title="Configure">edit</i> opens a side bar menu.  Adjustments can be made to the Group in this manner.  Systems can be added or removed from the group by using the **Add System** button or the Remove <i class="material-icons" aria-hidden="true" title="Delete">delete</i> button.  Click **Save Changes** when finished with your changes to update the Group to the new group settings.

![Groups Edit](/images/TrueCommand/2.0/SystemsGroupsEditGroup.png "Groups Edit")

{{< /tab >}}
{{< tab "Delete" >}}

Clicking the <i class="material-icons" aria-hidden="true" title="Delete">delete</i> button will initiate a popup confirmation box to delete a group. 

![Groups Delete](/images/TrueCommand/2.0/SystemsGroupsDeleteGroup.png "Group Delete")

{{< /tab >}}
{{< /tabs >}}
