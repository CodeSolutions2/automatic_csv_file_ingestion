# automatic_csv_file_ingestion

Automatic csv file ingestion: sorting of files by header, upload to cloud

The objective of this work was to create an automated bash script that sorts a folder of csv files, using the header name of the csv files. This project was for the final project of the Google Analytics Coursera Certification program (github.com/j622amilah/Case_Studies/tree/main/1_case_study_bikeshare). The bash code first reads in an initial header and labels this the current_header, it reads in each csv file and compares the new csv file header with the current_header. Each word/header in the current_header is compared with each word/header in the new csv file header, using both lexical matching and word similarity via a REST API Hugging Face model. Sufficiently similar words/headers in the new csv file are replaced by the equivalent word/header in the current_header. Once all the header words are compared, if the new csv file has the same header as the current_header it is moved to a folder called exact_match_header. If the new csv file has at least one header word that matches the current_header, the new csv file is moved to a folder called similar_match_header. If no header words match the current_header, it is moved to a folder called no_match_header.

In summary, a function that will organize a folder of csv files into three folders: exact_match_header, similar_match_header, no_match_header. The exact_match_header files all have the same common header, so they can be uploaded directly to a cloud server.

[Available for purchase on Upwork] (https://www.upwork.com/services/product/development-it-automatic-csv-file-ingestion-sorting-of-files-by-header-upload-to-cloud-1740355723544662016)
