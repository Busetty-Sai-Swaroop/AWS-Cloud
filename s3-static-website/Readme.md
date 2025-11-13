# Static Website Hosting on Amazon S3

This document provides a complete guide to hosting a static website using Amazon S3. It covers bucket creation, uploading files, configuring ACL permissions, enabling static hosting, and accessing the final public endpoint.

## 🌍 Live Website Endpoint

Your static website will be publicly available at:

### 🔗 http://mythragsai.s3-website.ap-south-1.amazonaws.com

(Upload your `index.html` file into the S3 bucket to activate the website.)

## 🌐 Overview

You deployed a static website on S3 by completing the following steps:

1. Creating a uniquely named S3 bucket  
2. Uploading website files (HTML, images, assets)  
3. Making objects public using ACL  
4. Enabling static website hosting  
5. Verifying the website through the S3 endpoint  

## 📝 Step-by-Step Process

### 1. Login to AWS Console
- Open AWS Management Console  
- Sign in using your AWS account  
- Note: Record login method if needed for documentation  

### 2. Create an S3 Bucket
- Go to **Services → S3 → Create bucket**  
- Enter a unique bucket name (Example: `mythragsai`)  
- Select the region **ap-south-1 (Mumbai)**  
- Disable **Block all public access**  
- Acknowledge the warning  
- Optional: Enable **Bucket Versioning**  
- Click **Create bucket**

### 3. Upload Your Website Files
Upload:
```
index.html
profile.jpg
assets (if any)
```

### 4. Set Public Permissions (ACL)
- Select `index.html` → **Actions → Make public using ACL**  
- Repeat for all required files  

### 5. Enable Static Website Hosting
Go to:
**Bucket → Properties → Static website hosting**

Then:
- Enable hosting  
- Choose **Host a static website**  
- Set index document to `index.html`  
- Save  

### 6. Access Your Website
- Open the endpoint in a browser  
- Verify the page loads with HTML and images  

## 🛠️ Technologies Used
- Amazon S3  
- AWS IAM  
- Static Website Hosting  
- HTML / CSS  

## 📁 Files Included
```
index.html
profile.jpg
Steps_to_host_static_website.docx
```

