# Deploying a Static Website on Amazon S3 with CloudFront

## Overview
This project demonstrates how to host a static website (portfolio or simple app) using Amazon S3 and distribute it globally with Amazon CloudFront. The goal is to learn cost-effective serverless hosting and global content delivery.

## Steps Performed

1. **Create AWS Account** – Used Free Tier account.
2. **Create S3 Bucket** – Enabled public access for hosting.
3. **Upload Website Files** – Uploaded HTML/JS using AWS CLI (`aws s3 sync`) and AWS Console.
4. **Enable Static Website Hosting** – Configured `index.html` and `error.html`.
5. **Create CloudFront Distribution** – Set S3 bucket as origin, enabled HTTPS.
6. **Test Website** – Verified website via CloudFront domain.
7. **Document Findings** – Analyzed cost and CDN performance benefits.

## Live Website

Access the live site here:http://dy9l4s5jyvc3x.cloudfront.net

## Files in Repository

- `index.html` – Main HTML file
  
- `bucket-policy.json` – S3 bucket policy used
- `README.md` – Project documentation

## Notes / Lessons Learned

- AWS CLI is used for automation.
- CloudFront significantly reduces load times for global users.
- Static hosting via S3 is cost-effective for small projects.
- Always use `.gitignore` to prevent large binaries from being pushed to GitHub.
