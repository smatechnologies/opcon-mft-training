---
sidebar_label: 'Exercise 13'
---

# Exercise 13

### Objective

To compress and encrypt a single job.

### Summary

To compress and encrypt a single file, MFT_File_13.txt, using the **TrainingKey** to encrypt the file during the transfer and place it in the  destination endpoint, **SCR_OUTPUT**.

### Instructions

##### In Solution Manager
1.  Select **Library**.
2.  Select **Master Job**.
3.  Click the **Add** button.

##### In the Master Job Definition screen

4.  In the **Schedule** drop-down, select **My MFT Schedule**
5.  In the **Name** field, enter **MFT Compression and Encryption Transfer**.
6.  In the **Job Type** drop-down, select **OpConMFT**.
7.  Expand **Task Details**.
8.  In the **General** section, select the **OpConMFT** machine.
9.  In the **Source** section,
    * Select the **SVR_INPUT** endpoint from the **Endpoint** drop-down.
    * Enter **MFT_File_13.txt** in the **File Filter** field.
    * Enter **5** in the **Timeout __ minutes** field.
10. In the **Destination** section
    * Select the **SVR_OUTPUT** endpoint from the **Endpoint** drop-down.
    * Select **Ture** from the **Overwrite** drop-down.
11. In the **Compression** section
    * Select **Compress** in the **Action** dropdown.
    * Enter **MFTFiles_13.zip** in the **File Name** field.
12. In the **Encryption** section
    * Select **Encrypt** in the **Action** dropdown.
    * Enter **\*** in the **File Filter** field.
    * Select the **TrainingKey** from the **Key** drop-down.
    * Verify that **SHA256** is selected for the **Signature Type**.
13. Click **Save**
14. Click the lock icon to enter **Admin Mode**.
15. Expand **Frequency** and move the **Inactive** frequency called **Example-Mon-Fri-O** into the **Active** column.
16. Click **Save**.
17. Close **Library**.

#### Add the Job to the Schedule

18. Select the **Operations**.
19. In **Operations Summary**, click **Processes** in the top right-hand corner.
20.	Select today's date in the **Date** column.
21. Right-click on **My MFT Schedule** in the **Schedule** section.
22. Click the **plus sign ( + )** in the **Schedule Selection** menu.

#### In the **Add Job(s)** Pop-up

23. Select the **MFT  Compression and Encryption Transfer** job.
24. Click **Next**.
25. Select **Release** for the **Build Status**.
26. Click **Next**.
27. Verify that the information is correct and click **Submit**.
28. Click **Close**.

#### In the Process Screen

29. Verify that the job was added and ran successfully.
30. Close **Operations**.