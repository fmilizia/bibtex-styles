# fram_plain
This style is derived from amsplain (American Mathematical Society).

The original style, which can be found in the "unmodified copies" folder, is distributed under the licence https://www.latex-project.org/lppl.txt.
Anyone wishing to distribute this or other derived works must comply with that licence.

List of changes in the derived work:
 - The entry 'doi' is added;
 - The entry 'location' is added; it is meant to be the place where a conference has been held, for 'inproceedings' entry-types. 'address' always refers to the place of publication, shown after the publisher.
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
 - Function 'format.incoll.inproc.crossref': the booktitle is now between double quotes, not emphasized.
