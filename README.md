# AWS S3 Public File Hosting Task

## 🪣 Bucket Name
`nivi1702`




## 🌐 Public Image URL
(https://nivi1702.s3.us-east-1.amazonaws.com/img2.jpg)

## ✅ Steps Done
1. Created an S3 bucket
2. Uploaded `img2.jpg`
3. Enabled public access via bucket policy
4. Verified the public URL

## 🔐 Bucket Policy Used
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
