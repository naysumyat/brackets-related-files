brackets-related-files
========================

"Related Files" for Brackets.  This extension scans files when they are opened/added to the working set and builds
a list of related files in the project.  You can fold down the related files via a discloser to the right of 
working set files and can open the related files from there.

The list of related files is determined by searching a document for relative paths to each of the files in a project.
A few tweaks are in place so that it can find requires in JavaScript.

Install
-----------
Copy (or git clone) this folder into the `brackets/src/extensions/user` folder and restart Brackets.
Mouse over a file you've opened in the working set and you will see a discloser to the right of the file.
Use the discloser to reveal related file and click on one to open it.

! WARNING !
-----------
The extension is designed to run in the background, with the current master branch of Brackets it runs
in a blocking manner.  It works better on large projects with pull request #1009 (Async.doSequentiallyInBackground support).
