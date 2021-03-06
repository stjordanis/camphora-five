## Creating your first app

**Notice**, the following app, or one similar to it, should already exist as a _"template example app"_.
If you still want to follow this tutorial, and create this app exactly as illustrated here - Then simply
delete the example app called _"address-book"_ from your list of apps.

[Open up Camphora Five](/camphora-five) and click the _"+"_ button, at the top right corner of your page.
Then name your app `address-book`. Notice, you cannot use spaces or capital letters in your app's name.
Then add some fields to your app, by clicking the _"+"_ in the area of your screen where it says _"fields"_.
You can create any fields you want to create, such as for instance.

* name - _"Singleline text"_ type
* address - _"Multiline text"_ type
* sex - _"Radiobuttons"_ type

If you choose _"Radiobuttons"_ or _"Select dropdown"_ as your field type however, you'll need to make sure
you supply the legal options for these fields, as a comma separated list of values. After you are done, your
screen should resemble the following.

https://phosphorusfive.files.wordpress.com/2018/05/camphora-five-create-address-boo-screenshot.png

Then simply click the _"power cord"_ button, next to the _"Floppy disc save"_ button. This will both save your app,
and generate it, at which point you can immediately start using your app. If you now go back to your desktop,
by clicking the home button, you'll see an icon for you app, resembling the following. If you want to,
you can change your app's desktop icon - However, we'll have a look at this later.

https://phosphorusfive.files.wordpress.com/2018/05/camphora-five-desktop-screenshot-new.png

If you open your app, and add some records to it, it'll end up resembling the following.

https://phosphorusfive.files.wordpress.com/2018/05/using-camphora-five-address-book-screenshot.png

**Notice**, already you can filter and sort your items - Both ascending and descending, by clicking
the column header once to sort ascencing, or twice to sort in reverse order. To filter, simply type
some piece of text into the _"search textbox"_ at the top, and click the spyglass.

### Settings for your app

The name of your app, also becomes the name of your database table, in addition to your app's URL. If you named
your app _"address-book"_ for instance, then its URL will be [/address-book](/address-book). This might be
important to remember for you, especially if you choose to not create a desktop icon for your app, since
then there will be no explicit desktop icon created for your app, and the only method you have to actually
open your app, is by remembering its URL.

You can also choose to explicitly hide a specific column from the datagrid view of your app, by checking
off the _"Show"_ checkbox on your columns. The data and column will still exist in your database, and you
can change and read its value when you edit a specific item - However, the data will not be visible in your
main _"datagrid"_ view. If we for instance choose to hide the _"address"_ field, then your app will end
up looking like the following.

https://phosphorusfive.files.wordpress.com/2018/05/camphora-five-hidden-column-screenshot.png

As you can see in the above screenshot, the _"address"_ field is no longer visible in the main _"datagrid"_ view,
but still possible to edit when having chosen to edit a specific item. This allows you to create a CRUD app with
dozens of columns, but still only display the most important columns in your _"datagrid"_ view.

### Editing your app

You can also edit your app, without generating it, and save your edits for later, still without generating your
app. If you wish to do this, you can save your app in the meantime by clicking the save button. This will save
your app's _"declaration"_, without generating it. You can also clone an existing app. This might be useful if you have a complex app, with lots of _"Views"_, and
you'll need to copy your app for some reasons.

Your app declarations are actually simply Hyperlambda files, which you can find in your user's home folder. However,
be careful if you edit these files manually, since if the the file's content becomes invalid, you can no longer generate
your app.

### Responsive CRUD apps

In general, your CRUD apps will be _"responsive"_. This implies that they'll also perfectly work on your
smart phone, tablet, and other types of devices capable of rendering HTML. However, since a phone typically
doesn't have the same resolution as a computer system, this might have consequences for the number of columns
that will be shown while you use a Camphora Five app on your phone or tablet. On a device with very small
resolution, only the first column will be visible, since otherwise the app would be almost impossible to use.
On larger devices, more and more columns are incrementally shown. You can also explicitly declare to some
extent which fields from your app you want to show in the datagrid view of your app.

Due to the above, it might be smart to make sure your most important fields are the first fields of your app.
