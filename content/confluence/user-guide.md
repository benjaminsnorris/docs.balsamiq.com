---
date: 2015-07-30T15:52:20-07:00
draft: false
title: "Mockups for Confluence User Guide"
menu:
  menuconfluence:
    parent: confluence
weight: 10
---

## Welcome 

This page contains usage instructions for [Mockups for Confluence](https://marketplace.atlassian.com/plugins/com.balsamiq.confluence.plugins.mockups/cloud/overview).

Confluence Server Administrators: the **[Mockups for Confluence Server Admin Guide](/confluence/admin-guide/)** is for you.

Confluence Cloud Administrators: the **[Mockups for Confluence Cloud Admin Guide](/confluence/admin-guide-cloud/)** is for you.

* * *

## Creating a New Mockup

Adding a mockup to a wiki page is very similar to adding an image.

Edit the page, position the cursor where you'd like your mockup to be, then click on the Insert menu and select "UI Mockup" from the list.

![](//media.balsamiq.com/img/support/docs/confluence/userguide/confluence1.png)

This will take you directly to the Balsamiq Mockup editor, where you can create your mockup (or import an existing mockup - see [this page](https://support.balsamiq.com/plugins/importtoatlassian/) for instructions).

If you have never used Balsamiq Mockups before, here's a little intro of what you can do with it when using the Confluence plugin:

<div class="video"><iframe allowfullscreen="" frameborder="0" src="//www.youtube.com/embed/l9-dLyINrac?rel=0"></iframe></div>

Once you are happy with your mockup, just select "Save" from the toolbar or the Mockup menu. You will be asked to give it a unique name. This is required and allows you to include more than one mockup on the same page.

![](//media.balsamiq.com/img/support/docs/confluence/userguide/m4csavenew.png)

Once you name your mockup you can continue working on it and saving it periodically.

When you are ready to go back to the wiki page, just click on "Close" or select "Close Editor" from the Mockup menu. You will be taken back to the Confluence editor. Save the page and you're done!

{{% alert info %}}**Note:** Even if your Balsamiq Mockups license is configured so that only specific people can create and edit mockups (explained in the [Admin Guide](/confluence/admin-guide)), anyone with access to your Confluence site will be able to see them.{{% /alert %}}

{{% alert info %}}**A note for Confluence 3.x users:** In Confluence 3.x, you have to add a mockup by selecting the "Add UI Mockup" menu under the "Add Content" menu section of your wiki page.{{% /alert %}}

## Editing a Mockup

To make changes to a mockup, edit the wiki page, select the mockup image and click on the "Edit" button in the little macro control panel that shows up.

![](//media.balsamiq.com/img/support/docs/confluence/userguide/confluence2.png)

{{% alert info %}}**A note for Confluence 3.x users:** In Confluence 3.x, you edit a mockup by clicking on the "edit this mockup" link under the mockup you want to edit.{{% /alert %}}

* * *

## Linking Mockups Together 

Much like the Desktop and Web versions of Mockups, you can create links between mockups by using the Link property in the Property Inspector (for controls that support linking; read [this article](https://support.balsamiq.com/tutorials/hotareas/) for controls that don't).

![](//media.balsamiq.com/img/support/docs/m4d/link_inspector.png)

You can link to other mockups or to web addresses. Once a link has been added the arrow in the lower-right corner will indicate what kind of link it is. Links to mockups will show as a plain arrow, while links to web pages will show as an arrow with a box around it.

![](//media.balsamiq.com/img/support/docs/m4d/button_link.png)

To navigate to other mockups that have been linked, go to Full Screen Presentation mode (View > Full Screen Presentation) in the Mockups Editor, or click on the linked control on the mockup image while viewing the page in Confluence.

* * *

## Deleting a Mockup

To remove a mockup from a page, simply edit the page, select the mockup and delete it or click on "Remove".

* * *

## Looking at a Mockup's History

Each UI mockup is saved as two separate attachments, one for the PNG image and one for the BMML source data. Confluence supports versioning of attachments, and Balsamiq Mockups takes advantage of it so that you can see how your mockup evolved over time, or roll back to a previous version.

![](//media.balsamiq.com/img/support/docs/confluence/userguide/m4chistory.png)​

* * *

## Rolling Back to a Previous Version of a Mockup

This is a bit tricky but it can be done. Go to the attachments view for your page, find the mockup you want to roll back, get the BMML for the version you want to roll it back to and copy it. Now you can go back to the page, edit the mockup and import your old BMML via the "Import" dialog.

* * *

## Moving a Mockup on a Page

To move a mockup to a different location on a page you edit the page, select it in the editor and use cut and paste to move it to another location on the page. Save the page and you're done!

* * *

## Aligning a Mockup on a Page

If you'd like to left-align or right-align the mockup's image relative to your page, you can do so via the macro control panel. Note that the macro won't align while in edit mode, but it will show up with the right alignment once you save the wiki page.

* * *

## Specifying the Size of a Mockup on a Page

You can use the "Small", "Medium" and "Original" buttons in the macro property panel.

* * *

## Adding an Existing Confluence Mockup to a New Confluence Page

You may want to add a mockup that you've already created in Confluence to a different page than you initially created it for. Right now you can only add mockups that are attached to the same page. However, you can create a copy of the mockup you want and add it to the new page. The fastest way to do that is via [export / import, as described here.](https://support.balsamiq.com/plugins/importtoatlassian/). This process involves exporting from the old one and importing into a new one. You can also see the steps [below](#moving-a-mockup-from-one-page-to-another) for moving a mockup from one page to another.

* * *

## Moving a Mockup from One Page to Another

It is possible to move mockups from one page to another. However, this is somewhat of an "advanced" feature, so it's not as easy as the tasks described above.

Here are the steps:

1.  Go to the Attachments page and move _both_ the .bmml and .png files (both file types should have a "mockup\_" prefix) to the page you wish to move the mockup to (_see [this page](https://confluence.atlassian.com/display/DOC/Moving+an+Attachment) for Confluence documentation on moving attachments_).
2.  On the new page, Edit the page and type the following text:
    1.  **{mockup:Name=**
    2.  *the name of the mockup without the "mockup\_" prefix or the .bmml extension (so "mockup\_login screen.bmml" would become "**login screen**")*
    3.  **}**  
    resulting in something like this **{mockup:Name=login screen}**.
3.  After doing this, you should see your mockup appear in the editor.

This process can also be useful if you have removed a mockup from a page and want to re-add it. In that case, skip step 1 and follow steps 2-4.

* * *

## Renaming a Mockup

Similar to the process described above, renaming a mockup is possible, but you have to go behind the scenes to do it.

Here are the steps:

1.  Go to the Attachments page and rename _both_ the .bmml and .png files (click on Properties and change the file name). Make sure to keep the "mockup\_" prefix for both files.
2.  Go back to the page the mockup was on (you should see an error where it used to be).
3.  Edit the page, then delete the macro placeholder for the old mockup name.
4.  In its place, type the following text:
    1.  **{mockup:Name=**
    2.  *the name of the renamed mockup without the "mockup\_" prefix or the .bmml extension (so "mockup\_new name.bmml" would become "**new name**")*
    3.  **}**  
    resulting in something like this **{mockup:Name=new name}**.
5.  After doing this, you should see your mockup appear in the editor.