# DOCX to PDF Quick Actions

If you are on macOS and want to generate a PDF from a DOCX file, you generally have to go through Word, LibreOffice, or Pages, using the Print or Export functions found under the File menu. It's slow, especially if you have multiple files. Ideally, you'd be able to simply select the file(s) in Finder, secondary-click, and run the operation right there.

Now you can!

Just [download the version(s) of your choice](https://github.com/IsaacWeiss/docx-to-pdf-quick-actions/releases/latest) and double-click to add this utility your context menu.

## AppleScript via Microsoft Word, LibreOffice, and Apple Pages
The user-visible behavior (see screenshot below) is identical for all three versions. So, why did I go to three times the trouble and recreate the same program with essentially three different script libraries?
* Each of the three word processors does slightly different rendering, especially with complex documents containing elements other than text (and your particular file[s] may have been created with LibreOffice or Pages instead of Word).
* Your particular computer may not have one or more of these programs installed (Office 365 is only available to me on my work laptop).
* Having multiple tools helps to overcome any limitations that may become apparent (see below).

## Usage Screenshot
![screenshot](https://github.com/user-attachments/assets/39509529-417f-4ba0-99a7-8dd4ef923fe6)

## Known Limitations
* Each Quick Action only works if the software it calls on is installed. If you don't have LibreOffice, you should ~~not try to use "Convert DOCX to PDF via LibreOffice"~~ install LibreOffice from www.libreoffice.org.
* For reasons I cannot begin to guess at, the Word one will only work *once* on a file stored in remote storage, such as Dropbox or OneDrive... and then it throws an error when trying to operate on the same *or any other file* in the given drive, *for all time.* So use that one shot wisely.
* Pages is likely to produce the worst rendering, just because Apple wasn't too careful with writing the DOCX import filters. However, it's also the only one that comes pre-installed on all Macs, so it's my pleasure to provide it just in case you need it.

## Feedback
Please let me know if you find this useful by leaving a quick comment [here](https://github.com/IsaacWeiss/docx-to-pdf-quick-actions/discussions/1). I would be truly grateful.
