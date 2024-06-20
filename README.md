# Download All Links From A Page

This repo showcase how my colleagues and I work on this site: https://www.arcweb.com/clients/reports, to get all the pdf downloaded into local device.
Due to urgency of this project, the method provided below is not optimized.

### You need: 
1. Chrome Browser
2. Chrome Extension by Nils Maier, https://chromewebstore.google.com/detail/downthemall/nljkibfhlpcnanjgbnlnbjecgicbjkge
3. HTML Editor

## A) Identify Objective
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
- 
### Step 2 - Extension Settings
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

  ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/366c076f-7ee8-4dda-a492-c20e16b25c1f)

- Open HTML editor (I use _VS Code_), and then paste the code into `<body> ... </body>` from a blank HTML canvas.
- Here is a blank HTML generated by ChatGPT: 
  ```
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
      <style>
          /* Add your CSS styling here */
      </style>
  </head>
  <body>

      <!-- Add your HTML content here -->

  </body>
  </html>
  ```

  - Save the file as 'Document.html'.
    
    ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/39b7e149-a2b0-44f3-a8bd-726e77266317)

  - Click and run the HTML file. It should be something like this:

    ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/0d89f85e-62d1-473c-812a-18504b2e7ff3)

  ### Step 4 - Conver Internal Links to External
  - In the HTML editor, press `Ctrl + F` on windows.
  - Search `/clients`.
  - Click the down arrow on the left.
  - Replace the word `https://www.arcweb.com/clients`.
 
    ![image](https://github.com/CPJ03/download-all-links-from-a-page/assets/88066484/797e1958-2c04-4caf-a132-da0fdeaf1016)

  - `Ctrl + S` to save the file
  - Reload the site and all the links should works.
    
  ### Step 5 - Open all the links
  - Open all the links by clicking the scroll wheel on the links.
    


