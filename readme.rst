##########################
BCIT... Course Hub Website
##########################

This is a course hub webapp that would suit BCIT courses.
It is currently used for 
`COMP47111 Introduction to Internet Software Development 
<http://www.bcit.ca/study/outlines/20171047992>`_.

*****
Setup
*****

Extract or clone the project into a subfolder inside
your public html files, & serve the app from its **public** folder.

The site is XML-driven, abstracting as much as possible so that the
webapp can be used for other courses. XML was chosen over an RDB
because of the rich data structures it can support.

Basically, course material used to generate pages is put into an
appropriate subfolder inside /data, while images that are part
of the resulting pages would go underneath /public, for instance
inside /public/pix.

There are a few course metadata files directly inside /data, and
then subfolders for some common kinds of content.

What the end-user experiences is managed through the organizer.xml
document.

Currently supported content formats include XML (to suit the S5
presentation framework) or MD (markdown).

Refer to the `COMP47111 course hub <https://github.com/jedi-academy/learn-4711>`_,
which is live at http://comp4711.jlparry.com/, for a more complete example.

************
Contributing
************

Contribute to this project by makeing a pull request to the develop branch.

***************
Project Folders
***************

/application	The course hub engine
/data           XML & markdown content for learning activities
/public         public-facing website
/system		CodeIgniter 3.1.x framework
/xml            DTDs that cab be used to validate XML content

*******
License
*******

MIT license.

***************
Acknowledgement
***************

This webapp was written by `James Parry <mailto:jim_parry@bcit.ca>`_, Instructor in Computer Systems
Technology at the British Columbia Institute of Technology,
and Project Lead for CodeIgniter.

The Parsedown library comes from https://github.com/erusev/parsedown, and has an MIT license.

CodeIgniter is a project of B.C.I.T.