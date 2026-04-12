Mechanical Movements extraction dataset

Source PDF: Mechanical_Movements_507.pdf
Pages processed: 138
OCR text files: 138
Diagram snapshots: 522

Contents
- ocr_pages/: one UTF-8 TXT file per page
- page_images/: rendered page JPEGs at 120 dpi
- diagram_snapshots/: automatically cropped diagram regions
- manifest.json: page + snapshot metadata
- diagram_manifest.csv: flat snapshot table

Notes
- This is a first-pass automatic extraction.
- Snapshot count is 522, which is above the book's nominal 507 mechanisms.
- The reason is over-segmentation on some pages with irregular layouts or tall cells.
- Bounding boxes are in rendered-image pixels, referenced to page_images/.
- OCR is page-level and best-effort; some scanned pages remain noisy.
