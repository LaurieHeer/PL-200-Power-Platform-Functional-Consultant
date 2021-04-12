---
lab:
    title: 'Lab 3.1: Creating an app'
    module: 'Module 3: Work with Dataverse'
---

Module 3: Work with Dataverse
=================================

## Lab 3.1: Practice Lab – Creating an app

### Important Notice (Effective November 2020):
Common Data Service has been renamed to Microsoft Dataverse. Some terminology in Microsoft Dataverse has been updated. For example, entity is now table and field is now column. 

While the application is in the process of updating its user experience, some references to terminology like the Common Data Service (now **Dataverse**), entity (now **table**), field (now **column**), and record (now **row**) may be out of date. Please keep this in mind as you work through the labs. We expect to have our content fully up to date very soon. 

For more information and for a complete list of affected terms, please visit [What is Microsoft Dataverse?](https://docs.microsoft.com/en-us/powerapps/maker/common-data-service/data-platform-intro#terminology-updates)

Scenario
--------

You are a functional consultant for your organization Contoso. You are assigned
to work on a project for your client Fabrikam. Fabrikam would like to encourage
their employees to continuously learn.  They want to build an application that 
allows a small set of employees to create knowledge assessments and then make
them available to all employees to test their knowledge.  The employees need to
be able to pick an assessment and quickly complete it in just a few minutes. In
this practice, you will be creating the apps necessary to support this effort.

Working with the solution architect on the project you have determined that you
will create two apps.

**Fabrikam Knowledge Admin** – this will be a model-driven application that you
can quickly enable creation of the knowledge assessments by the users.

**Fabrikam Knowledge** – this will be a canvas app that will be a custom user experience making it easy to find the assessments and take them.

In this practice, you will be starting the creation of these applications and
will build them out as you progress through the course. You will also create one of the template applications so you can see how easy it is to get started using a “Make from data” template.

Exercise 1 – Review Templates and Create App from Data
------------------------------------------------------

In this exercise, you will review the template and sample apps that are
available on the maker portal. You will also create an app using the Create from data templates to see how quickly that can get a basic canvas app started.

### Task 1 – Review + Create templates/samples

If you have time, you can choose any of these and select Make It and explore on
your own.

1.  Navigate to <https://make.powerapps.com>. You may need to sign in again using your credentials if necessary. 

2.  Switch to your **Practice** environment by using the Environment Selector in the upper right corner of the screen. (It will probably say **Contoso (Default)**.) Select your **Practice** environment from the list.

3.  Select **+ Create** from the left-hand navigation.

4.  Review the different apps that are available to use as both samples and
    starting templates.

5.  If you have time, choose any of these and select **Create** When you are done proceed to Task 2.

### Task 2 – Create an app over data for Account

Starting a canvas app from data is a quick way to start a canvas app when the
goal is to have a list of data from an entity. 

1.  Select **+ Create** again.

2.  Click **Canvas app from blank**. In the dialog box, name your app **Fabrikam Accounts** and select **Phone** layout.

3.  Click **Create** in the dialog. (You may be required to sign in again; enter your tenant credentials if necessary.)

4.  Your app should open in the designer. (You may get a few pop-ups first; close them.) Use the zoom slider to increase the size of your canvas. In the blank canvas, click the **connect to data** link.

5.  The **Data** pane will open. Select **+ Add data**. From the list of entities, then select **Accounts**.

6.  Open the **Insert** pane by clcking the **+** button on the left hand tab. Add a header to your app by adding a **Text label** to your canvas. Use the **Properties** pane on the right side of the screen to enter **Fabrikam Accounts** in the **Text** field. You can edit the size, font, and other attributes to customize the look and feel of the application. Explore other options available in the **Advanced** pane.

7.  Add a list of accounts to your app by selecting the **+** button on the left tab. Expand the **Layout** section. Add a **Vertical Gallery** to your canvas.

8.  A vertical gallery will be inserted into your app, and you will be prompted to select which data source it should pull from. Select **Accounts** from the pop-up.

9.  The application will load list of the accounts. Drag the gallery to fit the app or resize to your liking.

10. To preview your app, click **Play** (it will look like a Play button) in the upper right corner. Explore and then close the preview window.

11.  Click **File** and select **Save**.

12.  Select the **Cloud** and enter **Fabrikam Accounts** in the **Name**
    box.

13.  Click **Save**.

14. Explore the app as much as you want and then proceed to the next exercise.
    This app will be saved, and you can always revisit it later.

15. Close the **App Designer** browser tab.

Exercise 2 – Create the model-driven app
----------------------------------------

In this exercise, you will be creating the Knowledge Admin model-driven app. In
the data modeling module, you will be creating all the entities, so getting this
started will be easy.

### Task 1 – Create a model-driven app

1.  Open <https://make.powerapps.com> and make sure you are in your
    **Practice** environment.

2. Click on **+ Create** and select **Model-driven app from blank.** Select **Create** in the pop-up window.

3.  Enter **Knowledge Admin** for Name and click **Done**.

4.  Click the edit icon (it looks like a pencil) next to **Site Map**. *Note:* When you start a new app, you must edit the site map before you can run it - otherwise you will get an error. You need to add at least one item to the navigation.

5.  Click on **New Area** to open the **Properties** pane.

6.  Enter **Administration** for **Title**.

7.  Select **New Group**.

8.  Enter **User Admin** for **Title**.

9.  Select **New Subarea**.

10.  Select **Entity** for **Type**.

11. Select **User** for **Entity**.

12. **Save** the Sitemap Designer.

13. **Publish** the Sitemap Designer.

14. Click **Save and Close** to close the Sitemap Designer and return to the App Designer. 

15. Click **Save** to save your changes to the App Designer. Click **Publish**. After publishing, click **Save and Close** to close the App Designer.

16. Select **Apps**.

17. The **Knowledge Admin** application you created should be listed. Open the
    **Knowledge Admin** application by selecting the row and clicking **Play.**

18. The **Model-Driven** application **Knowledge Admin** will load.

19. Open one of the **Users**.

20. The User form of the selected record will load.

21. Close the application by closing the browser tab.

Exercise 3 – Create the Knowledge canvas App
--------------------------------------------

In this exercise, you will be creating the Fabrikam Knowledge canvas app. We will build out the detailed user experience in
the upcoming canvas app module.

### Task 1 – Create a canvas app

1.  Go back to <https://make.powerapps.com> and make sure you are in your
    **Practice** environment.

2.  Select **Solutions** and open **Common Data Services Default Solution**.

3.  Click **New \> App \> Canvas App \> **Tablet Form Factor**.

4.  Click **Skip** if you see a prompt before the designer loads.

5.  The Canvas App Designer will load. Hover over **Screen1** and click on the
    **…** button.

6.  Select **Rename**.

7.  Enter **mainScreen** and press the enter key. *Note:* It is important to name all app elements exactly as provided as we will reference these names using script in later modules. It is always a good idea to give components meaningful names as it makes them easier to use as your application gets more complex.

### Task 2 – Add Header to the App
Part of making a good app is giving it a personality. We are going to keep
things simple here and just add a basic header to the app.

1.  Select the **Insert** tab at the top of the screen.

2.  Click **Label** to add a text label to your cavas.

3.  Select the label.

4.  Rename the label **headerLabel** by clicking the **...** button in the **Tree View** pane.

5.  Customize your label using the **Properties** pane or the **Function** editor located above your canvas. Change the **Font size** to **28**.

7.  Set **Color** to **White**. *Note:* You can select a color by clicking a swatch in the **Properties** pane, or by using Function editor. First select **Color** from the dropdown to the left of the **FX** button, then  use the function editor to enter the name of the color, **White**, or the RGBA value of the color, **RGBA(255,255,255,1).

8.  The label text is now the same color as the canvas. Use the function editor to set the **Fill** value to **Blue**.

8.  Click **Text Alignment** and select **Center**.

10. Locate the **Position** section on the Properties window.

11. Enter **0** for **Y** and **0** for **X**.

12. Locate the **Size** section.

13. Enter **1365** for **Width** and **60** for **Height**.

14. Double click on the **Text** of the label to edit the text label on the canvas. Type **Fabrikam Assessment**.

15. View the **Text** value on the **Properties** pane and notice that it has been updated to **Fabrikam Assessment**.

### Task 3 – Add User Name to the Header

In this task, you are going to leverage the User() information to add the name
of the current user to the header.

1.  In the **Tree View** pane, select **MainScreen**.

2.  Select the **Insert** tab from the top menu and click **Label**.

3.  Rename the label **userLabel**.

4.  Use the function editor to set the **Text** value to 

            User().FullName

5.  Set the **Font Size** of the userLabel to **14**.

6.  Set the Font **Color** to **White**.

7.  Using the Function editor, set **Align** to **Right**.

8.  Set **Text alignment** to **Align right**.

9.  Set **Position X** to **1215** and **Position Y** to **0**.

10. Locate **Size** and set the Height to **60**.

11. Locate **Padding** and enter **10** for **Right**.

12. On the **Tree View** pane, review the items in the **mainScreen**. The canvas app uses layers. Select **headerLabel** and click the **...** button. Select **Reorder \> Bring to front**. Notice that the userLabel is now hidden behind the headerLabel. Undo your change. The userLabel is now visible again.

13. Click **File** and then **Save** to save your canvas app.

14. Select **Cloud** and enter **Fabrikam Assessment** for **Name**.

15. Click **Save**.

16. Click on the Power Apps **Back** button.

17. Click **Play**.

18. Your application will load.

19. Close the preview.

20. Close the Canvas App Designer.

21. Click **Done**.
