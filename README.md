# Google Dork-Based Asset Discovery

## Target: **[tesla.com](https://tesla.com)**

### Public Documents (PDF, XLSX, DOCX, etc.,)

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

`site:tesla.com ext:ods` gives bing chilling (as the only result) [https://www.tesla.com/sites/default/files/downloads/zh_TW/%E5%A0%B1%E5%BB%A2%E6%8F%9B%E6%96%B0%E8%BB%8A%E6%98%8E%E7%B4%B0%E8%A1%A8.ods](https://www.tesla.com/sites/default/files/downloads/zh_TW/%E5%A0%B1%E5%BB%A2%E6%8F%9B%E6%96%B0%E8%BB%8A%E6%98%8E%E7%B4%B0%E8%A1%A8.ods)

#### `site:tesla.com filetype:docx`

![image](https://github.com/user-attachments/assets/c1c4b9e3-5199-4c46-983d-a7ef9e67172a)

Some letter templates, and surveys, in different languages:
- [https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/2-Widerspruch-gegen-Aufhebung.docx](https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/2-Widerspruch-gegen-Aufhebung.docx)
- [https://www.tesla.com/sites/default/files/downloads/en_HK/apartment_residents_survey_EN_HK_2.docx](https://www.tesla.com/sites/default/files/downloads/en_HK/apartment_residents_survey_EN_HK_2.docx)
- [https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/A-umwelt.docx](https://www.tesla.com/sites/default/files/support/Ihr-Umweltbonus/A-umwelt.docx)
- [https://digitalassets.tesla.com/tesla-contents/raw/upload/EV_Installation_HOA_Request.docx](https://digitalassets.tesla.com/tesla-contents/raw/upload/EV_Installation_HOA_Request.docx)

`site:tesla.com filetype:odt OR filetype:fodt` returned 0 results

#### `site:tesla.com filetype:ppt OR filetype:pptx OR filetype:odp OR filetype:fodp` PPT(X)/ODP files were not found.

#### `site:tesla.com ext:md` Markdown files were not found

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

`site:tesla.com inurl:admin` - no result (ie., no portals/panels found)

`site:tesla.com inurl:login` - yields publicly accessible Tesla account login portals (like the gatekeeping one aforementioned). Additionally, this gives results from [feedback.tesla.com](https://feedback.tesla.com/login) that leads to Tesla's Microsoft adfs and organization account login portals:

![image](https://github.com/user-attachments/assets/bb50d391-08c4-46ed-990f-9c24de6f51fb)
![image](https://github.com/user-attachments/assets/1ed01575-5099-4ef1-9d54-f7ec80256c0e)
![image](https://github.com/user-attachments/assets/30695e4a-abb7-4a8d-a2b8-a204b7e288f8)

`site:feedback.tesla.com` gives [one feedback form](https://feedback.tesla.com/jfe/form/SV_ea4r6Mwcc3aXVBk) and the rest lead to the same identity provider select link shown above.

`site:tesla.com intitle:"login"`, `site:tesla.com intitle:"panel"`, `site:tesla.com inurl:"panel"`, `site:tesla.com intitle:"portal"`, `site:tesla.com inurl:"portal"` all yield results already seen/irreleveant results.

`site:tesla.com inurl:dashboard` fetches some unique endpoints:

![image](https://github.com/user-attachments/assets/48415023-f137-48bd-88fb-be3c36a820ab)

The inside.tesla.com/en-US/learning/dashboard site redirects to the Microsoft Account login page for Tesla organization, the warp.tesla.com/dashboard site redirects to the older Microsoft Active Directory Federation Services (adfs) login page.

`site:tesla.com inurl:auth` fetches more endpoints:

![image](https://github.com/user-attachments/assets/966f2fda-e528-4a4d-aec5-df38c2fa92f7)
![image](https://github.com/user-attachments/assets/9fd8e021-0ac4-493c-a6d6-77eb5999fb5a)
![image](https://github.com/user-attachments/assets/330f1a6f-973c-4bc5-a340-532abee21ec3)

All of which redirect to auth.tesla.com (Tesla account login page)

### Public Backup / Config Files

`site:tesla.com intitle:"index of"` yields nothing (aimed at finding directory listings like this: [https://docs.oasis-open.org/](https://docs.oasis-open.org/)]

`site:tesla.com inurl:old` yields one result: [https://tesla.com/en_MY/support/referral-program-old](https://tesla.com/en_MY/support/referral-program-old)

`site:tesla.com inurl:test` shows results about test drives, and not any leftover test directories on site.

`site:tesla.com inurl:dev` yields one new endpoint that also points to the ADFS login page. Other than that, nothing of interest.

![image](https://github.com/user-attachments/assets/1d0a33da-7174-48d5-ae73-379dd6a07615)

`site:tesla.com inurl:"prod"` fetches two seemingly broken pages, which look like the page you will get after you sign in (judging by the `'s Tesla`, which looks like it takes a name before it, and the account management options)

- [https://www.tesla.com/ko_KR/teslaaccount/prod](https://www.tesla.com/ko_KR/teslaaccount/prod)
- [https://www.tesla.com/fr_CA/teslaaccount/prod](https://www.tesla.com/fr_CA/teslaaccount/prod)

![image](https://github.com/user-attachments/assets/5577f3e7-a7a7-4ee1-8fc7-85ceeaeb3419)
![image](https://github.com/user-attachments/assets/290f795a-9f8a-46a4-a4b4-0d5ab230d6e9)

This page doesn't exist in other languages (say, en_US. It returns 404)

`site:tesla.com inurl:"config"` yields just one result, which seems to be the subscription agreement that will be displayed when you try to sign up for "Drive Anywhere" on a Tesla app: [https://www.tesla.com/app-assets-config/pdf/Drive_Anywhere_Agreement.pdf](https://www.tesla.com/app-assets-config/pdf/Drive_Anywhere_Agreement.pdf)

`site:tesla.com (ext:env OR ext:yml OR ext:yaml OR ext:toml OR ext:config OR ext:conf OR ext:xml)` returns 0 results. *Clean*

`site:tesla.com "api"` returned many things about their Fleet API, but going to the 6th or 7th page of the result, we start seeing PDF files regarging Damage Disclosure

![image](https://github.com/user-attachments/assets/dc0cf142-baca-4099-a63d-f3c0b4973e39)


![image](https://github.com/user-attachments/assets/5692506a-e6e5-4f21-b6cc-aaae60f47850)

These PDFs do not seem to have personally identifiable information other than the vehicle serial numbers.

### Exposed Logs / Errors

`site:tesla.com filetype:log` - 0 results.

`site:tesla.com inurl:"log"` - "Log Technician, Field Reliability Engineering"

![image](https://github.com/user-attachments/assets/1ffa2cd8-8852-41f7-840c-3aaca07a8cc9)

`site:tesla.com inurl:"logs"` - a single press release and nothing else

![image](https://github.com/user-attachments/assets/047518af-4077-4bf9-9258-89ba57fb7f8e)

`site:tesla.com inurl:error` - Gives login error pages in many locales

![image](https://github.com/user-attachments/assets/06d793af-b871-491c-a851-48de3c8ab087)

`site:tesla.com "stacktrace"` - 0 results.

`site:tesla.com "promise"` (result of an asynchronous operation in js) - very mysterious result that redirects to tesla account login page: [https://tesla.com/en_NZ/file/son-man-promise-familyjpg](https://tesla.com/en_NZ/file/son-man-promise-familyjpg)

![image](https://github.com/user-attachments/assets/6dab25a0-2c2c-4fc9-a63e-7998cb82a1e2)

Other than that its all results about their empty promises to customers.

### Emails & Contact Info

`site:tesla.com intext:"email"` We have many regional service phone lines and email addresses in the search results. This is publicly available information and is of no interest to us (unless we are making a very useless excel sheet of all tesla support regions and email addresses.) 

![image](https://github.com/user-attachments/assets/6894e119-731c-4b15-9739-9bb539ccaeae)

If we go back to our ir.tesla.com subdomain, we'll get TONS of contact info from all the investor documentation, letters and legal documents on there. I will attach screenshots of a few. As it is out of the scope of this exercise, I won't be opening any of those PDFs to search for contacts. I will only post screenshots here of indexed search results.

`site:ir.tesla.com filetype:pdf email OR Contact`

![image](https://github.com/user-attachments/assets/7892d1bc-53fb-4442-aeb6-e49b8c230fa0)

![image](https://github.com/user-attachments/assets/7111fbd4-ffa8-4c1f-a5e3-7c61d99dacb8)

![image](https://github.com/user-attachments/assets/c8078d59-3d4f-4e28-88bf-c29856ddfc97)

![image](https://github.com/user-attachments/assets/dc703fd3-227a-4234-9eca-3fd80d4aa208)

![image](https://github.com/user-attachments/assets/a06de790-6026-4759-b2c6-9d5ebd6c2245)

### Git Folders and Env Files

`site:tesla.com ext:env` as we've already seen, returns 0 results.

`site:tesla.com "src"` no relevant results

`site:tesla.com inurl:repo OR inurl:repository` 0 results

`site:tesla.com inurl:git` 0 results

`site:tesla.com ext:py OR ext:c OR ext:java OR ext:rs OR ext:js OR ext:kt` well we tried

`site:tesla.com ".git" OR ".gitignore" OR ".svn"` pulls stuff from Fleet API documentation. No leaked source code here

If you really think about it, the whole site is still open source ¯\\\_(ツ)_/¯

![ezgif-4b8a3e47d34ef3](https://github.com/user-attachments/assets/09672ad9-6ea8-4699-bd85-ad8427882feb)
