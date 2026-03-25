# Event Announcement System

A serverless event announcement website built on AWS that allows users to 
subscribe to event notifications, view upcoming events, and create new events.

---

## Live Demo
S3 Static Website URL:http://event-announcement-website-797793345031-us-east-1-an.s3-website-us-east-1.amazonaws.com

img width="620" height="534" alt="image" src="https://github.com/user-attachments/assets/2001253f-523c-4692-bdaf-7ed10f0acc68"

---

## Architecture
![Architecture Diagram](architecture/diagram.png)

The system is built entirely on AWS serverless services:
- User visits the static website hosted on **S3**
- Event data is stored and retrieved from **S3** (`events.json`)
- **API Gateway** exposes two endpoints: `/subscribe` and `/create-event`
- **Lambda** functions handle backend logic for subscriptions and event creation
- **SNS** manages email subscriptions and sends notifications to subscribers
- **IAM** roles secure access between services

---

## Services Used
| Service | Purpose |
|---|---|
| AWS S3 | Frontend hosting and event data storage |
| AWS SNS | Email subscriptions and notifications |
| AWS Lambda | Backend logic for events and subscriptions |
| AWS API Gateway | API endpoints for frontend-backend communication |
| AWS IAM | Permissions and access control |

---

## Project Steps
1. **S3 Frontend Hosting** — Set up static website hosting with public access
2. **SNS & Lambda** — Configure notifications and backend logic
3. **API Gateway** — Set up and deploy API endpoints
4. **Testing & Finalizing** — End-to-end testing of all features

> 📄 See the [`docs/`](./docs) folder for detailed notes on each step.

---

## Cleanup
To avoid any unexpected AWS charges, delete the following after the project:
- S3 Bucket
- Lambda Functions
- API Gateway
- SNS Topic
- IAM Roles

---

## What I Learned
> *(Fill this in as you complete the project)*
