# AWS Voting App
Host a static web app with Python backend using AWS S3 for frontend and Lambda for server-side logic, featuring HTML, CSS, and configurable settings.

### Project Structure
```
.
├── static/                  # Static files (CSS, JS, images)
│   └── default.css          # Default stylesheet
├── templates/               # HTML templates
│   └── index.html           # Main HTML file
├── config_file.cfg          # Configuration file
├── main.py                  # Python backend logic
└── README.md                # Project documentation
```

### Features
* Frontend: A responsive static web page (index.html) styled with default.css.
* Backend: Python-based server-side logic (main.py) for handling API requests.
* Configuration: Customizable settings in config_file.cfg.

### Hosting on AWS
This app is hosted on AWS using the following services:
1. Amazon S3: Hosts static files (index.html, static/default.css).
2. AWS Lambda: Runs the Python backend (main.py).
3. API Gateway: Exposes the Lambda function as an API endpoint.

### Steps to Deploy
1. Static Files:
* Upload index.html and static/ to an S3 bucket.
* Enable static website hosting in the S3 bucket settings.
2. Backend:
* Package main.py and its dependencies into a deployment package.
* Create a Lambda function and upload the deployment package.
* Set up API Gateway to trigger the Lambda function.
3. Custom Domain (Optional):
* Use Route 53 to register a custom domain.
* Use CloudFront to enable HTTPS and improve performance.

### Acknowledgments
This project uses source code originally from [Azure-Voting-App](https://github.com/ceteongvanness/azure-voting-app)
