Scripts that are designed to extract text from pdfs and map them to fields
defined by rectangles and limited by font


The current incantation like this

 perl uncompressed-to-text-with-locations 1709508-uncompressed.pdf
 | ./add_form_id - |  ./map-locations-to-fields  - | ./coalesce-fragments -
