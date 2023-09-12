---
sidebar_label: 'Exercise 2'
---

# Exercise 2

### Objective

To successfully define two Path Endpoints.

### Summary

Define the source endpoint, **SVR_INPUT**, with a path of ```C:\MFT_Training\Input``` and a destination endpoint, **SVR_OUTPUT**, with a path of ```C:\MFT_Training\Output```.

### Instructions

#### Define the Path Endpoints

##### In Solution Manager

1.  Select **Library**.
2.  Select **Agents**.
3.  Right-click on the **OpConMFT** agent to open the side menu.
4.  Click on the wrench icon to view the **Agent Details** screen.
5.  Expand the **OpCon MFT Agent Settings** section.
6.  Click the blue hyperlink called **Path Endpoints**.

:::info Note
This will open in a new tab in your Chrome browser.
:::

##### In the Path Endpoints Tab

7.  Select **Add Site**.
8.  Enter **SVR_INPUT** for the **Site Name**.
9.  Enter ```C:\MFT_Training\Input``` for the **Directory Name**.
10. Select **OK** to save new definition.
11. Repeat Steps 7-10 to define a second site with the following settings:
    * **Site Name**: SVR_OUTPUT 
    * **Directory**: ```C:\MFT_Training\Output```.
12. Close the **Path Endpoints** tab.
13. Navigate back to **Solution Manager** and close both **Operations** and **Library**.
