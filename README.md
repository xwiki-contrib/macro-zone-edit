Zone Edit
========

The zone macro lets you insert an editable section, that stores the content into another document.
The section displays a little pencil (both in view and inline mode) in the top right corner for the users that have edit rights, which if clicked redirects you to the inline mode of the document storing the content and lets you modify the title, content and a "Read more" link.
This was tested on XWiki 5.4.4, 6.4.x., and 7.4

Usage
=====

Insert the following macro on the page you want the editable section.

{{zone document="Space.Name" /}}

The document given as parameter must exist.
You can add a ZoneCode.ZoneClass object and add some content in there.
If the document does not have the object already, it will be added automatically and you will be able to edit after a refresh of the document from which you called the macro.

When editing a zone you have the posibility to edit:

* The title of the section
* The content of the section
* And the Read more link 

If you insert a link in the link section, a "Read more" button will appear.

If you decide to write the velocity code in the included document, then it's worth mentioning that the context will be that of the included document and not that of the document calling the macro.
