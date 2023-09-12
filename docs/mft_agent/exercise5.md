---
sidebar_label: 'Exercise 5'
---

# Exercise 5

### Objective

To utilize wildcards to move files with different extentions between two endpoints.

### Summary

This task will move a selection of files with **.txt** and **.dat** extentions from the source endpoint, **SVR_INPUT**, to the destination endpoint, **SVR_OUTPUT**.

### Instructions

#### Defining the Job

##### In Solution Manager
1.  Select **Library**.
2.  Select **Master Job**.
3.  Click the **Add** button.

##### In the Master Job Definition screen

4.  In the **Schedule** drop-down, select **My MFT Schedule**
5.  In the **Name** field, enter **MFT Multiple Extentions**.
6.  In the **Job Type** drop-down, select **OpConMFT**.
7.  Expand **Task Details**.
8.  In the **General** section, select the **OpConMFT** machine.
9.  In the **Source** section,
    * Select the **SVR_INPUT** endpoint from the **Endpoint** drop-down.
    * Enter **MFT_File_05?.txt|MFT_File_05?.dat** in the **File Filter** field.
    * Enter **5** in the **Timeout __ minutes** field.
10. In the **Destination** section
    * Select the **SVR_OUTPUT** endpoint from the **Endpoint** drop-down.
    * Select **Ture** from the **Overwrite** drop-down.
11. Click **Save**
12. Click the lock icon to enter **Admin Mode**.
13. Expand **Frequency** and move the **Inactive** frequency called **Example-Mon-Fri-O** into the **Active** column.
14. Click **Save**.
15. Close **Library**.

#### Add the Job to the Schedule

16. Select the **Operations**.
17. In **Operations Summary**, click **Processes** in the top right-hand corner.
18.	Select today's date in the **Date** column.
19. Right-click on **My MFT Schedule** in the **Schedule** section.
20. Click the **plus sign ( + )** in the **Schedule Selection** menu.

#### In the **Add Job(s)** Pop-up

21. Select the **MFT Multiple Extentions** job.
22. Click **Next**.
23. Select **Release** for the **Build Status**.
24. Click **Next**.
25. Verify that the information is correct and click **Submit**.
26. Click **Close**.

#### In the Process Screen

27. Verify that the job was added and ran successfully.
28. Close **Operations**.