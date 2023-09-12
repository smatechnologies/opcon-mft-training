---
sidebar_label: 'Exercise 1'
---

# Exercise 1

### Objective

To successfully add an MFT Agent and establish communication.

### Summary

You will utilize the **Configurator** to get the Port Number of the Agent. Then using Solution Manager, add a new MFT Agent and establish communication with it.

### Instructions

##### Getting the Port Number

1.  In a File Explorer window, navigate to ```C:\Program Files\OpConxps\MFTAgent```.
2.  Open the **Configurator** utiiliy.
3.  Choose **System**.
4.  Click **Yes** in the Windows pop-up.
5.  Select **Scheduler** in the navigation panel on the left.
6.  Select the **Schedule Settings** tab.
7.  Make note of the **UI Port** number.
8.  Leave the **Configurator** open.

##### Defining the Agent

9.  In **Solution Manager**, select **Library**
10. Select **Agents**.
11. Click the **Add** button.
12. In the **Name** field, enter **OpConMFT**.
13. In the **Type** drop-down list, select **OpConMFT**.
14. Expand the **General Settings** section.
15. In the **IP Address field, enter in your Windows IP Address.
16. In the **Socket Number** field, enter in the **UI Port** number you made note of in Step 6.
17. Click **Save**
18. Expand the **Communication Settings** section.
19. In the **JORS Port Number** field, enter in the **UI Port** number you made note of in Step 6.
20. Click **Save**.

##### Authentication of the MFT Agent

22. Navigate back to the **Configuration** utility.

:::info Note
The **Congifuration** unitility should still be opened and the icon should show in your tool bar at the bottom of your RDP session. If it is not, follow Steps 1-5 to get back to the **Schedule Settings** tab.
:::

23. In the **Schedule Settings** tab, click the **Resest Auth Token Dedline**.
24. In the **Agent Details** screen in **Solution Manager** click the **Authenticate** button.
25. Click the **Change Communication Status** button.
26. Select **Enable Full Comm. (Job Start Enabled)**.
