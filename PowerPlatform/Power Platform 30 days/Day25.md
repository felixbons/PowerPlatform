
# Day 25 – PDF Generation, Emails, and Attachments Using Power Automate

---

## 📝 Overview

Power Automate allows you to automate document generation, send emails with dynamic content, and include attachments. With built-in and third-party connectors, you can generate PDFs from HTML or data, attach them to emails, and streamline approvals or document delivery processes.

In this session, you’ll create a flow that generates a PDF, sends it via email, and attaches files from SharePoint or OneDrive.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Prepare Your Content

- Have a sample **HTML file** or **template** ready
- Prepare dynamic data (e.g., form fields, Dataverse rows)
- Optional: Store files in SharePoint or OneDrive

---

### ✅ Step 2: Generate PDF (3 Options)

**Option A: Word + OneDrive (No Premium)**
1. Upload a Word file with content controls (placeholders)
2. Use **Populate a Microsoft Word template** (OneDrive)
3. Add **Convert Word Document to PDF**

**Option B: HTML to PDF with 3rd-party (e.g., Encodian, Muhimbi)**
1. Use **HTML content** with dynamic data
2. Pass it to the PDF generator action
3. Store result in SharePoint or OneDrive

**Option C: Create File + Convert File**
1. Use **Create File** action (OneDrive or SharePoint)
2. Add **Convert File (Preview)** to PDF
3. Save or email the output

---

### ✅ Step 3: Send Email with Attachment

1. Add action: **Send an email (V2)** (Outlook or Gmail)
2. Fill:
   - To: Dynamic or static address
   - Subject: `Your Report is Ready`
   - Body: Include dynamic content or custom text
3. Attach the PDF:
   - **File Content**: Use from previous PDF step
   - **File Name**: `Report.pdf`

---

### ✅ Step 4: Optional – Store Attachment in SharePoint

1. Use **Create file**
2. Choose a document library
3. Set file name and content using dynamic outputs

---

### ✅ Step 5: Test the Flow

1. Trigger the flow manually or via a form submission
2. Check email and attachment
3. Verify PDF is correctly formatted and accessible

---

## 🔎 What You Should Try Today

- Generate a PDF using Word or HTML
- Send a dynamic email with a PDF attachment
- Store the attachment in SharePoint or OneDrive
- Use conditions to only send if criteria are met

---

## 🔁 Navigation

⬅️ [**Go to Day 24: Custom Connectors – consume external APIs in Power Apps**](/PowerPlatform/Power%20Platform%2030%20days/Day24.md)  
➡️ [**Go to Day 26: Power BI + Power Platform – embed reports into your apps**](/PowerPlatform/Power%20Platform%2030%20days/Day26.md)
