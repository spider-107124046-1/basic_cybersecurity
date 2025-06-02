# Google Dork-Based Asset Discovery

## Target: **[tesla.com](https://tesla.com)**

### Public Documents (PDF, XLSX, DOCX,etc)

#### `site:tesla.com filetype:pdf` 

Normally searching for PDFs with the base domain will return many manuals, guides, and detail sheets in many languages, as expected. Most notable results out of those come from the subdomains service.tesla.com and ir.tesla.com

service.tesla.com mentions:

> All users with a Tesla Account can browse published catalogs for their country, for the following information: Diagrams, Part Numbers/Descriptions, Sales Requirements

#### But, `site:service.tesla.com filetype:pdf` fetches a lot of those diagrams and part descriptions

![image](https://github.com/user-attachments/assets/88d21359-2848-40da-989e-bb52cebedd96)

Some links:
- [https://service.tesla.com/docs/ModelY/ElectricalReference/prog-52/interactive/pdf/index_print.pdf](https://service.tesla.com/docs/ModelY/ElectricalReference/prog-52/interactive/pdf/index_print.pdf)
- [https://service.tesla.com/docs/Public/epc/UserGuide/SPEC_EXT_137658-00-D_01_SUMITOMO_TO_RJ45.pdf](https://service.tesla.com/docs/Public/epc/UserGuide/SPEC_EXT_137658-00-D_01_SUMITOMO_TO_RJ45.pdf)
- [https://service.tesla.com/docs/ModelS/ElectricalReference2012/s-lhd-sop9/2016.3_ModelS_LHD_Release.pdf](https://service.tesla.com/docs/ModelS/ElectricalReference2012/s-lhd-sop9/2016.3_ModelS_LHD_Release.pdf)

ir.tesla.com is their Investor Relations site. It has a lot of information about their investors.

#### The documents that `site:ir.tesla.com filetype:pdf` fetches don't seem to be accessible directly on the site, atleast on face value.

![image](https://github.com/user-attachments/assets/b7b7c35d-d9ef-4a2d-ba2c-c2219921186d)

Some links:
- [https://ir.tesla.com/_flysystem/s3/sec/000195004724008368/000195004724008368-gen.pdf](https://ir.tesla.com/_flysystem/s3/sec/000195004724008368/000195004724008368-gen.pdf)
- [https://ir.tesla.com/_flysystem/s3/sec/000177136423000001/000177136423000001-gen.pdf](https://ir.tesla.com/_flysystem/s3/sec/000177136423000001/000177136423000001-gen.pdf)
- [https://ir.tesla.com/_flysystem/s3/sec/000083423722009097/us88160r1014_031122-gen.pdf](https://ir.tesla.com/_flysystem/s3/sec/000083423722009097/us88160r1014_031122-gen.pdf)

#### `site:tesla.com filetype:xlsx`

![image](https://github.com/user-attachments/assets/2a44b678-43f0-4b1d-82f8-c402a02b1c06)

Links:
- [https://service.tesla.com/docs/ServiceBulletins/External/SB/Damper_Sort5081_1027461-00-G_v2_(1).xlsx](https://service.tesla.com/docs/ServiceBulletins/External/SB/Damper_Sort5081_1027461-00-G_v2_(1).xlsx)
- [https://service.tesla.com/docs/ServiceBulletins/External/SB/Damper_PN_Checker_For_SB-20-31-004_and_005.xlsx](https://service.tesla.com/docs/ServiceBulletins/External/SB/Damper_PN_Checker_For_SB-20-31-004_and_005.xlsx)
- [https://service.tesla.com/docs/ServiceBulletins/External/SB/CLAIM_FORM_DEALER_EN_foam_detachment_Model_Y.xlsx](https://service.tesla.com/docs/ServiceBulletins/External/SB/CLAIM_FORM_DEALER_EN_foam_detachment_Model_Y.xlsx)
- [https://service.tesla.com/docs/ServiceBulletins/External/SB/CLAIM_FORM_DEALER_EN_foam_detachment_Model_3.xlsx](https://service.tesla.com/docs/ServiceBulletins/External/SB/CLAIM_FORM_DEALER_EN_foam_detachment_Model_3.xlsx)

Seems to be two forms, a protected product number lookup sheet, and a list of serial numbers whose dampers are suspected to be defective

![image](https://github.com/user-attachments/assets/b13dfb92-f87e-47d6-a67f-59b8fc23659d)

#### `site:tesla.com filetype:docx`

![image](https://github.com/user-attachments/assets/c1c4b9e3-5199-4c46-983d-a7ef9e67172a)

Some letter templates, and surveys, in different languages:
- [https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/2-Widerspruch-gegen-Aufhebung.docx](https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/2-Widerspruch-gegen-Aufhebung.docx)
- [https://www.tesla.com/sites/default/files/downloads/en_HK/apartment_residents_survey_EN_HK_2.docx](https://www.tesla.com/sites/default/files/downloads/en_HK/apartment_residents_survey_EN_HK_2.docx)
- [https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/A-umwelt.docx](https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/A-umwelt.docx)
- [https://digitalassets.tesla.com/tesla-contents/raw/upload/EV_Installation_HOA_Request.docx](https://digitalassets.tesla.com/tesla-contents/raw/upload/EV_Installation_HOA_Request.docx)

#### PPT(X) files were not found.

#### `site:tesla.com filetype:txt` returns the site's robots.txt and a file called security.txt containing information on where to report vulnerabilities.

![image](https://github.com/user-attachments/assets/e8ab5b79-f0c6-4169-9dde-d8216c8338c4)

#### `site:tesla.com filetype:csv`

![image](https://github.com/user-attachments/assets/a3dd983b-2377-43bf-910a-a1e298459e1d)

The pricebook is a json file with csv extension. The next two links seem to be some sort of hourly electricity demand profile. The last one is interesting, it has a list of all possible error codes given by their diagnostic tool.

Links:
- [https://www.tesla.com/configurator/pricebook?pricebook=MS_US](https://www.tesla.com/configurator/pricebook?pricebook=MS_US)
- [https://www.tesla.com/sites/default/files/downloads/US-fully-electrified-demand-profile-part-2.csv](https://www.tesla.com/sites/default/files/downloads/US-fully-electrified-demand-profile-part-2.csv)
- [https://www.tesla.com/sites/default/files/downloads/US-fully-electrified-demand-profile-part-1.csv](https://www.tesla.com/sites/default/files/downloads/US-fully-electrified-demand-profile-part-1.csv)
- [https://fleet-api-files-prd.tesla.com/alert_dictionary.csv](https://fleet-api-files-prd.tesla.com/alert_dictionary.csv)

#### Generalising the search with something like `site:tesla.com inurl:download` yields agreements:

![image](https://github.com/user-attachments/assets/ff61e915-237a-4fb9-8c80-8662c6808183)

The notable results from partners.tesla.com and toolbox.tesla.com are properly gatekept by a login page. Even all results from `site:partners.tesla.com` and `site:toolbox.tesla.com` are inaccessible.

![image](https://github.com/user-attachments/assets/3d1b4345-fcc2-46b0-b361-074ae68b4933)

#### `site:tesla.com inurl:content` yields more manuals and... job openings! (many links now return 404) :( 

![image](https://github.com/user-attachments/assets/50de001f-32ce-43d1-9bb0-40757cea56e8)

### Login Pages / Admin Panels
### Public Backup / Config Files
### Exposed Logs / Errors
### Emails & Contact Info
### Git Folders and Env Files
