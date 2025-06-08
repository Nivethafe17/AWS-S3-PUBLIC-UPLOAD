#A BUCKET SETUP WITH FILES UPLOAD

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: NIVETHA P

*INTERN ID*: CT04DN74

*DOMAIN*: CLOUD COMPUTING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTHOSH


## ☁️ AWS S3 Public File Hosting Task

This task involves creating and configuring an Amazon S3 bucket to host and share files publicly over the internet. As part of the internship under the cloud computing domain, this task demonstrates hands-on experience with one of the most widely used cloud storage services: Amazon S3.

---

## 🪣 Bucket Name

**`nivi1702`**

This is the unique bucket name created under my AWS account. S3 bucket names must be globally unique, and I selected this name to align with my personal identity and ensure it is distinct.

---

## 🖼️ Uploaded Files

Two image files were uploaded to the S3 bucket:
- `img1.webp`
- `img2.jpg`

These files were selected to demonstrate the public hosting capability of AWS S3, which is useful for sharing assets like images, static files, PDFs, and more in real-world projects.

---

## 🌐 Public Image URL

After uploading and configuring the access, the following file is now publicly accessible:
- [img1.webp](https://nivi1702.s3.us-east-1.amazonaws.com/img1.webp)
- [img2.jpg](https://nivi1702.s3.us-east-1.amazonaws.com/img2.jpg)

You can click on the link to directly view the image from anywhere without requiring AWS credentials.

---

## ✅ Steps Performed

1. **Signed in to AWS Console** using a new account and selected the S3 service.
2. **Created a new S3 bucket** named `nivi1702`, making sure to select the appropriate region (US East - N. Virginia).
3. **Disabled “Block All Public Access”** from bucket permissions to allow file sharing.
4. **Uploaded image files** `img1.webp` and `img2.jpg` using the AWS S3 console.
5. **Manually applied a bucket policy** to allow public read access to all objects inside the bucket.
6. **Verified the public access** by opening the image URL in a browser.
7. Documented all steps and prepared this README for uploading to GitHub.


---
#output

## 🔐 Bucket Policy Used

The following policy was added under the "Permissions > Bucket Policy" section of the S3 console:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadForObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::nivi1702/*"
    }
  ]
}

