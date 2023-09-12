---
sidebar_label: 'Exercise 3'
---

# Exercise 3

### Objective

To successfully transfer a single file between two endpoints.

### Summary

Move a file, **MFT_File_1.txt**, from the source endpoint, SVR_INPUT, to the destination endpoint, SVR_OUTPUT.

### Instructions

#### Defining the Job

##### In Solution Manager
1.  Select **Library**.
2.  Select **Master Job**.
3.  Click the **Add** button.

##### In the Master Job Definition screen

4.  In the **Schedule** drop-down, select **My MFT Schedule**
5.  In the **Name** field, enter **MFT Single File Transfer**.
6.  In the **Job Type** drop-down, select **OpConMFT**.
7.  Expand **Task Details**.
8.  In the **General** section, select the **OpConMFT** machine.
9.  In the **Source** section,
    * Select the **SVR_INPUT** endpoint from the **Endpoint** drop-down.
    * Enter **MFT_File_03.txt** in the **File Filter** field.
    * Enter **5** in the **Timeout __ minutes** field.
10. In the **Destination** section
    * Select the **SVR_OUTPUT** endpoint from the **Endpoint** drop-down.
    * Select **Ture** from the **Overwrite** drop-down.
11. Click **Save**
12. Click the lock icon to enter **Admin Mode**.
13. Expand **Frequency** and move the **Inactive** frequency called **Example-Mon-Fri-O** into the **Active** column.
14. Click **Save**.
15. Close **Library**.

#### Build the Schedule

16. Select the **Operations**.
17. In **Operations Summary**, click **Schedule Build** in the top right-hand corner.

##### In the Schedule Build screen

18.	In the **Scheduling Dates** section, select today's dates for **From** and **To** using the Calendar Icon.
19.	In **Schedule Build** section, select the **Released** option .
20. In the **Schedule List**, select **My MFT Schedule**.
21. Click the **Build** button.
22.	On the **Build Results** screen, expand the dropdown menu and click down to select and click on **My MFT Schedule**.
23.	The **Processes** screen will allow review of the Job Run results and details.
