# AWS Voting App
This is a static web application built with Python, HTML, and CSS. It includes a frontend (`index.html`) and a backend (`main.py`) for server-side logic. The app is designed to be hosted on AWS using S3 for static files and AWS Lambda + API Gateway for backend functionality.

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
- **Frontend**: A responsive static web page (`index.html`) styled with `default.css`.
- **Backend**: Python-based server-side logic (`main.py`) for handling API requests.
- **Configuration**: Customizable settings in `config_file.cfg`.

### Hosting on AWS
This app is hosted on AWS using the following services:
1. **Amazon S3**: Hosts static files (`index.html`, `static/default.css`).
2. **AWS Lambda**: Runs the Python backend (`main.py`).
3. **API Gateway**: Exposes the Lambda function as an API endpoint.

### Steps to Deploy
1. **Static Files**:
- Upload `index.html` and `static/` to an S3 bucket.
- Enable static website hosting in the S3 bucket settings.
2. **Backend**:
- Package `main.py` and its dependencies into a deployment package.
- Create a Lambda function and upload the deployment package.
- Set up API Gateway to trigger the Lambda function.
3. **Custom Domain (Optional)**:
- Use Route 53 to register a custom domain.
- Use CloudFront to enable HTTPS and improve performance.

### Local Development
#### Prerequisites
- Python 3.x
- `pip` for dependency management

#### Installation
1. Clone this repository
```
git clone https://github.com/ceteongvanness/aws-voting-app.git
cd aws-voting-app
```

### Configuration
Edit `config_file.cfg` to customize app settings.

### Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (git checkout -b feature/your-feature).
3. Commit your changes (git commit -m 'Add some feature').
4. Push to the branch (git push origin feature/your-feature).
5. Open a pull request

### License
This project is licensed under the MIT License. See the [LICENSE(https://github.com/ceteongvanness/aws-voting-app/blob/main/LICENSE) file for details.

### Acknowledgments
This project uses source code originally from [Azure-Voting-App](https://github.com/ceteongvanness/azure-voting-app)
