# Event Table Edit
Event Table Edit (abbrev. ETE) is a free and open source table plugin for Joomla 2.5, 3.x and above (original author: Manuel Kaspar, continuation: Matthias Gruhn). With the plugin, you can create a responsive, editable table with CSV import and export function and XML export/import for table settings. It also has a full rights management (Joomla ACL). 
You can  transform the table into an appointment booking system with confirmation emails for users and the admin, including iCal calendar files for both in the attachment. As it is based on a CSS-template, the layout of the table can be changed easily. The responsive function is based on the "Column Toggle Table with Mini Map" from the tablesaw plugins (https://github.com/filamentgroup/tablesaw).

Download latest version 4.5.3 (since 12.04.2017): https://github.com/Theophilix/event-table-edit/archive/master.zip

Demo site for backend and frontend (includes appointment table): http://demo.eventtableedit.com 

## I Features:

- Editable table (insert pictures, BBCode...)
- Sorting options (A-Z, Z-A, natural sorting is used)
- Choice of layout mode (stack, swipe, toggle) for enhanced responsiveness
- Multiple appointment booking function with confirmation email and ICAL calendar (.ics file) attachment
- Complete rights management (Joomla ACL: add/delete rows, edit cells, rearrange rows, administer table from frontend)
- Multilingual (currently available: DE, EN)
- CSV and TXT import with different formats (text, date, time, integer, float, boolean, link, mail) 
  and import settings (separator, values in quotes or not)
- CSV Export
- XML import and export: import and export a table with all settings
- Own CSS based template

Frontend view options:
- Sort columns (setting in rights management)
- Delete rows (setting in rights management)
- Add rows (setting in rights management)
- Filter rows
- Pagination
- Print view
- Administer table (setting in rights management)

Backend options:

a) General
- Normal or appointment booking function
- Options for appointment booking function:
  + ICAL / .ics-File options (location, subject, name of file)
  + Set admin email address and email display name
  + Confirmation email settings (chose subject and message text with appointment-date and -time-variables)
  + CSV Import and Export
  + Show or hide user names to user or admin
- Show or hide table title
- Usertext before and after table
- Show or hide column to delete or sort rows
- Use Metadata
- Enhanced SEO
- Support BB-Code

b) Layout / Style

Choose or select:
- Date format
- Time format
- Float separator ("," or ".")
- Cell spacing
- Cell padding
- Colors of alternating rows
- Maximum length of cell content
- Display table in the same, or a new window

Please post all feature requests in the issues tab.


## II Version history

For version 4.5.3:

[2] Appointment mode
- enhancement: https://github.com/Theophilix/event-table-edit/issues/42: Frontend / Appointment function: Allow multiple bookings for the same day and time
- enhancement: new options in backend: "show username to admin" and  "show username to user".
- enhancement: admin can insert several usernames separated by ENTER key.
- bugfix: print view now shows exactly what user sees

[3] Universal changes
- bugfix / enhancement: xml download: proposed filename is table name



For version 4.5.2:

[1] Normal mode
- bugfix: layout mode change when using pagination https://github.com/Theophilix/event-table-edit/issues/30

[3] Universal changes
- bugfix / enhancement: xml import error and version handling

For version 4.5.1:

[1] Normal mode
- bugfix: uploaded wrong stringparser file -> bbcode works now
- bugfix: “deprecated” warnings in development debug mode

[2] Appointment mode
- enhancement: https://github.com/Theophilix/event-table-edit/issues/41: Frontend / Appointment table: admins can edit table values directly (change free -> reserved and vice versa) when logged in to frontend.


For version 4.5:

[1] Normal mode
- enhancement: natural sorting, not perfect yet, but work on it will continue
- bugfix: BBCode is working now
- bugfix: php 7.1 modulo by zero
- bugfix: 800px width (deleting column disappeared)
- bugfix: sort date problem when deleting content of date cell
- bugfix: dropdown fields error
- bugfix: filter problem:  a) Umlaut ä/ö/ü + b) filter not working with enter key + c) value does not stay in filter input form after clicking on “show” -> now, 2 input fields
- bugfix: firefox browser asks to refresh page after editing cells

[2] Appointment mode
- bugfix: admin doesn’t get email (was problem with „/“) + email does not show multiple appointments (example:  you have an appointment on 05.03.2017 / 06.03.2017 at 17:20 / 17:40)


For version 4.4.3:

[1] Normal mode
- bug removed: https://github.com/Theophilix/event-table-edit/issues/27: Locale not recognized (in date format) (?)
- bug removed: https://github.com/Theophilix/event-table-edit/issues/39: When adding a new row, refreshing page is necessary before editing cell.
- Joomla update notification and update via Joomla administrator backend enabled. 


For version 4.4.2:

[1] Normal mode
- bug removed: https://github.com/Theophilix/event-table-edit/issues/31: Sorting row column disappears in toggle view

For version 4.4.1:

[1] Normal mode
- bug removed: https://github.com/Theophilix/event-table-edit/issues/28: Sorting by date field results in an error if date field is empty

[3] Universal changes
- english corrections: https://github.com/Theophilix/event-table-edit/pull/29 -> Thank you, user "brianteeman"!

For version 4.4:

[1] Normal mode
- bug removed: when importing empty cells from csv-file, cell value changed to "free". Solution: select box "csv is appointment-table".

[2] Appointment mode
- bug removed: ICS files are deleted now

[3] Universal changes
- minor spellings errors corrected
- xml import/export: now xml-files are scanned for ETE-signature
- plugin update notification and update function via Joomla backend reactivated

For version 4.3:

[1] Normal mode
- XML import and export function: export and import a table with all settings.
- file download option for csv export
- additional delete and sort row function renamed. It is called "Additional row sorting and deleting column"(ger:"Zusatzspalte zur Umsortierung und Löschung der Tabellenzeilen")

[2] Appointment mode
- no changes

For version 4.2:

[1] Normal mode
- Column sorting (via header click or selection menu) option added (unfortunately, natural sorting is still not working)
- Table administrate view bug is fixed
- Choice of layout mode (stack, swipe, toggle)-option added
- Backend overview improved

[2] Appointment mode
- Selection of multiple appointments added. Users have to click a button after selecting dates/times.
- Time limit option (cells are marked as "blocked") added
- "Add weekdays to header" option added
- Layout improvements in frontend and backend


