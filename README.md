🎨✨ AI Image Editing App — Serverless + Bedrock Titan V2

Edit images with AI. No servers. Just AWS magic.

<p align="center"> <img src="https://img.shields.io/badge/AWS-Bedrock-orange?style=for-the-badge" /> <img src="https://img.shields.io/badge/Serverless-Application-blueviolet?style=for-the-badge" /> <img src="https://img.shields.io/badge/React-Frontend-61dafb?style=for-the-badge&logo=react" /> <img src="https://img.shields.io/badge/Amplify-Hosting-ff9900?style=for-the-badge&logo=aws-amplify" /> </p>
🖼️ About the Project

Welcome to the AI Image Editing App, a fully serverless application powered by Amazon Bedrock’s Titan Image Generator V2 — giving you the ability to create, edit, transform, and remix images using the power of generative AI.

This project was built as part of the AWS AI Workshop, but it is production-ready, scalable, and perfect for showing off your cloud skills.

⚡ What This App Can Do
✨ AI-Powered Image Editing

Type what you want → Titan V2 generates it.
Examples:

“Make background pastel purple”

“Convert this into a Pixar-style character”

“Give this object a neon glow”

🔐 Secure Login (Cognito)

Every user signs in using secure authentication provided by AWS Cognito.

⚙️ Serverless Backend

A beautifully simple backend created using:

API Gateway

Lambda

Amazon Bedrock

DynamoDB

No servers. No maintenance. Just compute when you need it.

🌐 Hosted on AWS Amplify

Your app goes live on the internet with one click.
Push to GitHub → Amplify deploys automatically.

🧬 High-Level Architecture
         🤳 User
           |
           v
   [React Frontend – Amplify Hosting]
           |
           v
   [Amazon Cognito – Auth]
           |
           v
   [API Gateway]
           |
           v
   [Lambda Function]
           |
           v
   [Amazon Bedrock – Titan Image Generator V2]
           |
           v
   [DynamoDB – History Storage]


A modern, clean serverless pipeline designed for real-world workloads.

🧩 Tech Stack
Layer	Technology	Purpose
Frontend	React + Amplify Hosting	UI for image editing
Auth	Amazon Cognito	Login/signup
AI Model	Bedrock Titan Image Generator V2	Image generation
Backend	Lambda	Runs AI logic
API	API Gateway	RESTful API
Database	DynamoDB	Save results & history
🔧 Setup Guide (Super Simple)
1️⃣ Clone the Project
git clone https://github.com/YashasviRajput13/image-editing-app.git
cd image-editing-app

2️⃣ Install Dependencies
npm install

3️⃣ Add Your AWS Config

Update the workshopConfig.js file:

window._workshopConfig = {
  cognito: {
    userPoolId: 'YOUR_POOL_ID',
    userPoolClientId: 'YOUR_CLIENT_ID',
    region: 'us-east-1'
  },
  api: {
    invokeUrl: 'YOUR_API_GATEWAY_URL'
  }
};

4️⃣ Run Locally
npm start

🌟 What Makes Titan Image Generator V2 Special?

🟣 High-fidelity image generation
🖌 Inpainting and object editing
🎨 Beautiful artistic transformations
🧠 Strong prompt alignment
🛡 Safe and enterprise-ready

Readable. Powerful. Responsible.

🚀 Deploying with Amplify

Open AWS Amplify Console

Click Create App → Host Web App

Select GitHub

Choose your repo

Deploy

CI/CD is automatically enabled 🎉
Every push to main updates your live site.

🛤️ Future Possibilities

AI-powered background removal

Photo restoration

Applying LLM-based captioning

Multi-model support (Stable Diffusion, Claude Image-to-Text)

Save/share user galleries

Light/Dark mode UI

🤝 Contributing

Contributions, ideas, and pull requests are always welcome!
Whether it's UI improvements, new features, or AWS enhancements — feel free to collaborate.

⭐ Give This Repo a Star

If you like this project, hitting the ⭐ button helps others discover it!
