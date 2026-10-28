# AWS Static Website Deployment

A static website (HTML, CSS/SCSS, JavaScript, with a custom error page) used to practise **deploying and hosting a website on AWS**.

## What's Inside

```
AWSDemo-master/
├── index.html     # Home page
├── error/         # Custom error page
├── assets/        # CSS/SCSS and JavaScript
└── images/
```

## Deploying on Amazon S3 (static website hosting)

1. Create an S3 bucket and **enable static website hosting**, with `index.html` as the index document and the error page as the error document.
2. Upload the contents of `AWSDemo-master/`:
   ```bash
   aws s3 sync AWSDemo-master/ s3://<your-bucket-name>/
   ```
3. Allow public read access with a bucket policy (or put **CloudFront** in front of a private bucket for HTTPS and caching).
4. Open the S3 website endpoint (or the CloudFront domain) in your browser.

## Skills Practised

AWS S3 static hosting · bucket policies and access control · AWS CLI · CloudFront basics · HTML/CSS/JS

## Author

**Surupam Kumar Pandey** · [GitHub](https://github.com/Surupam2002) · [LinkedIn](https://www.linkedin.com/in/surupam-kumar-pandey-44b293218)
