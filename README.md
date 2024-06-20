# Download All Links From A Page

This repo showcase how my colleagues and I work on this site: https://www.arcweb.com/clients/reports, to get all the pdf downloaded into local device.
Due to urgency of this project, the method provided below is not optimized.

## Tools/Code include:
1. Chrome Browser
2. Chrome Extension by Nils Maier, https://chromewebstore.google.com/detail/downthemall/nljkibfhlpcnanjgbnlnbjecgicbjkge
3. HTML

## A) IDENTIFY OBJECTIVE
Our goal is to download all the pdf files from the web based on catogories/filter
![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/c39120bd-acdf-4a31-b59e-74c71a00d268)

## B) Problems
1. There are thousand of documets to be downloaded. 
2. The website required authentication for downloading report purposes.
3. The href links in the source code are internal links.

## C) Solution
### Step 1 - Install Chrome Extension
- Open Google Chrome
- Go to https://chromewebstore.google.com/detail/downthemall/nljkibfhlpcnanjgbnlnbjecgicbjkge and click 'Add to Chrome'.
- Click 'Add extension' in the popup. 
### Step 2 - Allow 
- Go to upper right corner in google chrome where there is a puzzle icon.
  
   ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/15eecfb0-3d43-46a6-91e4-5d4636e6e53a)
 
- Click three dots beside the extension.
- Click 'Manage Extension'.
  
  ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/16404c8b-31fd-446d-9bed-b12ce9648f48)

- Enable 'Allow access to file URLs'
  
  ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/cb730de5-e391-414f-bff3-9ec2c766425c)

### Step 3 - Create HTML lists
- Go to https://www.arcweb.com/clients/reports.
- Log in account.
- Filter files needed using filter panel on the left. Remember to click 'Apply'. 

  ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/e23ffb93-b30d-43e8-a397-a88cda67fee1)

- On Page 1, right click -> 'View page source'
- Scroll until you find the `<table>` tags
- Copy the whole `<table> ... </table>` tags

  ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/f14b05f2-6034-4ec1-8e01-6193c5c377bc)

- 

