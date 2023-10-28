# fram_plain
This style is derived from amsplain (American Mathematical Society).

A copy of the original style can be found in the "unmodified copies" folder, which is subjected to the licence https://www.latex-project.org/lppl.txt.
If you wish to distribute a work derived from the original *amsplain* or the derived *fram_plain*, please refer to the aforementioned documentation.

List of changes in the derived work:
 - The entry 'doi' is added;
 - A function 'output.nonempty.doi' is added.
 - In the function 'fin.entry', the note is printed, the mr is now ignored, and the new 'output.nonempty.doi' is executed.
 - The 'note output' line is removed from all entry-type named functions (see previous point). This might change the note position for 'incollection', 'inproceedings', 'masterthesis', 'misc', 'phdthesis', and 'unpublished'.
 - Function 'format.names': now abbreviates first names to initials, and does not put a comma before the last name.
 - Function 'format.authors': now always repeats the authors, never uses the horizontal line.
 - A function 'format.title.book' is added. It puts on the stack the content of the variable 'title', with no case changed, enclosed between double quotes.
 - Function 'format.crossref.editor': first names are now abbreviated to initials.
 - Function 'article': does not print the number anymore.
 - Functions 'book', 'booklet', 'inbook', 'manual', 'masterthesis', 'phdthesis', 'proceedings': use format.title.book instead of format.title.
 - Function 'unpublished': now uses 'output' instead of 'output.check' when printing 'note'.
 - Function 'format.nonauthor.editors': now places "ed." or "eds." in parenthesis.
 - Functions 'format.inproc.title.address.editors' and 'format.incoll.title.editors': now do not enclose editors in patenthesis, and put the booktitle between "in: ``" and "''".
 
