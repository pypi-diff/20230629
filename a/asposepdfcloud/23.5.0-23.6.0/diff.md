# Comparing `tmp/asposepdfcloud-23.5.0.tar.gz` & `tmp/asposepdfcloud-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asposepdfcloud-23.5.0.tar", last modified: Wed May 24 08:32:50 2023, max compression
+gzip compressed data, was "asposepdfcloud-23.6.0.tar", last modified: Thu Jun 29 11:22:36 2023, max compression
```

## Comparing `asposepdfcloud-23.5.0.tar` & `asposepdfcloud-23.6.0.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 08:32:50.943620 asposepdfcloud-23.5.0/
-drwxrwxrwx   0        0        0        0 2023-05-24 08:32:42.824341 asposepdfcloud-23.5.0/Examples/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/__init__.py
--rw-rw-rw-   0        0        0      464 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/configuration.py
--rw-rw-rw-   0        0        0      347 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/delete_all_annotations.py
--rw-rw-rw-   0        0        0      187 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/delete_document_annotations.py
--rw-rw-rw-   0        0        0      217 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/delete_page_annotations.py
--rw-rw-rw-   0        0        0      368 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_carret_annotations.py
--rw-rw-rw-   0        0        0      370 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_circle_annotation.py
--rw-rw-rw-   0        0        0      119 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_annotatios.py
--rw-rw-rw-   0        0        0      220 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_attachment.py
--rw-rw-rw-   0        0        0      274 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_attachment_by_index.py
--rw-rw-rw-   0        0        0      283 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_bookamarks.py
--rw-rw-rw-   0        0        0      212 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_bookmars.py
--rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_carret_annotation.py
--rw-rw-rw-   0        0        0      197 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_circle_annotations.py
--rw-rw-rw-   0        0        0      206 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_file_annotations.py
--rw-rw-rw-   0        0        0      206 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_free_text_annotations.py
--rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_highlight_annotations.py
--rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_ink_annotations.py
--rw-rw-rw-   0        0        0      193 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_line_annotations.py
--rw-rw-rw-   0        0        0      201 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_movie_annotations.py
--rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_polygon_annotations.py
--rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_polyline_annotations.py
--rw-rw-rw-   0        0        0      270 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_popup_annotation_parent.py
--rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_redaction_annotation.py
--rw-rw-rw-   0        0        0      211 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_screen_annotations.py
--rw-rw-rw-   0        0        0      201 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_sqiuggly_annotation.py
--rw-rw-rw-   0        0        0      201 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_square_annotations.py
--rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_storage_pdf.py
--rw-rw-rw-   0        0        0      205 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_strikeout_annotation.py
--rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_document_underline_annotations.py
--rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_doucment_popup_annotations.py
--rw-rw-rw-   0        0        0      195 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_doument_annotations.py
--rw-rw-rw-   0        0        0      192 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_doument_sound_annotations.py
--rw-rw-rw-   0        0        0      369 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_file_attachment_annotations.py
--rw-rw-rw-   0        0        0      393 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_file_attachment_annotations_data.py
--rw-rw-rw-   0        0        0      378 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_free_text_annotation.py
--rw-rw-rw-   0        0        0      376 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_hightlight_annotation.py
--rw-rw-rw-   0        0        0      341 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_html_storage_pdf.py
--rw-rw-rw-   0        0        0      364 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_ink_annotations.py
--rw-rw-rw-   0        0        0      368 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_line_annotation.py
--rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_mht_storage_pdf.py
--rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_movie_annotation.py
--rw-rw-rw-   0        0        0      214 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_annotations.py
--rw-rw-rw-   0        0        0      228 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_carret_annotations.py
--rw-rw-rw-   0        0        0      229 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_cirlce_annotations.py
--rw-rw-rw-   0        0        0      233 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_file_attachment_annotations.py
--rw-rw-rw-   0        0        0      234 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_free_text_annotations.py
--rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_highlight_annotations.py
--rw-rw-rw-   0        0        0      226 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_ink_annotations.py
--rw-rw-rw-   0        0        0      227 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_line_annotations.py
--rw-rw-rw-   0        0        0      231 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_movie_annotations.py
--rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_polygon_annotations.py
--rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_polyline_annotations.py
--rw-rw-rw-   0        0        0      228 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_popup_annotations.py
--rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_redaction_annotation.py
--rw-rw-rw-   0        0        0      235 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_screen_annotations.py
--rw-rw-rw-   0        0        0      228 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_sound_annotations.py
--rw-rw-rw-   0        0        0      227 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_square_annotations.py
--rw-rw-rw-   0        0        0      225 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_squiggly_annotations.py
--rw-rw-rw-   0        0        0      230 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_stamp_annotations.py
--rw-rw-rw-   0        0        0      233 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_strikeout_annotations.py
--rw-rw-rw-   0        0        0      227 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_text_annotations.py
--rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_page_underline_annotations.py
--rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pcl_storage.py
--rw-rw-rw-   0        0        0      206 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_epub.py
--rw-rw-rw-   0        0        0      208 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_html.py
--rw-rw-rw-   0        0        0      217 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_latext.py
--rw-rw-rw-   0        0        0      210 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_mobi_xml.py
--rw-rw-rw-   0        0        0      254 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_pdfa.py
--rw-rw-rw-   0        0        0      208 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_pptx.py
--rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_svg.py
--rw-rw-rw-   0        0        0      208 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_tiff.py
--rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_xls.py
--rw-rw-rw-   0        0        0      209 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_xml.py
--rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_pdf_storage_xvg.py
--rw-rw-rw-   0        0        0      374 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_polygon_annotation.py
--rw-rw-rw-   0        0        0      374 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_polyline_annotation.py
--rw-rw-rw-   0        0        0      376 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_redaction_annotation.py
--rw-rw-rw-   0        0        0      376 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_screen_annotation.py
--rw-rw-rw-   0        0        0      370 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_sound_annotation.py
--rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_sound_annotation_data.py
--rw-rw-rw-   0        0        0      370 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_square_annotation.py
--rw-rw-rw-   0        0        0      374 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_squiggly_annotation.py
--rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_stamp_annotations_data.py
--rw-rw-rw-   0        0        0      378 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_strikeout_annotation.py
--rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_svg_storage.py
--rw-rw-rw-   0        0        0      368 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_text_annotation.py
--rw-rw-rw-   0        0        0      372 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_underline_annotations.py
--rw-rw-rw-   0        0        0      375 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_underline_annottion.py
--rw-rw-rw-   0        0        0      128 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_web_storage.py
--rw-rw-rw-   0        0        0      225 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_xfa_pdf_storage_acro.py
--rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_xml_storage_pdf.py
--rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_xps_storage_pdf.py
--rw-rw-rw-   0        0        0      209 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/get_xslfo_storage.py
--rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_append_document.py
--rw-rw-rw-   0        0        0      444 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_append_document_body_params.py
--rw-rw-rw-   0        0        0     1066 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_ink_annotations.py
--rw-rw-rw-   0        0        0      833 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_carret_annotations.py
--rw-rw-rw-   0        0        0      676 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_circle_annotations.py
--rw-rw-rw-   0        0        0      928 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_file_attachment_annotations.py
--rw-rw-rw-   0        0        0     1263 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_free_annotations.py
--rw-rw-rw-   0        0        0      948 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_highlight_annotations.py
--rw-rw-rw-   0        0        0      783 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_line_annotations.py
--rw-rw-rw-   0        0        0      775 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_movie_annotations.py
--rw-rw-rw-   0        0        0      894 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_polygon_annotations.py
--rw-rw-rw-   0        0        0      894 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_polyline_annotations.py
--rw-rw-rw-   0        0        0      774 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_redaction_annotations.py
--rw-rw-rw-   0        0        0      817 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_screen_annotations.py
--rw-rw-rw-   0        0        0      869 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_sound_annotations.py
--rw-rw-rw-   0        0        0      702 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_square_annotations.py
--rw-rw-rw-   0        0        0      946 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_squiggly_annotations.py
--rw-rw-rw-   0        0        0      867 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_stamp_annotations.py
--rw-rw-rw-   0        0        0      947 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_strikeout_annotations.py
--rw-rw-rw-   0        0        0      773 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_text_annotations.py
--rw-rw-rw-   0        0        0      944 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_page_underline_annotations.py
--rw-rw-rw-   0        0        0      667 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/post_popup_annotations.py
--rw-rw-rw-   0        0        0      997 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_carret_annotations.py
--rw-rw-rw-   0        0        0      862 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_circle_annotation.py
--rw-rw-rw-   0        0        0      284 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_df_storage_xls.py
--rw-rw-rw-   0        0        0      301 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_epub_storage_pdf.py
--rw-rw-rw-   0        0        0      383 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_file_attachement_annotations.py
--rw-rw-rw-   0        0        0     1071 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_file_attachment_annotations.py
--rw-rw-rw-   0        0        0     1403 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_free_text_annotation.py
--rw-rw-rw-   0        0        0     1115 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_hightlight_annotation.py
--rw-rw-rw-   0        0        0      425 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_html_storage_pdf.py
--rw-rw-rw-   0        0        0     1249 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_ink_annotations.py
--rw-rw-rw-   0        0        0      942 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_line_annotation.py
--rw-rw-rw-   0        0        0      300 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_mht_storage_pdf.py
--rw-rw-rw-   0        0        0      912 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_movie_annotation.py
--rw-rw-rw-   0        0        0      300 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pcl_storage_pdf.py
--rw-rw-rw-   0        0        0      265 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_epub.py
--rw-rw-rw-   0        0        0      264 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_html.py
--rw-rw-rw-   0        0        0      255 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_latext.py
--rw-rw-rw-   0        0        0      267 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_mobi_xml.py
--rw-rw-rw-   0        0        0      314 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_pdfa.py
--rw-rw-rw-   0        0        0      265 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_pptx.py
--rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_svg.py
--rw-rw-rw-   0        0        0      267 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_tiff.py
--rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_to_doc.py
--rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_xls.py
--rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_xml.py
--rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_request_xps.py
--rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_epub.py
--rw-rw-rw-   0        0        0      285 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_html.py
--rw-rw-rw-   0        0        0      290 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_latext.py
--rw-rw-rw-   0        0        0      290 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_mobi_xml.py
--rw-rw-rw-   0        0        0      282 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_pdf.py
--rw-rw-rw-   0        0        0      338 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_pdfa.py
--rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_pptx.py
--rw-rw-rw-   0        0        0      264 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_svg.py
--rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_tiff.py
--rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_xml.py
--rw-rw-rw-   0        0        0      284 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_pdf_storage_xps.py
--rw-rw-rw-   0        0        0     1066 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_polyline_annotation.py
--rw-rw-rw-   0        0        0      919 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_popup_annotations.py
--rw-rw-rw-   0        0        0     1056 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_redaction_annotation.py
--rw-rw-rw-   0        0        0      958 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_screen_annotation.py
--rw-rw-rw-   0        0        0      380 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_screen_annotation_data_extarct.py
--rw-rw-rw-   0        0        0     1006 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_sound_annotation.py
--rw-rw-rw-   0        0        0      412 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_sound_annotation_data_extract.py
--rw-rw-rw-   0        0        0      866 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_square_annotation.py
--rw-rw-rw-   0        0        0     1110 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_squiggly_annotation.py
--rw-rw-rw-   0        0        0     1006 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_stamp_annotations.py
--rw-rw-rw-   0        0        0      412 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_stamp_annotations_data_extarct.py
--rw-rw-rw-   0        0        0     1115 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_strikeout_annotation.py
--rw-rw-rw-   0        0        0      296 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_svg_storage_pdf.py
--rw-rw-rw-   0        0        0      908 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_text_annotation.py
--rw-rw-rw-   0        0        0     1109 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_underline_annotations.py
--rw-rw-rw-   0        0        0      226 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_web_storage_pdf.py
--rw-rw-rw-   0        0        0      281 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_xfa_pdf_request_acro.py
--rw-rw-rw-   0        0        0      302 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_xfa_pdf_storage_acro.py
--rw-rw-rw-   0        0        0      295 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_xps_storage_pdf.py
--rw-rw-rw-   0        0        0      309 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/Examples/put_xslfo_storage_pdf.py
--rw-rw-rw-   0        0        0     1094 2023-02-21 05:28:12.000000 asposepdfcloud-23.5.0/LICENSE
--rw-rw-rw-   0        0        0       45 2021-10-29 10:28:29.000000 asposepdfcloud-23.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2869 2023-05-24 08:32:50.943620 asposepdfcloud-23.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3823 2023-05-23 03:52:57.000000 asposepdfcloud-23.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 08:32:42.949342 asposepdfcloud-23.5.0/asposepdfcloud/
--rw-rw-rw-   0        0        0    17470 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/__init__.py
--rw-rw-rw-   0        0        0    27131 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:32:43.293097 asposepdfcloud-23.5.0/asposepdfcloud/apis/
--rw-rw-rw-   0        0        0     1292 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/apis/__init__.py
--rw-rw-rw-   0        0        0  2097739 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/apis/pdf_api.py
--rw-rw-rw-   0        0        0     6707 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/configuration.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:32:50.943620 asposepdfcloud-23.5.0/asposepdfcloud/models/
--rw-rw-rw-   0        0        0    15280 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/__init__.py
--rw-rw-rw-   0        0        0    12403 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotation.py
--rw-rw-rw-   0        0        0     3745 2023-05-23 03:52:43.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_flags.py
--rw-rw-rw-   0        0        0    13587 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_info.py
--rw-rw-rw-   0        0        0     3660 2023-05-23 03:52:43.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_state.py
--rw-rw-rw-   0        0        0     4141 2023-05-23 03:52:43.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_type.py
--rw-rw-rw-   0        0        0     4797 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotations_info.py
--rw-rw-rw-   0        0        0     5720 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/annotations_info_response.py
--rw-rw-rw-   0        0        0     3589 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/antialiasing_processing_type.py
--rw-rw-rw-   0        0        0     4774 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/aspose_response.py
--rw-rw-rw-   0        0        0     9969 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/attachment.py
--rw-rw-rw-   0        0        0     5612 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/attachment_response.py
--rw-rw-rw-   0        0        0     4720 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/attachments.py
--rw-rw-rw-   0        0        0     5652 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/attachments_response.py
--rw-rw-rw-   0        0        0    17128 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/bookmark.py
--rw-rw-rw-   0        0        0     5532 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/bookmark_response.py
--rw-rw-rw-   0        0        0     4685 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/bookmarks.py
--rw-rw-rw-   0        0        0     5572 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/bookmarks_response.py
--rw-rw-rw-   0        0        0     7569 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/border.py
--rw-rw-rw-   0        0        0     3496 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/border_corner_style.py
--rw-rw-rw-   0        0        0     3483 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/border_effect.py
--rw-rw-rw-   0        0        0     7277 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/border_info.py
--rw-rw-rw-   0        0        0     3557 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/border_style.py
--rw-rw-rw-   0        0        0     3561 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/box_style.py
--rw-rw-rw-   0        0        0     3487 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/cap_style.py
--rw-rw-rw-   0        0        0     3490 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/caption_position.py
--rw-rw-rw-   0        0        0    17162 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotation.py
--rw-rw-rw-   0        0        0     5714 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotation_response.py
--rw-rw-rw-   0        0        0     4799 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotations.py
--rw-rw-rw-   0        0        0     5754 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotations_response.py
--rw-rw-rw-   0        0        0     3486 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/caret_symbol.py
--rw-rw-rw-   0        0        0    16502 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/cell.py
--rw-rw-rw-   0        0        0     5115 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/cell_recognized.py
--rw-rw-rw-   0        0        0    23077 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_field.py
--rw-rw-rw-   0        0        0     5574 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_field_response.py
--rw-rw-rw-   0        0        0     4767 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_fields.py
--rw-rw-rw-   0        0        0     5614 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_fields_response.py
--rw-rw-rw-   0        0        0    20470 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/choice_field.py
--rw-rw-rw-   0        0        0    17392 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotation.py
--rw-rw-rw-   0        0        0     5734 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotation_response.py
--rw-rw-rw-   0        0        0     4815 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotations.py
--rw-rw-rw-   0        0        0     5774 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotations_response.py
--rw-rw-rw-   0        0        0     5781 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/color.py
--rw-rw-rw-   0        0        0     3553 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/color_depth.py
--rw-rw-rw-   0        0        0     3568 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/column_adjustment.py
--rw-rw-rw-   0        0        0    23871 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_field.py
--rw-rw-rw-   0        0        0     5574 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_field_response.py
--rw-rw-rw-   0        0        0     4767 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_fields.py
--rw-rw-rw-   0        0        0     5614 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_fields_response.py
--rw-rw-rw-   0        0        0    17842 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/common_figure_annotation.py
--rw-rw-rw-   0        0        0     3549 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/compression_type.py
--rw-rw-rw-   0        0        0     3548 2023-05-23 03:52:44.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/crypto_algorithm.py
--rw-rw-rw-   0        0        0     4699 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/dash.py
--rw-rw-rw-   0        0        0     4787 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/default_page_config.py
--rw-rw-rw-   0        0        0     3466 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/direction.py
--rw-rw-rw-   0        0        0     4996 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/disc_usage.py
--rw-rw-rw-   0        0        0    13041 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/display_properties.py
--rw-rw-rw-   0        0        0     5911 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/display_properties_response.py
--rw-rw-rw-   0        0        0     3468 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/doc_format.py
--rw-rw-rw-   0        0        0     3606 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/doc_mdp_access_permission_type.py
--rw-rw-rw-   0        0        0     3503 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/doc_recognition_mode.py
--rw-rw-rw-   0        0        0     6580 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document.py
--rw-rw-rw-   0        0        0     7339 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_config.py
--rw-rw-rw-   0        0        0     5492 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_page_response.py
--rw-rw-rw-   0        0        0     5530 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_pages_response.py
--rw-rw-rw-   0        0        0    16115 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_privilege.py
--rw-rw-rw-   0        0        0     4836 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_properties.py
--rw-rw-rw-   0        0        0     5951 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_properties_response.py
--rw-rw-rw-   0        0        0     6267 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_property.py
--rw-rw-rw-   0        0        0     5871 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_property_response.py
--rw-rw-rw-   0        0        0     6353 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/document_response.py
--rw-rw-rw-   0        0        0     3527 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/epub_recognition_mode.py
--rw-rw-rw-   0        0        0     6159 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/error.py
--rw-rw-rw-   0        0        0     4808 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/error_details.py
--rw-rw-rw-   0        0        0     7357 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/field.py
--rw-rw-rw-   0        0        0     5412 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/field_response.py
--rw-rw-rw-   0        0        0     3520 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/field_type.py
--rw-rw-rw-   0        0        0     4719 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/fields.py
--rw-rw-rw-   0        0        0     5452 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/fields_response.py
--rw-rw-rw-   0        0        0    20586 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotation.py
--rw-rw-rw-   0        0        0     5894 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotation_response.py
--rw-rw-rw-   0        0        0     4943 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotations.py
--rw-rw-rw-   0        0        0     5924 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotations_response.py
--rw-rw-rw-   0        0        0     3521 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_icon.py
--rw-rw-rw-   0        0        0     8697 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_version.py
--rw-rw-rw-   0        0        0     4085 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4112 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/files_list.py
--rw-rw-rw-   0        0        0     4867 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     3552 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/font_encoding_rules.py
--rw-rw-rw-   0        0        0     3618 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/font_saving_modes.py
--rw-rw-rw-   0        0        0     3533 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/font_styles.py
--rw-rw-rw-   0        0        0    18666 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/form_field.py
--rw-rw-rw-   0        0        0    19228 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotation.py
--rw-rw-rw-   0        0        0     5776 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotation_response.py
--rw-rw-rw-   0        0        0     4849 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotations.py
--rw-rw-rw-   0        0        0     5816 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotations_response.py
--rw-rw-rw-   0        0        0     3564 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_intent.py
--rw-rw-rw-   0        0        0    13133 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/graph_info.py
--rw-rw-rw-   0        0        0    17162 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotation.py
--rw-rw-rw-   0        0        0     5794 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotation_response.py
--rw-rw-rw-   0        0        0     4863 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotations.py
--rw-rw-rw-   0        0        0     5834 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotations_response.py
--rw-rw-rw-   0        0        0     3544 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/horizontal_alignment.py
--rw-rw-rw-   0        0        0     3495 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/html_document_type.py
--rw-rw-rw-   0        0        0     3566 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/html_markup_generation_modes.py
--rw-rw-rw-   0        0        0     7573 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image.py
--rw-rw-rw-   0        0        0     3541 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_compression_version.py
--rw-rw-rw-   0        0        0     3540 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_encoding.py
--rw-rw-rw-   0        0        0    16417 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_footer.py
--rw-rw-rw-   0        0        0     9612 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_fragment.py
--rw-rw-rw-   0        0        0    16351 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_header.py
--rw-rw-rw-   0        0        0     5412 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_response.py
--rw-rw-rw-   0        0        0     3481 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_src_type.py
--rw-rw-rw-   0        0        0    18138 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_stamp.py
--rw-rw-rw-   0        0        0    10409 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_template.py
--rw-rw-rw-   0        0        0     6405 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/image_templates_request.py
--rw-rw-rw-   0        0        0     4637 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/images.py
--rw-rw-rw-   0        0        0     5452 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/images_response.py
--rw-rw-rw-   0        0        0    17271 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotation.py
--rw-rw-rw-   0        0        0     5674 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotation_response.py
--rw-rw-rw-   0        0        0     4767 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotations.py
--rw-rw-rw-   0        0        0     5714 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotations_response.py
--rw-rw-rw-   0        0        0     3507 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/justification.py
--rw-rw-rw-   0        0        0     3666 2023-05-23 03:52:45.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/letters_positioning_methods.py
--rw-rw-rw-   0        0        0    26346 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotation.py
--rw-rw-rw-   0        0        0     5694 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotation_response.py
--rw-rw-rw-   0        0        0     4783 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotations.py
--rw-rw-rw-   0        0        0     5734 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotations_response.py
--rw-rw-rw-   0        0        0     3693 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_ending.py
--rw-rw-rw-   0        0        0     3530 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_intent.py
--rw-rw-rw-   0        0        0     3492 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/line_spacing.py
--rw-rw-rw-   0        0        0     7200 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link.py
--rw-rw-rw-   0        0        0     3669 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_action_type.py
--rw-rw-rw-   0        0        0     8455 2023-05-23 03:52:48.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotation.py
--rw-rw-rw-   0        0        0     5572 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotation_response.py
--rw-rw-rw-   0        0        0     4783 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotations.py
--rw-rw-rw-   0        0        0     5612 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotations_response.py
--rw-rw-rw-   0        0        0     4047 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_element.py
--rw-rw-rw-   0        0        0     3574 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/link_highlighting_mode.py
--rw-rw-rw-   0        0        0    24041 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_field.py
--rw-rw-rw-   0        0        0     5554 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_field_response.py
--rw-rw-rw-   0        0        0     4751 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_fields.py
--rw-rw-rw-   0        0        0     5594 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_fields_response.py
--rw-rw-rw-   0        0        0     6250 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/margin_info.py
--rw-rw-rw-   0        0        0    15771 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/markup_annotation.py
--rw-rw-rw-   0        0        0     4135 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/merge_documents.py
--rw-rw-rw-   0        0        0    14871 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotation.py
--rw-rw-rw-   0        0        0     5714 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotation_response.py
--rw-rw-rw-   0        0        0     4799 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotations.py
--rw-rw-rw-   0        0        0     5754 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotations_response.py
--rw-rw-rw-   0        0        0     5025 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/object_exist.py
--rw-rw-rw-   0        0        0    19320 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/optimize_options.py
--rw-rw-rw-   0        0        0     6089 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/option.py
--rw-rw-rw-   0        0        0     5360 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/organize_document_data.py
--rw-rw-rw-   0        0        0     4263 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/organize_document_request.py
--rw-rw-rw-   0        0        0     3481 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/output_format.py
--rw-rw-rw-   0        0        0     5962 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/page.py
--rw-rw-rw-   0        0        0     3664 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/page_layout.py
--rw-rw-rw-   0        0        0     3607 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/page_mode.py
--rw-rw-rw-   0        0        0    17912 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/page_number_stamp.py
--rw-rw-rw-   0        0        0     4472 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/page_range.py
--rw-rw-rw-   0        0        0     4968 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/page_word_count.py
--rw-rw-rw-   0        0        0     4621 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/pages.py
--rw-rw-rw-   0        0        0    13318 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/paragraph.py
--rw-rw-rw-   0        0        0     3573 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/parts_embedding_modes.py
--rw-rw-rw-   0        0        0     3498 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/pdf_a_type.py
--rw-rw-rw-   0        0        0    17482 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/pdf_page_stamp.py
--rw-rw-rw-   0        0        0     3801 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/permissions_flags.py
--rw-rw-rw-   0        0        0     4595 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/point.py
--rw-rw-rw-   0        0        0    20166 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/poly_annotation.py
--rw-rw-rw-   0        0        0     3587 2023-05-23 03:52:46.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/poly_intent.py
--rw-rw-rw-   0        0        0    20514 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotation.py
--rw-rw-rw-   0        0        0     5774 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotation_response.py
--rw-rw-rw-   0        0        0     4847 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotations.py
--rw-rw-rw-   0        0        0     5814 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotations_response.py
--rw-rw-rw-   0        0        0    20427 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotation.py
--rw-rw-rw-   0        0        0     5754 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotation_response.py
--rw-rw-rw-   0        0        0     4831 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotations.py
--rw-rw-rw-   0        0        0     5794 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotations_response.py
--rw-rw-rw-   0        0        0    13460 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotation.py
--rw-rw-rw-   0        0        0     5744 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotation_response.py
--rw-rw-rw-   0        0        0    14772 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotation_with_parent.py
--rw-rw-rw-   0        0        0     4829 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotations.py
--rw-rw-rw-   0        0        0     5754 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotations_response.py
--rw-rw-rw-   0        0        0     4984 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/position.py
--rw-rw-rw-   0        0        0    23616 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_field.py
--rw-rw-rw-   0        0        0     5634 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_field_response.py
--rw-rw-rw-   0        0        0     4809 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_fields.py
--rw-rw-rw-   0        0        0     5668 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_fields_response.py
--rw-rw-rw-   0        0        0    21291 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_option_field.py
--rw-rw-rw-   0        0        0     3695 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/raster_images_saving_modes.py
--rw-rw-rw-   0        0        0     6219 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/rectangle.py
--rw-rw-rw-   0        0        0    18170 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotation.py
--rw-rw-rw-   0        0        0     5794 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotation_response.py
--rw-rw-rw-   0        0        0     4863 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotations.py
--rw-rw-rw-   0        0        0     5834 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotations_response.py
--rw-rw-rw-   0        0        0     3509 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/rotation.py
--rw-rw-rw-   0        0        0    13011 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/row.py
--rw-rw-rw-   0        0        0     5053 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/row_recognized.py
--rw-rw-rw-   0        0        0    14148 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotation.py
--rw-rw-rw-   0        0        0     5734 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotation_response.py
--rw-rw-rw-   0        0        0     4815 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotations.py
--rw-rw-rw-   0        0        0     5774 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotations_response.py
--rw-rw-rw-   0        0        0     5085 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/segment.py
--rw-rw-rw-   0        0        0     3507 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/shape_type.py
--rw-rw-rw-   0        0        0    17074 2021-10-29 08:53:57.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature.py
--rw-rw-rw-   0        0        0    15711 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_custom_appearance.py
--rw-rw-rw-   0        0        0    20192 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_field.py
--rw-rw-rw-   0        0        0     5594 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_field_response.py
--rw-rw-rw-   0        0        0     4783 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_fields.py
--rw-rw-rw-   0        0        0     5634 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_fields_response.py
--rw-rw-rw-   0        0        0     3523 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_type.py
--rw-rw-rw-   0        0        0     5694 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/signature_verify_response.py
--rw-rw-rw-   0        0        0    20322 2021-10-29 08:53:57.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotation.py
--rw-rw-rw-   0        0        0     5714 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotation_response.py
--rw-rw-rw-   0        0        0     4799 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotations.py
--rw-rw-rw-   0        0        0     5754 2023-05-23 03:52:49.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotations_response.py
--rw-rw-rw-   0        0        0     3524 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/sound_encoding.py
--rw-rw-rw-   0        0        0     3474 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/sound_icon.py
--rw-rw-rw-   0        0        0     4182 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/split_range_pdf_options.py
--rw-rw-rw-   0        0        0     4200 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/split_result.py
--rw-rw-rw-   0        0        0     8196 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/split_result_document.py
--rw-rw-rw-   0        0        0     5554 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/split_result_response.py
--rw-rw-rw-   0        0        0    17392 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotation.py
--rw-rw-rw-   0        0        0     5734 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotation_response.py
--rw-rw-rw-   0        0        0     4815 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotations.py
--rw-rw-rw-   0        0        0     5774 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotations_response.py
--rw-rw-rw-   0        0        0    17057 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotation.py
--rw-rw-rw-   0        0        0     5794 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotation_response.py
--rw-rw-rw-   0        0        0     4867 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotations.py
--rw-rw-rw-   0        0        0     5834 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotations_response.py
--rw-rw-rw-   0        0        0    22009 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp.py
--rw-rw-rw-   0        0        0    17904 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotation.py
--rw-rw-rw-   0        0        0     5710 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotation_response.py
--rw-rw-rw-   0        0        0     4799 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotations.py
--rw-rw-rw-   0        0        0     5754 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotations_response.py
--rw-rw-rw-   0        0        0    11543 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_base.py
--rw-rw-rw-   0        0        0     3854 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_icon.py
--rw-rw-rw-   0        0        0     9021 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_info.py
--rw-rw-rw-   0        0        0     3522 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_type.py
--rw-rw-rw-   0        0        0     4693 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamps_info.py
--rw-rw-rw-   0        0        0     5520 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/stamps_info_response.py
--rw-rw-rw-   0        0        0     4174 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7015 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/storage_file.py
--rw-rw-rw-   0        0        0    17128 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotation.py
--rw-rw-rw-   0        0        0     5794 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotation_response.py
--rw-rw-rw-   0        0        0     4863 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotations.py
--rw-rw-rw-   0        0        0     5834 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotations_response.py
--rw-rw-rw-   0        0        0    23748 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/table.py
--rw-rw-rw-   0        0        0     3531 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/table_broken.py
--rw-rw-rw-   0        0        0     7133 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/table_recognized.py
--rw-rw-rw-   0        0        0     5612 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/table_recognized_response.py
--rw-rw-rw-   0        0        0     4777 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/tables_recognized.py
--rw-rw-rw-   0        0        0     5652 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/tables_recognized_response.py
--rw-rw-rw-   0        0        0    17854 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotation.py
--rw-rw-rw-   0        0        0     5694 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotation_response.py
--rw-rw-rw-   0        0        0     4783 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotations.py
--rw-rw-rw-   0        0        0     5734 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotations_response.py
--rw-rw-rw-   0        0        0    24062 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_field.py
--rw-rw-rw-   0        0        0     5556 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_field_response.py
--rw-rw-rw-   0        0        0     4753 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_fields.py
--rw-rw-rw-   0        0        0     5596 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_fields_response.py
--rw-rw-rw-   0        0        0    16535 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_footer.py
--rw-rw-rw-   0        0        0    16469 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_header.py
--rw-rw-rw-   0        0        0     3614 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_horizontal_alignment.py
--rw-rw-rw-   0        0        0     3680 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_icon.py
--rw-rw-rw-   0        0        0     5273 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_line.py
--rw-rw-rw-   0        0        0    10182 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_rect.py
--rw-rw-rw-   0        0        0     4041 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_rects.py
--rw-rw-rw-   0        0        0     5711 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_rects_response.py
--rw-rw-rw-   0        0        0     8530 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_replace.py
--rw-rw-rw-   0        0        0     7087 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_replace_list_request.py
--rw-rw-rw-   0        0        0     5621 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_replace_response.py
--rw-rw-rw-   0        0        0    18248 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_stamp.py
--rw-rw-rw-   0        0        0    11377 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_state.py
--rw-rw-rw-   0        0        0     7403 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/text_style.py
--rw-rw-rw-   0        0        0     5406 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/timestamp_settings.py
--rw-rw-rw-   0        0        0    17128 2023-05-23 03:52:51.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotation.py
--rw-rw-rw-   0        0        0     5794 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotation_response.py
--rw-rw-rw-   0        0        0     4863 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotations.py
--rw-rw-rw-   0        0        0     5834 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotations_response.py
--rw-rw-rw-   0        0        0     3538 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/vertical_alignment.py
--rw-rw-rw-   0        0        0     3978 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/word_count.py
--rw-rw-rw-   0        0        0     5708 2023-05-23 03:52:50.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/word_count_response.py
--rw-rw-rw-   0        0        0     3536 2023-05-23 03:52:47.000000 asposepdfcloud-23.5.0/asposepdfcloud/models/wrap_mode.py
--rw-rw-rw-   0        0        0    14812 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/asposepdfcloud/rest.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:32:43.011843 asposepdfcloud-23.5.0/asposepdfcloud.egg-info/
--rw-rw-rw-   0        0        0     2869 2023-05-24 08:32:37.000000 asposepdfcloud-23.5.0/asposepdfcloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19197 2023-05-24 08:32:37.000000 asposepdfcloud-23.5.0/asposepdfcloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 08:32:37.000000 asposepdfcloud-23.5.0/asposepdfcloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-05-24 08:32:37.000000 asposepdfcloud-23.5.0/asposepdfcloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-24 08:32:37.000000 asposepdfcloud-23.5.0/asposepdfcloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 08:32:50.943620 asposepdfcloud-23.5.0/setup.cfg
--rw-rw-rw-   0        0        0     6037 2023-05-23 03:52:53.000000 asposepdfcloud-23.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:22:36.738754 asposepdfcloud-23.6.0/
+drwxrwxrwx   0        0        0        0 2023-06-29 11:22:35.473110 asposepdfcloud-23.6.0/Examples/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/__init__.py
+-rw-rw-rw-   0        0        0      464 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/configuration.py
+-rw-rw-rw-   0        0        0      347 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/delete_all_annotations.py
+-rw-rw-rw-   0        0        0      187 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/delete_document_annotations.py
+-rw-rw-rw-   0        0        0      217 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/delete_page_annotations.py
+-rw-rw-rw-   0        0        0      368 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_carret_annotations.py
+-rw-rw-rw-   0        0        0      370 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_circle_annotation.py
+-rw-rw-rw-   0        0        0      119 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_annotatios.py
+-rw-rw-rw-   0        0        0      220 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_attachment.py
+-rw-rw-rw-   0        0        0      274 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_attachment_by_index.py
+-rw-rw-rw-   0        0        0      283 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_bookamarks.py
+-rw-rw-rw-   0        0        0      212 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_bookmars.py
+-rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_carret_annotation.py
+-rw-rw-rw-   0        0        0      197 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_circle_annotations.py
+-rw-rw-rw-   0        0        0      206 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_file_annotations.py
+-rw-rw-rw-   0        0        0      206 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_free_text_annotations.py
+-rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_highlight_annotations.py
+-rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_ink_annotations.py
+-rw-rw-rw-   0        0        0      193 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_line_annotations.py
+-rw-rw-rw-   0        0        0      201 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_movie_annotations.py
+-rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_polygon_annotations.py
+-rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_polyline_annotations.py
+-rw-rw-rw-   0        0        0      270 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_popup_annotation_parent.py
+-rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_redaction_annotation.py
+-rw-rw-rw-   0        0        0      211 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_screen_annotations.py
+-rw-rw-rw-   0        0        0      201 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_sqiuggly_annotation.py
+-rw-rw-rw-   0        0        0      201 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_square_annotations.py
+-rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_storage_pdf.py
+-rw-rw-rw-   0        0        0      205 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_strikeout_annotation.py
+-rw-rw-rw-   0        0        0      204 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_document_underline_annotations.py
+-rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_doucment_popup_annotations.py
+-rw-rw-rw-   0        0        0      195 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_doument_annotations.py
+-rw-rw-rw-   0        0        0      192 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_doument_sound_annotations.py
+-rw-rw-rw-   0        0        0      369 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_file_attachment_annotations.py
+-rw-rw-rw-   0        0        0      393 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_file_attachment_annotations_data.py
+-rw-rw-rw-   0        0        0      378 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_free_text_annotation.py
+-rw-rw-rw-   0        0        0      376 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_hightlight_annotation.py
+-rw-rw-rw-   0        0        0      341 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_html_storage_pdf.py
+-rw-rw-rw-   0        0        0      364 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_ink_annotations.py
+-rw-rw-rw-   0        0        0      368 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_line_annotation.py
+-rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_mht_storage_pdf.py
+-rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_movie_annotation.py
+-rw-rw-rw-   0        0        0      214 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_annotations.py
+-rw-rw-rw-   0        0        0      228 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_carret_annotations.py
+-rw-rw-rw-   0        0        0      229 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_cirlce_annotations.py
+-rw-rw-rw-   0        0        0      233 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_file_attachment_annotations.py
+-rw-rw-rw-   0        0        0      234 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_free_text_annotations.py
+-rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_highlight_annotations.py
+-rw-rw-rw-   0        0        0      226 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_ink_annotations.py
+-rw-rw-rw-   0        0        0      227 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_line_annotations.py
+-rw-rw-rw-   0        0        0      231 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_movie_annotations.py
+-rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_polygon_annotations.py
+-rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_polyline_annotations.py
+-rw-rw-rw-   0        0        0      228 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_popup_annotations.py
+-rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_redaction_annotation.py
+-rw-rw-rw-   0        0        0      235 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_screen_annotations.py
+-rw-rw-rw-   0        0        0      228 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_sound_annotations.py
+-rw-rw-rw-   0        0        0      227 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_square_annotations.py
+-rw-rw-rw-   0        0        0      225 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_squiggly_annotations.py
+-rw-rw-rw-   0        0        0      230 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_stamp_annotations.py
+-rw-rw-rw-   0        0        0      233 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_strikeout_annotations.py
+-rw-rw-rw-   0        0        0      227 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_text_annotations.py
+-rw-rw-rw-   0        0        0      232 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_page_underline_annotations.py
+-rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pcl_storage.py
+-rw-rw-rw-   0        0        0      206 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_epub.py
+-rw-rw-rw-   0        0        0      208 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_html.py
+-rw-rw-rw-   0        0        0      217 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_latext.py
+-rw-rw-rw-   0        0        0      210 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_mobi_xml.py
+-rw-rw-rw-   0        0        0      254 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_pdfa.py
+-rw-rw-rw-   0        0        0      208 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_pptx.py
+-rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_svg.py
+-rw-rw-rw-   0        0        0      208 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_tiff.py
+-rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_xls.py
+-rw-rw-rw-   0        0        0      209 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_xml.py
+-rw-rw-rw-   0        0        0      207 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_pdf_storage_xvg.py
+-rw-rw-rw-   0        0        0      374 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_polygon_annotation.py
+-rw-rw-rw-   0        0        0      374 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_polyline_annotation.py
+-rw-rw-rw-   0        0        0      376 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_redaction_annotation.py
+-rw-rw-rw-   0        0        0      376 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_screen_annotation.py
+-rw-rw-rw-   0        0        0      370 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_sound_annotation.py
+-rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_sound_annotation_data.py
+-rw-rw-rw-   0        0        0      370 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_square_annotation.py
+-rw-rw-rw-   0        0        0      374 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_squiggly_annotation.py
+-rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_stamp_annotations_data.py
+-rw-rw-rw-   0        0        0      378 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_strikeout_annotation.py
+-rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_svg_storage.py
+-rw-rw-rw-   0        0        0      368 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_text_annotation.py
+-rw-rw-rw-   0        0        0      372 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_underline_annotations.py
+-rw-rw-rw-   0        0        0      375 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_underline_annottion.py
+-rw-rw-rw-   0        0        0      128 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_web_storage.py
+-rw-rw-rw-   0        0        0      225 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_xfa_pdf_storage_acro.py
+-rw-rw-rw-   0        0        0      200 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_xml_storage_pdf.py
+-rw-rw-rw-   0        0        0      198 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_xps_storage_pdf.py
+-rw-rw-rw-   0        0        0      209 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/get_xslfo_storage.py
+-rw-rw-rw-   0        0        0      371 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_append_document.py
+-rw-rw-rw-   0        0        0      444 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_append_document_body_params.py
+-rw-rw-rw-   0        0        0     1066 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_ink_annotations.py
+-rw-rw-rw-   0        0        0      833 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_carret_annotations.py
+-rw-rw-rw-   0        0        0      676 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_circle_annotations.py
+-rw-rw-rw-   0        0        0      928 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_file_attachment_annotations.py
+-rw-rw-rw-   0        0        0     1263 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_free_annotations.py
+-rw-rw-rw-   0        0        0      948 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_highlight_annotations.py
+-rw-rw-rw-   0        0        0      783 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_line_annotations.py
+-rw-rw-rw-   0        0        0      775 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_movie_annotations.py
+-rw-rw-rw-   0        0        0      894 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_polygon_annotations.py
+-rw-rw-rw-   0        0        0      894 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_polyline_annotations.py
+-rw-rw-rw-   0        0        0      774 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_redaction_annotations.py
+-rw-rw-rw-   0        0        0      817 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_screen_annotations.py
+-rw-rw-rw-   0        0        0      869 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_sound_annotations.py
+-rw-rw-rw-   0        0        0      702 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_square_annotations.py
+-rw-rw-rw-   0        0        0      946 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_squiggly_annotations.py
+-rw-rw-rw-   0        0        0      867 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_stamp_annotations.py
+-rw-rw-rw-   0        0        0      947 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_strikeout_annotations.py
+-rw-rw-rw-   0        0        0      773 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_text_annotations.py
+-rw-rw-rw-   0        0        0      944 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_page_underline_annotations.py
+-rw-rw-rw-   0        0        0      667 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/post_popup_annotations.py
+-rw-rw-rw-   0        0        0      997 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_carret_annotations.py
+-rw-rw-rw-   0        0        0      862 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_circle_annotation.py
+-rw-rw-rw-   0        0        0      284 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_df_storage_xls.py
+-rw-rw-rw-   0        0        0      301 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_epub_storage_pdf.py
+-rw-rw-rw-   0        0        0      383 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_file_attachement_annotations.py
+-rw-rw-rw-   0        0        0     1071 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_file_attachment_annotations.py
+-rw-rw-rw-   0        0        0     1403 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_free_text_annotation.py
+-rw-rw-rw-   0        0        0     1115 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_hightlight_annotation.py
+-rw-rw-rw-   0        0        0      425 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_html_storage_pdf.py
+-rw-rw-rw-   0        0        0     1249 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_ink_annotations.py
+-rw-rw-rw-   0        0        0      942 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_line_annotation.py
+-rw-rw-rw-   0        0        0      300 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_mht_storage_pdf.py
+-rw-rw-rw-   0        0        0      912 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_movie_annotation.py
+-rw-rw-rw-   0        0        0      300 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pcl_storage_pdf.py
+-rw-rw-rw-   0        0        0      265 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_epub.py
+-rw-rw-rw-   0        0        0      264 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_html.py
+-rw-rw-rw-   0        0        0      255 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_latext.py
+-rw-rw-rw-   0        0        0      267 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_mobi_xml.py
+-rw-rw-rw-   0        0        0      314 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_pdfa.py
+-rw-rw-rw-   0        0        0      265 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_pptx.py
+-rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_svg.py
+-rw-rw-rw-   0        0        0      267 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_tiff.py
+-rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_to_doc.py
+-rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_xls.py
+-rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_xml.py
+-rw-rw-rw-   0        0        0      263 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_request_xps.py
+-rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_epub.py
+-rw-rw-rw-   0        0        0      285 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_html.py
+-rw-rw-rw-   0        0        0      290 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_latext.py
+-rw-rw-rw-   0        0        0      290 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_mobi_xml.py
+-rw-rw-rw-   0        0        0      282 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_pdf.py
+-rw-rw-rw-   0        0        0      338 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_pdfa.py
+-rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_pptx.py
+-rw-rw-rw-   0        0        0      264 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_svg.py
+-rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_tiff.py
+-rw-rw-rw-   0        0        0      286 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_xml.py
+-rw-rw-rw-   0        0        0      284 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_pdf_storage_xps.py
+-rw-rw-rw-   0        0        0     1066 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_polyline_annotation.py
+-rw-rw-rw-   0        0        0      919 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_popup_annotations.py
+-rw-rw-rw-   0        0        0     1056 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_redaction_annotation.py
+-rw-rw-rw-   0        0        0      958 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_screen_annotation.py
+-rw-rw-rw-   0        0        0      380 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_screen_annotation_data_extarct.py
+-rw-rw-rw-   0        0        0     1006 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_sound_annotation.py
+-rw-rw-rw-   0        0        0      412 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_sound_annotation_data_extract.py
+-rw-rw-rw-   0        0        0      866 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_square_annotation.py
+-rw-rw-rw-   0        0        0     1110 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_squiggly_annotation.py
+-rw-rw-rw-   0        0        0     1006 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_stamp_annotations.py
+-rw-rw-rw-   0        0        0      412 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_stamp_annotations_data_extarct.py
+-rw-rw-rw-   0        0        0     1115 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_strikeout_annotation.py
+-rw-rw-rw-   0        0        0      296 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_svg_storage_pdf.py
+-rw-rw-rw-   0        0        0      908 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_text_annotation.py
+-rw-rw-rw-   0        0        0     1109 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_underline_annotations.py
+-rw-rw-rw-   0        0        0      226 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_web_storage_pdf.py
+-rw-rw-rw-   0        0        0      281 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_xfa_pdf_request_acro.py
+-rw-rw-rw-   0        0        0      302 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_xfa_pdf_storage_acro.py
+-rw-rw-rw-   0        0        0      295 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_xps_storage_pdf.py
+-rw-rw-rw-   0        0        0      309 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/Examples/put_xslfo_storage_pdf.py
+-rw-rw-rw-   0        0        0     1094 2023-02-21 05:28:12.000000 asposepdfcloud-23.6.0/LICENSE
+-rw-rw-rw-   0        0        0       45 2021-10-29 10:28:29.000000 asposepdfcloud-23.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2869 2023-06-29 11:22:36.738754 asposepdfcloud-23.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3984 2023-06-29 05:39:23.000000 asposepdfcloud-23.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 11:22:35.488738 asposepdfcloud-23.6.0/asposepdfcloud/
+-rw-rw-rw-   0        0        0    17470 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/__init__.py
+-rw-rw-rw-   0        0        0    27131 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/api_client.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:22:35.551236 asposepdfcloud-23.6.0/asposepdfcloud/apis/
+-rw-rw-rw-   0        0        0     1292 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/apis/__init__.py
+-rw-rw-rw-   0        0        0  2098408 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/apis/pdf_api.py
+-rw-rw-rw-   0        0        0     6707 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:22:36.723130 asposepdfcloud-23.6.0/asposepdfcloud/models/
+-rw-rw-rw-   0        0        0    15280 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/__init__.py
+-rw-rw-rw-   0        0        0    12403 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotation.py
+-rw-rw-rw-   0        0        0     3745 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_flags.py
+-rw-rw-rw-   0        0        0    13587 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_info.py
+-rw-rw-rw-   0        0        0     3660 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_state.py
+-rw-rw-rw-   0        0        0     4141 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_type.py
+-rw-rw-rw-   0        0        0     4797 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotations_info.py
+-rw-rw-rw-   0        0        0     5720 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/annotations_info_response.py
+-rw-rw-rw-   0        0        0     3589 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/antialiasing_processing_type.py
+-rw-rw-rw-   0        0        0     4774 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/aspose_response.py
+-rw-rw-rw-   0        0        0     9969 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/attachment.py
+-rw-rw-rw-   0        0        0     5612 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/attachment_response.py
+-rw-rw-rw-   0        0        0     4720 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/attachments.py
+-rw-rw-rw-   0        0        0     5652 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/attachments_response.py
+-rw-rw-rw-   0        0        0    17128 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/bookmark.py
+-rw-rw-rw-   0        0        0     5532 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/bookmark_response.py
+-rw-rw-rw-   0        0        0     4685 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/bookmarks.py
+-rw-rw-rw-   0        0        0     5572 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/bookmarks_response.py
+-rw-rw-rw-   0        0        0     7569 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/border.py
+-rw-rw-rw-   0        0        0     3496 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/border_corner_style.py
+-rw-rw-rw-   0        0        0     3483 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/border_effect.py
+-rw-rw-rw-   0        0        0     7277 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/border_info.py
+-rw-rw-rw-   0        0        0     3557 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/border_style.py
+-rw-rw-rw-   0        0        0     3561 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/box_style.py
+-rw-rw-rw-   0        0        0     3487 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/cap_style.py
+-rw-rw-rw-   0        0        0     3490 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/caption_position.py
+-rw-rw-rw-   0        0        0    17162 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotation.py
+-rw-rw-rw-   0        0        0     5714 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotation_response.py
+-rw-rw-rw-   0        0        0     4799 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotations.py
+-rw-rw-rw-   0        0        0     5754 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotations_response.py
+-rw-rw-rw-   0        0        0     3486 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/caret_symbol.py
+-rw-rw-rw-   0        0        0    16502 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/cell.py
+-rw-rw-rw-   0        0        0     5115 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/cell_recognized.py
+-rw-rw-rw-   0        0        0    23077 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_field.py
+-rw-rw-rw-   0        0        0     5574 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_field_response.py
+-rw-rw-rw-   0        0        0     4767 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_fields.py
+-rw-rw-rw-   0        0        0     5614 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_fields_response.py
+-rw-rw-rw-   0        0        0    20470 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/choice_field.py
+-rw-rw-rw-   0        0        0    17392 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotation.py
+-rw-rw-rw-   0        0        0     5734 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotation_response.py
+-rw-rw-rw-   0        0        0     4815 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotations.py
+-rw-rw-rw-   0        0        0     5774 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotations_response.py
+-rw-rw-rw-   0        0        0     5781 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/color.py
+-rw-rw-rw-   0        0        0     3553 2023-06-29 05:39:08.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/color_depth.py
+-rw-rw-rw-   0        0        0     3568 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/column_adjustment.py
+-rw-rw-rw-   0        0        0    23871 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_field.py
+-rw-rw-rw-   0        0        0     5574 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_field_response.py
+-rw-rw-rw-   0        0        0     4767 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_fields.py
+-rw-rw-rw-   0        0        0     5614 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_fields_response.py
+-rw-rw-rw-   0        0        0    17842 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/common_figure_annotation.py
+-rw-rw-rw-   0        0        0     3549 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/compression_type.py
+-rw-rw-rw-   0        0        0     3548 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/crypto_algorithm.py
+-rw-rw-rw-   0        0        0     4699 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/dash.py
+-rw-rw-rw-   0        0        0     4787 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/default_page_config.py
+-rw-rw-rw-   0        0        0     3466 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/direction.py
+-rw-rw-rw-   0        0        0     4996 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0    13041 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/display_properties.py
+-rw-rw-rw-   0        0        0     5911 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/display_properties_response.py
+-rw-rw-rw-   0        0        0     3468 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/doc_format.py
+-rw-rw-rw-   0        0        0     3606 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/doc_mdp_access_permission_type.py
+-rw-rw-rw-   0        0        0     3503 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/doc_recognition_mode.py
+-rw-rw-rw-   0        0        0     6580 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document.py
+-rw-rw-rw-   0        0        0     7339 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_config.py
+-rw-rw-rw-   0        0        0     5492 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_page_response.py
+-rw-rw-rw-   0        0        0     5530 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_pages_response.py
+-rw-rw-rw-   0        0        0    16115 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_privilege.py
+-rw-rw-rw-   0        0        0     4836 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_properties.py
+-rw-rw-rw-   0        0        0     5951 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_properties_response.py
+-rw-rw-rw-   0        0        0     6267 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_property.py
+-rw-rw-rw-   0        0        0     5871 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_property_response.py
+-rw-rw-rw-   0        0        0     6353 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/document_response.py
+-rw-rw-rw-   0        0        0     3527 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/epub_recognition_mode.py
+-rw-rw-rw-   0        0        0     6159 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/error.py
+-rw-rw-rw-   0        0        0     4808 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/error_details.py
+-rw-rw-rw-   0        0        0     7357 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/field.py
+-rw-rw-rw-   0        0        0     5412 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/field_response.py
+-rw-rw-rw-   0        0        0     3520 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/field_type.py
+-rw-rw-rw-   0        0        0     4719 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/fields.py
+-rw-rw-rw-   0        0        0     5452 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/fields_response.py
+-rw-rw-rw-   0        0        0    20586 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotation.py
+-rw-rw-rw-   0        0        0     5894 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotation_response.py
+-rw-rw-rw-   0        0        0     4943 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotations.py
+-rw-rw-rw-   0        0        0     5924 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotations_response.py
+-rw-rw-rw-   0        0        0     3521 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_icon.py
+-rw-rw-rw-   0        0        0     8697 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4085 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4112 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4867 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     3552 2023-06-29 05:39:09.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/font_encoding_rules.py
+-rw-rw-rw-   0        0        0     3618 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/font_saving_modes.py
+-rw-rw-rw-   0        0        0     3533 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/font_styles.py
+-rw-rw-rw-   0        0        0    18666 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/form_field.py
+-rw-rw-rw-   0        0        0    19228 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotation.py
+-rw-rw-rw-   0        0        0     5776 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotation_response.py
+-rw-rw-rw-   0        0        0     4849 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotations.py
+-rw-rw-rw-   0        0        0     5816 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotations_response.py
+-rw-rw-rw-   0        0        0     3564 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_intent.py
+-rw-rw-rw-   0        0        0    13133 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/graph_info.py
+-rw-rw-rw-   0        0        0    17162 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotation.py
+-rw-rw-rw-   0        0        0     5794 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotation_response.py
+-rw-rw-rw-   0        0        0     4863 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotations.py
+-rw-rw-rw-   0        0        0     5834 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotations_response.py
+-rw-rw-rw-   0        0        0     3544 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/horizontal_alignment.py
+-rw-rw-rw-   0        0        0     3495 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/html_document_type.py
+-rw-rw-rw-   0        0        0     3566 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/html_markup_generation_modes.py
+-rw-rw-rw-   0        0        0     7573 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image.py
+-rw-rw-rw-   0        0        0     3541 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_compression_version.py
+-rw-rw-rw-   0        0        0     3540 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_encoding.py
+-rw-rw-rw-   0        0        0    16417 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_footer.py
+-rw-rw-rw-   0        0        0     9612 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_fragment.py
+-rw-rw-rw-   0        0        0    16351 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_header.py
+-rw-rw-rw-   0        0        0     5412 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_response.py
+-rw-rw-rw-   0        0        0     3481 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_src_type.py
+-rw-rw-rw-   0        0        0    18138 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_stamp.py
+-rw-rw-rw-   0        0        0    10409 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_template.py
+-rw-rw-rw-   0        0        0     6405 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/image_templates_request.py
+-rw-rw-rw-   0        0        0     4637 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/images.py
+-rw-rw-rw-   0        0        0     5452 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/images_response.py
+-rw-rw-rw-   0        0        0    17271 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotation.py
+-rw-rw-rw-   0        0        0     5674 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotation_response.py
+-rw-rw-rw-   0        0        0     4767 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotations.py
+-rw-rw-rw-   0        0        0     5714 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotations_response.py
+-rw-rw-rw-   0        0        0     3507 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/justification.py
+-rw-rw-rw-   0        0        0     3666 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/letters_positioning_methods.py
+-rw-rw-rw-   0        0        0    26346 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotation.py
+-rw-rw-rw-   0        0        0     5694 2023-06-29 05:39:13.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotation_response.py
+-rw-rw-rw-   0        0        0     4783 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotations.py
+-rw-rw-rw-   0        0        0     5734 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotations_response.py
+-rw-rw-rw-   0        0        0     3693 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_ending.py
+-rw-rw-rw-   0        0        0     3530 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_intent.py
+-rw-rw-rw-   0        0        0     3492 2023-06-29 05:39:10.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/line_spacing.py
+-rw-rw-rw-   0        0        0     7200 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link.py
+-rw-rw-rw-   0        0        0     3669 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_action_type.py
+-rw-rw-rw-   0        0        0     8455 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotation.py
+-rw-rw-rw-   0        0        0     5572 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotation_response.py
+-rw-rw-rw-   0        0        0     4783 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotations.py
+-rw-rw-rw-   0        0        0     5612 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotations_response.py
+-rw-rw-rw-   0        0        0     4047 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_element.py
+-rw-rw-rw-   0        0        0     3574 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/link_highlighting_mode.py
+-rw-rw-rw-   0        0        0    24041 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_field.py
+-rw-rw-rw-   0        0        0     5554 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_field_response.py
+-rw-rw-rw-   0        0        0     4751 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_fields.py
+-rw-rw-rw-   0        0        0     5594 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_fields_response.py
+-rw-rw-rw-   0        0        0     6250 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/margin_info.py
+-rw-rw-rw-   0        0        0    15771 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/markup_annotation.py
+-rw-rw-rw-   0        0        0     4135 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/merge_documents.py
+-rw-rw-rw-   0        0        0    14871 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotation.py
+-rw-rw-rw-   0        0        0     5714 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotation_response.py
+-rw-rw-rw-   0        0        0     4799 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotations.py
+-rw-rw-rw-   0        0        0     5754 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotations_response.py
+-rw-rw-rw-   0        0        0     5025 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/object_exist.py
+-rw-rw-rw-   0        0        0    19320 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/optimize_options.py
+-rw-rw-rw-   0        0        0     6089 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/option.py
+-rw-rw-rw-   0        0        0     5360 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/organize_document_data.py
+-rw-rw-rw-   0        0        0     4263 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/organize_document_request.py
+-rw-rw-rw-   0        0        0     3481 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/output_format.py
+-rw-rw-rw-   0        0        0     5962 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/page.py
+-rw-rw-rw-   0        0        0     3664 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/page_layout.py
+-rw-rw-rw-   0        0        0     3607 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/page_mode.py
+-rw-rw-rw-   0        0        0    17912 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/page_number_stamp.py
+-rw-rw-rw-   0        0        0     4472 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/page_range.py
+-rw-rw-rw-   0        0        0     4968 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/page_word_count.py
+-rw-rw-rw-   0        0        0     4621 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/pages.py
+-rw-rw-rw-   0        0        0    13318 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/paragraph.py
+-rw-rw-rw-   0        0        0     3573 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/parts_embedding_modes.py
+-rw-rw-rw-   0        0        0     3498 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/pdf_a_type.py
+-rw-rw-rw-   0        0        0    17482 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/pdf_page_stamp.py
+-rw-rw-rw-   0        0        0     3801 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/permissions_flags.py
+-rw-rw-rw-   0        0        0     4595 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/point.py
+-rw-rw-rw-   0        0        0    20166 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/poly_annotation.py
+-rw-rw-rw-   0        0        0     3587 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/poly_intent.py
+-rw-rw-rw-   0        0        0    20514 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotation.py
+-rw-rw-rw-   0        0        0     5774 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotation_response.py
+-rw-rw-rw-   0        0        0     4847 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotations.py
+-rw-rw-rw-   0        0        0     5814 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotations_response.py
+-rw-rw-rw-   0        0        0    20427 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotation.py
+-rw-rw-rw-   0        0        0     5754 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotation_response.py
+-rw-rw-rw-   0        0        0     4831 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotations.py
+-rw-rw-rw-   0        0        0     5794 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotations_response.py
+-rw-rw-rw-   0        0        0    13460 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotation.py
+-rw-rw-rw-   0        0        0     5744 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotation_response.py
+-rw-rw-rw-   0        0        0    14772 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotation_with_parent.py
+-rw-rw-rw-   0        0        0     4829 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotations.py
+-rw-rw-rw-   0        0        0     5754 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotations_response.py
+-rw-rw-rw-   0        0        0     4984 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/position.py
+-rw-rw-rw-   0        0        0    23616 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_field.py
+-rw-rw-rw-   0        0        0     5634 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_field_response.py
+-rw-rw-rw-   0        0        0     4809 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_fields.py
+-rw-rw-rw-   0        0        0     5668 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_fields_response.py
+-rw-rw-rw-   0        0        0    21291 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_option_field.py
+-rw-rw-rw-   0        0        0     3695 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/raster_images_saving_modes.py
+-rw-rw-rw-   0        0        0     6219 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/rectangle.py
+-rw-rw-rw-   0        0        0    18170 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotation.py
+-rw-rw-rw-   0        0        0     5794 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotation_response.py
+-rw-rw-rw-   0        0        0     4863 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotations.py
+-rw-rw-rw-   0        0        0     5834 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotations_response.py
+-rw-rw-rw-   0        0        0     3509 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/rotation.py
+-rw-rw-rw-   0        0        0    13011 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/row.py
+-rw-rw-rw-   0        0        0     5053 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/row_recognized.py
+-rw-rw-rw-   0        0        0    14148 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotation.py
+-rw-rw-rw-   0        0        0     5734 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotation_response.py
+-rw-rw-rw-   0        0        0     4815 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotations.py
+-rw-rw-rw-   0        0        0     5774 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotations_response.py
+-rw-rw-rw-   0        0        0     5085 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/segment.py
+-rw-rw-rw-   0        0        0     3507 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/shape_type.py
+-rw-rw-rw-   0        0        0    17074 2021-10-29 08:53:57.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature.py
+-rw-rw-rw-   0        0        0    15711 2023-06-29 05:39:11.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_custom_appearance.py
+-rw-rw-rw-   0        0        0    20192 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_field.py
+-rw-rw-rw-   0        0        0     5594 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_field_response.py
+-rw-rw-rw-   0        0        0     4783 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_fields.py
+-rw-rw-rw-   0        0        0     5634 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_fields_response.py
+-rw-rw-rw-   0        0        0     3523 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_type.py
+-rw-rw-rw-   0        0        0     5694 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/signature_verify_response.py
+-rw-rw-rw-   0        0        0    20322 2021-10-29 08:53:57.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotation.py
+-rw-rw-rw-   0        0        0     5714 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotation_response.py
+-rw-rw-rw-   0        0        0     4799 2023-06-29 05:39:14.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotations.py
+-rw-rw-rw-   0        0        0     5754 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotations_response.py
+-rw-rw-rw-   0        0        0     3524 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/sound_encoding.py
+-rw-rw-rw-   0        0        0     3474 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/sound_icon.py
+-rw-rw-rw-   0        0        0     4182 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/split_range_pdf_options.py
+-rw-rw-rw-   0        0        0     4200 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/split_result.py
+-rw-rw-rw-   0        0        0     8196 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/split_result_document.py
+-rw-rw-rw-   0        0        0     5554 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/split_result_response.py
+-rw-rw-rw-   0        0        0    17392 2023-06-29 05:39:17.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotation.py
+-rw-rw-rw-   0        0        0     5734 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotation_response.py
+-rw-rw-rw-   0        0        0     4815 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotations.py
+-rw-rw-rw-   0        0        0     5774 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotations_response.py
+-rw-rw-rw-   0        0        0    17057 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotation.py
+-rw-rw-rw-   0        0        0     5794 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotation_response.py
+-rw-rw-rw-   0        0        0     4867 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotations.py
+-rw-rw-rw-   0        0        0     5834 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotations_response.py
+-rw-rw-rw-   0        0        0    22009 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp.py
+-rw-rw-rw-   0        0        0    17904 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotation.py
+-rw-rw-rw-   0        0        0     5710 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotation_response.py
+-rw-rw-rw-   0        0        0     4799 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotations.py
+-rw-rw-rw-   0        0        0     5754 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotations_response.py
+-rw-rw-rw-   0        0        0    11543 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_base.py
+-rw-rw-rw-   0        0        0     3854 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_icon.py
+-rw-rw-rw-   0        0        0     9021 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_info.py
+-rw-rw-rw-   0        0        0     3522 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_type.py
+-rw-rw-rw-   0        0        0     4693 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamps_info.py
+-rw-rw-rw-   0        0        0     5520 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/stamps_info_response.py
+-rw-rw-rw-   0        0        0     4174 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7015 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/storage_file.py
+-rw-rw-rw-   0        0        0    17128 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotation.py
+-rw-rw-rw-   0        0        0     5794 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotation_response.py
+-rw-rw-rw-   0        0        0     4863 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotations.py
+-rw-rw-rw-   0        0        0     5834 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotations_response.py
+-rw-rw-rw-   0        0        0    23748 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/table.py
+-rw-rw-rw-   0        0        0     3531 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/table_broken.py
+-rw-rw-rw-   0        0        0     7133 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/table_recognized.py
+-rw-rw-rw-   0        0        0     5612 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/table_recognized_response.py
+-rw-rw-rw-   0        0        0     4777 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/tables_recognized.py
+-rw-rw-rw-   0        0        0     5652 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/tables_recognized_response.py
+-rw-rw-rw-   0        0        0    17854 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotation.py
+-rw-rw-rw-   0        0        0     5694 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotation_response.py
+-rw-rw-rw-   0        0        0     4783 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotations.py
+-rw-rw-rw-   0        0        0     5734 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotations_response.py
+-rw-rw-rw-   0        0        0    24062 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_field.py
+-rw-rw-rw-   0        0        0     5556 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_field_response.py
+-rw-rw-rw-   0        0        0     4753 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_fields.py
+-rw-rw-rw-   0        0        0     5596 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_fields_response.py
+-rw-rw-rw-   0        0        0    16535 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_footer.py
+-rw-rw-rw-   0        0        0    16469 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_header.py
+-rw-rw-rw-   0        0        0     3614 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_horizontal_alignment.py
+-rw-rw-rw-   0        0        0     3680 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_icon.py
+-rw-rw-rw-   0        0        0     5273 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_line.py
+-rw-rw-rw-   0        0        0    10182 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_rect.py
+-rw-rw-rw-   0        0        0     4041 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_rects.py
+-rw-rw-rw-   0        0        0     5711 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_rects_response.py
+-rw-rw-rw-   0        0        0     8530 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_replace.py
+-rw-rw-rw-   0        0        0     7087 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_replace_list_request.py
+-rw-rw-rw-   0        0        0     5621 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_replace_response.py
+-rw-rw-rw-   0        0        0    18248 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_stamp.py
+-rw-rw-rw-   0        0        0    11377 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_state.py
+-rw-rw-rw-   0        0        0     7403 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/text_style.py
+-rw-rw-rw-   0        0        0     5406 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/timestamp_settings.py
+-rw-rw-rw-   0        0        0    17128 2023-06-29 05:39:16.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotation.py
+-rw-rw-rw-   0        0        0     5794 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotation_response.py
+-rw-rw-rw-   0        0        0     4863 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotations.py
+-rw-rw-rw-   0        0        0     5834 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotations_response.py
+-rw-rw-rw-   0        0        0     3538 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/vertical_alignment.py
+-rw-rw-rw-   0        0        0     3978 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/word_count.py
+-rw-rw-rw-   0        0        0     5708 2023-06-29 05:39:15.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/word_count_response.py
+-rw-rw-rw-   0        0        0     3536 2023-06-29 05:39:12.000000 asposepdfcloud-23.6.0/asposepdfcloud/models/wrap_mode.py
+-rw-rw-rw-   0        0        0    14812 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/asposepdfcloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:22:35.551236 asposepdfcloud-23.6.0/asposepdfcloud.egg-info/
+-rw-rw-rw-   0        0        0     2869 2023-06-29 11:22:31.000000 asposepdfcloud-23.6.0/asposepdfcloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19197 2023-06-29 11:22:31.000000 asposepdfcloud-23.6.0/asposepdfcloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:22:31.000000 asposepdfcloud-23.6.0/asposepdfcloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-06-29 11:22:31.000000 asposepdfcloud-23.6.0/asposepdfcloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-29 11:22:31.000000 asposepdfcloud-23.6.0/asposepdfcloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 11:22:36.738754 asposepdfcloud-23.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     6037 2023-06-29 05:39:18.000000 asposepdfcloud-23.6.0/setup.py
```

### Comparing `asposepdfcloud-23.5.0/Examples/post_ink_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_ink_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_carret_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_carret_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_circle_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_circle_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_file_attachment_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_file_attachment_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_free_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_free_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_highlight_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_highlight_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_line_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_line_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_movie_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_movie_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_polygon_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_polygon_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_polyline_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_polyline_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_redaction_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_redaction_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_screen_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_screen_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_sound_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_sound_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_square_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_square_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_squiggly_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_squiggly_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_stamp_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_stamp_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_strikeout_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_strikeout_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_text_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_text_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_page_underline_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_page_underline_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/post_popup_annotations.py` & `asposepdfcloud-23.6.0/Examples/post_popup_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_carret_annotations.py` & `asposepdfcloud-23.6.0/Examples/put_carret_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_circle_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_circle_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_file_attachment_annotations.py` & `asposepdfcloud-23.6.0/Examples/put_file_attachment_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_free_text_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_free_text_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_hightlight_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_hightlight_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_ink_annotations.py` & `asposepdfcloud-23.6.0/Examples/put_ink_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_line_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_line_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_movie_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_movie_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_polyline_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_polyline_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_popup_annotations.py` & `asposepdfcloud-23.6.0/Examples/put_popup_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_redaction_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_redaction_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_screen_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_screen_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_sound_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_sound_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_square_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_square_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_squiggly_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_squiggly_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_stamp_annotations.py` & `asposepdfcloud-23.6.0/Examples/put_stamp_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_strikeout_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_strikeout_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_text_annotation.py` & `asposepdfcloud-23.6.0/Examples/put_text_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/Examples/put_underline_annotations.py` & `asposepdfcloud-23.6.0/Examples/put_underline_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/LICENSE` & `asposepdfcloud-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/PKG-INFO` & `asposepdfcloud-23.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposepdfcloud
-Version: 23.5.0
+Version: 23.6.0
 Summary: Aspose.PDF Cloud
 Home-page: https://products.aspose.cloud/pdf/cloud
 Author: Aspose PDF Cloud
 Author-email: 
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-pdf-cloud/aspose-pdf-cloud-python
 Project-URL: Website, https://www.aspose.cloud
```

### Comparing `asposepdfcloud-23.5.0/README.md` & `asposepdfcloud-23.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,21 @@
 
 ## Save PDF As
 XLS, XLSX, PPTX, DOC, DOCX, MobiXML, JPEG, EMF, PNG, BMP, GIF, TIFF, Text
 
 ## Read PDF Formats
 MHT, PCL, PS, XSLFO, MD
 
-## Enhancements in Version 23.5
+## Enhancements in Version 23.6
+- Support to convert password protected PDF documents to PPTX.
 - A new version of Aspose.PDF Cloud was prepared using the latest version of Aspose.PDF for .NET.
 
+## Bugs fixed in Version 23.6
+- Text Replacement API constantly hitting 504 Gateway Timeout.
+
 ## Requirements.
 Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
 If the python package is hosted on Github, you can install directly from Github
```

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/__init__.py` & `asposepdfcloud-23.6.0/asposepdfcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/api_client.py` & `asposepdfcloud-23.6.0/asposepdfcloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def __init__(self, app_key, app_sid, host=None):
         """
         Constructor of the class.
         """
         self.rest_client = RESTClientObject()
         self.default_headers = {}
         self.default_headers['x-aspose-client'] = 'python sdk'
-        self.default_headers['x-aspose-client-version'] = '23.5.0'
+        self.default_headers['x-aspose-client-version'] = '23.6.0'
         
         self.app_key = app_key
         self.app_sid = app_sid
 
         if host is None:
             self.host = Configuration().host
         else:
```

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/apis/__init__.py` & `asposepdfcloud-23.6.0/asposepdfcloud/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/apis/pdf_api.py` & `asposepdfcloud-23.6.0/asposepdfcloud/apis/pdf_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17313,14 +17313,15 @@
         :param callback function: The callback function
             for asynchronous request. (optional)
         :param str name: The document name. (required)
         :param bool separate_images: Separate images.
         :param bool slides_as_images: Slides as images.
         :param str folder: The document folder.
         :param str storage: The document storage.
+        :param str password: Base64 encoded password.
         :return: file
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('callback'):
             return self.get_pdf_in_storage_to_pptx_with_http_info(name, **kwargs)
@@ -17342,20 +17343,21 @@
         :param callback function: The callback function
             for asynchronous request. (optional)
         :param str name: The document name. (required)
         :param bool separate_images: Separate images.
         :param bool slides_as_images: Slides as images.
         :param str folder: The document folder.
         :param str storage: The document storage.
+        :param str password: Base64 encoded password.
         :return: file
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'separate_images', 'slides_as_images', 'folder', 'storage']
+        all_params = ['name', 'separate_images', 'slides_as_images', 'folder', 'storage', 'password']
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -17382,14 +17384,16 @@
             query_params.append(('separateImages', params['separate_images']))
         if 'slides_as_images' in params:
             query_params.append(('slidesAsImages', params['slides_as_images']))
         if 'folder' in params:
             query_params.append(('folder', params['folder']))
         if 'storage' in params:
             query_params.append(('storage', params['storage']))
+        if 'password' in params:
+            query_params.append(('password', params['password']))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -36916,14 +36920,15 @@
 
         :param callback function: The callback function
             for asynchronous request. (optional)
         :param str out_path: Full resulting filename (ex. /folder1/folder2/result.pptx) (required)
         :param bool separate_images: Separate images.
         :param bool slides_as_images: Slides as images.
         :param str storage: The document storage.
+        :param str password: Base64 encoded password.
         :param file file: A file to be converted.
         :return: AsposeResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('callback'):
@@ -36945,21 +36950,22 @@
 
         :param callback function: The callback function
             for asynchronous request. (optional)
         :param str out_path: Full resulting filename (ex. /folder1/folder2/result.pptx) (required)
         :param bool separate_images: Separate images.
         :param bool slides_as_images: Slides as images.
         :param str storage: The document storage.
+        :param str password: Base64 encoded password.
         :param file file: A file to be converted.
         :return: AsposeResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['out_path', 'separate_images', 'slides_as_images', 'storage', 'file']
+        all_params = ['out_path', 'separate_images', 'slides_as_images', 'storage', 'password', 'file']
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -36984,14 +36990,16 @@
             query_params.append(('outPath', params['out_path']))
         if 'separate_images' in params:
             query_params.append(('separateImages', params['separate_images']))
         if 'slides_as_images' in params:
             query_params.append(('slidesAsImages', params['slides_as_images']))
         if 'storage' in params:
             query_params.append(('storage', params['storage']))
+        if 'password' in params:
+            query_params.append(('password', params['password']))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
         if 'file' in params:
             local_var_files['file'] = params['file']
@@ -38677,14 +38685,15 @@
             for asynchronous request. (optional)
         :param str name: The document name. (required)
         :param str out_path: Full resulting filename (ex. /folder1/folder2/result.pptx) (required)
         :param bool separate_images: Separate images.
         :param bool slides_as_images: Slides as images.
         :param str folder: The document folder.
         :param str storage: The document storage.
+        :param str password: Base64 encoded password.
         :return: AsposeResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('callback'):
             return self.put_pdf_in_storage_to_pptx_with_http_info(name, out_path, **kwargs)
@@ -38707,20 +38716,21 @@
             for asynchronous request. (optional)
         :param str name: The document name. (required)
         :param str out_path: Full resulting filename (ex. /folder1/folder2/result.pptx) (required)
         :param bool separate_images: Separate images.
         :param bool slides_as_images: Slides as images.
         :param str folder: The document folder.
         :param str storage: The document storage.
+        :param str password: Base64 encoded password.
         :return: AsposeResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name', 'out_path', 'separate_images', 'slides_as_images', 'folder', 'storage']
+        all_params = ['name', 'out_path', 'separate_images', 'slides_as_images', 'folder', 'storage', 'password']
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -38752,14 +38762,16 @@
             query_params.append(('separateImages', params['separate_images']))
         if 'slides_as_images' in params:
             query_params.append(('slidesAsImages', params['slides_as_images']))
         if 'folder' in params:
             query_params.append(('folder', params['folder']))
         if 'storage' in params:
             query_params.append(('storage', params['storage']))
+        if 'password' in params:
+            query_params.append(('password', params['password']))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/configuration.py` & `asposepdfcloud-23.6.0/asposepdfcloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,9 +195,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 23.5.0".\
+               "SDK Package Version: 23.6.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/__init__.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_flags.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_flags.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_state.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_state.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotation_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotation_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotations_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotations_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/annotations_info_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/annotations_info_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/antialiasing_processing_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/antialiasing_processing_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/aspose_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/aspose_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/attachment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/attachment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/attachment_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/attachment_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/attachments.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/attachments.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/attachments_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/attachments_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/bookmark.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/bookmark_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/bookmark_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/bookmarks.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/bookmarks.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/bookmarks_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/border.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/border.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/border_corner_style.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/border_corner_style.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/border_effect.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/border_effect.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/border_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/border_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/border_style.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/border_style.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/box_style.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/box_style.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/cap_style.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/cap_style.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/caption_position.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/caption_position.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/caret_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/caret_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/caret_symbol.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/caret_symbol.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/cell.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/cell.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/cell_recognized.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/cell_recognized.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/check_box_fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/check_box_fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/choice_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/choice_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/circle_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/circle_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/color.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/color.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/color_depth.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/color_depth.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/column_adjustment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/column_adjustment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/combo_box_fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/combo_box_fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/common_figure_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/common_figure_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/compression_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/compression_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/crypto_algorithm.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/crypto_algorithm.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/dash.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/dash.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/default_page_config.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/default_page_config.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/direction.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/direction.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/disc_usage.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/display_properties.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/display_properties.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/display_properties_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/display_properties_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/doc_format.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/doc_format.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/doc_mdp_access_permission_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/doc_mdp_access_permission_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/doc_recognition_mode.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/doc_recognition_mode.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_config.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_config.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_page_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_page_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_pages_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_pages_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_privilege.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_privilege.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_properties.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_properties_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_properties_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_property.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_property_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_property_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/document_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/document_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/epub_recognition_mode.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/epub_recognition_mode.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/error.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/error_details.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/field_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/field_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_attachment_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_attachment_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_icon.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_icon.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_version.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/file_versions.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/files_list.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/files_upload_result.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/font_encoding_rules.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/font_encoding_rules.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/font_saving_modes.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/font_saving_modes.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/font_styles.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/font_styles.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/form_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/form_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/free_text_intent.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/free_text_intent.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/graph_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/graph_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/highlight_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/highlight_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/horizontal_alignment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/horizontal_alignment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/html_document_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/html_document_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/html_markup_generation_modes.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/html_markup_generation_modes.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_compression_version.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_compression_version.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_encoding.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_encoding.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_footer.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_footer.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_fragment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_fragment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_header.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_header.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_src_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_src_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_stamp.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_stamp.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_template.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_template.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/image_templates_request.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/image_templates_request.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/images.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/images_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/images_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/ink_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/ink_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/justification.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/justification.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/letters_positioning_methods.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/letters_positioning_methods.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_ending.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_ending.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_intent.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_intent.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/line_spacing.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/line_spacing.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_action_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_action_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_element.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/link_highlighting_mode.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/link_highlighting_mode.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/list_box_fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/list_box_fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/margin_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/margin_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/markup_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/markup_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/merge_documents.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/merge_documents.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/movie_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/movie_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/object_exist.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/optimize_options.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/optimize_options.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/option.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/option.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/organize_document_data.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/organize_document_data.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/organize_document_request.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/organize_document_request.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/output_format.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/output_format.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/page.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/page.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/page_layout.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/page_layout.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/page_mode.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/page_mode.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/page_number_stamp.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/page_number_stamp.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/page_range.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/page_range.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/page_word_count.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/page_word_count.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/pages.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/pages.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/paragraph.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/parts_embedding_modes.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/parts_embedding_modes.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/pdf_a_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/pdf_a_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/pdf_page_stamp.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/pdf_page_stamp.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/permissions_flags.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/permissions_flags.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/point.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/point.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/poly_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/poly_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/poly_intent.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/poly_intent.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/poly_line_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/poly_line_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/polygon_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/polygon_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotation_with_parent.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotation_with_parent.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/popup_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/popup_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/position.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/position.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/radio_button_option_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/radio_button_option_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/raster_images_saving_modes.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/raster_images_saving_modes.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/rectangle.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/rectangle.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/redaction_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/redaction_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/rotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/rotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/row.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/row.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/row_recognized.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/row_recognized.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/screen_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/screen_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/segment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/segment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/shape_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_custom_appearance.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_custom_appearance.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/signature_verify_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/signature_verify_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/sound_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/sound_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/sound_encoding.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/sound_encoding.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/sound_icon.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/sound_icon.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/split_range_pdf_options.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/split_range_pdf_options.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/split_result.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/split_result.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/split_result_document.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/split_result_document.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/split_result_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/split_result_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/square_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/square_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/squiggly_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/squiggly_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_base.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_base.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_icon.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_icon.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamp_type.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamp_type.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamps_info.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamps_info.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/stamps_info_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/stamps_info_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/storage_exist.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/storage_file.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/strike_out_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/strike_out_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/table.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/table.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/table_broken.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/table_broken.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/table_recognized.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/table_recognized.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/table_recognized_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/table_recognized_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/tables_recognized.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/tables_recognized.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/tables_recognized_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/tables_recognized_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_field.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_field.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_field_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_field_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_fields.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_fields.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_box_fields_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_box_fields_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_footer.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_footer.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_header.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_header.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_horizontal_alignment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_horizontal_alignment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_icon.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_icon.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_line.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_line.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_rect.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_rect.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_rects.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_rects.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_rects_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_rects_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_replace.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_replace.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_replace_list_request.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_replace_list_request.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_replace_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_stamp.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_stamp.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_state.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_state.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/text_style.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/text_style.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/timestamp_settings.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/timestamp_settings.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotation.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotation.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotation_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotation_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotations.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotations.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/underline_annotations_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/underline_annotations_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/vertical_alignment.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/vertical_alignment.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/word_count.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/word_count.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/word_count_response.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/word_count_response.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/models/wrap_mode.py` & `asposepdfcloud-23.6.0/asposepdfcloud/models/wrap_mode.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud/rest.py` & `asposepdfcloud-23.6.0/asposepdfcloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud.egg-info/PKG-INFO` & `asposepdfcloud-23.6.0/asposepdfcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposepdfcloud
-Version: 23.5.0
+Version: 23.6.0
 Summary: Aspose.PDF Cloud
 Home-page: https://products.aspose.cloud/pdf/cloud
 Author: Aspose PDF Cloud
 Author-email: 
 License: MIT
 Project-URL: Source With Tests, https://github.com/aspose-pdf-cloud/aspose-pdf-cloud-python
 Project-URL: Website, https://www.aspose.cloud
```

### Comparing `asposepdfcloud-23.5.0/asposepdfcloud.egg-info/SOURCES.txt` & `asposepdfcloud-23.6.0/asposepdfcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asposepdfcloud-23.5.0/setup.py` & `asposepdfcloud-23.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "asposepdfcloud"
-VERSION = "23.5.0"
+VERSION = "23.6.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

