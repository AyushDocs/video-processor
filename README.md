# AWS Video Processing Pipeline 🎥

> A serverless video processing workflow using AWS services (S3, SNS, SQS, Lambda, CloudFront) with IAM-based authentication.

## 🚀 Features
- User uploads videos via a demo site
- Event-driven processing pipeline with SNS + SQS
- Transcoding to multiple resolutions using FFmpeg in Lambda
- Secure video delivery via CloudFront
- Built with AWS-native CI/CD deployment

## 🛠 Tech Stack
- **AWS Services**: S3, SNS, SQS, Lambda, CloudFront, IAM
- **Language**: Python/Node.js (for Lambda)
- **CI/CD**: GitHub Actions + Docker
- **Auth**: IAM-based authentication

## 📂 Repository Structure
.github/workflows/ → CI/CD pipelines
docs/ → Documentation
src/ → Lambda & App code (coming soon)


## 📦 Deployment
> This project uses GitHub Actions to build Docker images and deploy to AWS.

### Steps:
1. Fork & clone the repo
2. Create `.env` file with AWS credentials
3. Run:
```bash
docker build -t aws-video-pipeline .
docker run -p 8080:8080 aws-video-pipeline
```

## 📝 License
Licensed under the MIT License.


---

## **5. `CONTRIBUTING.md`**
```markdown
# Contributing Guidelines

Thank you for your interest in contributing!

## Steps to Contribute
1. Fork this repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/my-feature
   git commit -m "Add my feature"
   git push origin feature/my-feature
3. Open a Pull Request.

```


---

## **6. `CODE_OF_CONDUCT.md`** (Contributor Covenant)
```markdown

# Contributor Code of Conduct

As contributors and maintainers of this project, we pledge to respect all people who contribute through reporting issues, posting feature requests, updating documentation, submitting pull requests, and other activities.

We are committed to making participation in this project a harassment-free experience for everyone.

For full details, see the [Contributor Covenant](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).
