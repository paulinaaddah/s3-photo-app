# S3 Photo App

A browser-based AWS photo manager where users can upload, view, and delete images using S3 and Cognito.

## Overview

This project is a serverless photo album app deployed on AWS. Users interact with a browser interface to manage photos in an Amazon S3 bucket. The app uses Amazon Cognito to authorize access for unauthenticated users, and the AWS SDK for JavaScript to handle upload, view, and delete operations.

## Live Demo

🚧 *Coming Soon – Demo video and screenshots to be added.*

## Architecture

- **Frontend:** Static HTML, CSS, and JS served from S3  
- **Backend (Serverless):** Amazon S3 + Amazon Cognito + IAM Roles  
- **Deployment:** CloudShell compilation and S3 hosting

## Tech Stack

- Amazon S3
- Amazon Cognito
- IAM Roles & Policies
- JavaScript SDK (v3)
- AWS CloudShell

## Features

- Upload, view, and delete images from albums
- Full AWS authentication and access control using Cognito
- Hosted as a static website on S3

## Setup Instructions

1. Create an S3 bucket
2. Set public access, attach bucket policy (see `website-hosting-policy.json`)
3. Set up Cognito Identity Pool for unauthenticated users
4. Edit `PhotoApp.ts` with your region, identity pool ID, and bucket name
5. Compile using CloudShell:
   ```bash
   npm install
   npm run build
