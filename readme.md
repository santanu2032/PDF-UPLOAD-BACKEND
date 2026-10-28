# CSE CYS 1 (32-64) PDF Upload Portal

A public web portal designed for the Computer Science and Engineering (Cyber Security) CYS 1 cohort at Guru Nanak Institute of Technology. This tool allows students (Roll 32–64) to easily upload their assignment PDFs directly to a centralized Google Drive folder without requiring any Google login.

## Features
* **Anonymous 1-Click Uploads:** No Google account sign-in required for students.
* **Automatic File Naming:** Enforces a strict `RollNo_Name_Document.pdf` naming convention to keep submissions organized.
* **Direct Drive Integration:** Uploads go straight to the designated Google Drive folder via a Google Apps Script backend.
* **Responsive UI:** Simple, drag-and-drop interface.

## System Architecture
This project consists of two parts:
1. **Frontend (`index.html`):** A static HTML/JS web page hosted on GitHub Pages.
2. **Backend (Google Apps Script):** A serverless `doPost` endpoint attached to the destination Google Drive folder.

## Setup Instructions

### 1. Backend (Google Apps Script)
1. Go to [script.google.com](https://script.google.com/) and create a **New project**.
2. Paste the provided backend code into the editor.
3. Replace the `FOLDER_ID` variable with your target Google Drive folder ID.
4. Click **Deploy > New deployment**.
5. Select **Web app**.
6. Set **Execute as** to `Me` and **Who has access** to `Anyone`.
7. Click **Deploy** and authorize the script to access your Google Drive.
8. Copy the generated **Web app URL**.

### 2. Frontend Configuration
1. Open `index.html` in your local environment.
2. Paste the **Web app URL** generated from the step above into the frontend configuration.
3. Push the repository to GitHub.

### 3. Hosting (GitHub Pages)
1. Navigate to your repository settings on GitHub.
2. Go to **Pages** under the "Build and deployment" section.
3. Select the `main` branch as the source and click **Save**.
4. Share the generated GitHub Pages live link with the class.

## License
This project is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).

---
*Maintained by Santanu Sarkar, Class Representative (CYS 1)*