Scripts that are designed to extract text from pdfs and map them to fields
defined by rectangles and limited by font

The current incantation like this

# uncompress-pdf 1709508-uncompressed.pdf | \

podofouncompress 1709508.pdf
cat 1709508-uncompressed.pdf | \
   ./uncompressed-to-text-with-locations - | \
   ./add_form_id - |  \
   ./map-locations-to-fields  - |  \
   ./coalesce-fragments -
