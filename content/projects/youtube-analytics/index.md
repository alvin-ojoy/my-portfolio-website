---
title: "Serverless YouTube Channel Analytics Tool"
date: 2024-09-05
tags: ["devops", "serverless", "aws", "lambda", "python"]
thumbnail: "blowfish_logo.png"
github_url: "https://github.com/yourusername/youtube-analytics-lambda"
---

## Overview  
A **cost-efficient analytics pipeline** that fetches YouTube API data (views, engagement) daily via AWS Lambda, processes it with Pandas, and visualizes it in a React frontend.  

![Workflow](/images/projects/youtube-analytics-flow.png)  
*Flow: YouTube API → S3 (raw) → Lambda (transform) → DynamoDB → React frontend*

## Key Features  
- 🚀 **Serverless**: Lambda + DynamoDB + S3 (zero idle costs)  
- 📈 **Automated Reports**: Email summaries via Amazon SES  
- 🔄 **CI/CD**: Terraform deploys Lambda + API Gateway  
- 🎥 **Filmmaking Metrics**: Track audience retention vs. video edits  

## Technical Stack  
```plaintext
AWS Services:
- Lambda (Python 3.10)
- DynamoDB (NoSQL)
- EventBridge (scheduled triggers)
- S3 (data lake)

Libraries:
- Pandas (data cleaning)
- Matplotlib (generate graphs)
- Serverless Framework (deployment)