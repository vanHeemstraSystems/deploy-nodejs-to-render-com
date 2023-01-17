deploy-nodejs-to-render-com
# Deploy NodeJS to Render.com

Based on "Deploy Your Node.js Application to render.com" at https://youtube.com/watch?v=39ngl2PF43Q

Based on ""nodejs-render-deployment" at https://github.com/dube-academy/nodejs-render-deployment

## 100 - Introduction

## 200 - Requirements

## 300 - Building Our Application

On https://dashboard.render.com/ choose **New +** and select **Web Service**.

Enter the following information in the form of the new web service:

### General

**Name**: sample-node-deployment

**Region**: Frankfurt (EU Central)

**Instance Type**: Free

### Build & Deploy

**Branch**: production

**Root Directory**: = leave empty =

**Build Filters**: = leave empty =

**Build Command**: $ yarn

**Start Command**: $ yarn start

**Auto-Deploy**: Yes

**Deploy Hook**: = leave what is being given =

### Custom Domains

We will address this separately, for now skip it.

### PR Previews

**Pull Request Previews**: Disabled

### Health & Alerts

**Health Check Path**: = leave empty =

**Service Failure Notifications**: Use account notification settings

Finally, choose **Create Web Service**

After your web service has been deployed and build, the URL to visit it will be highlighted in the log file.

**NOTE**: Edit any files on branches other then **production**, then use ```pull requests``` to merge your changes into the ***production** branch. Rendfer will automatically start deploying changes that are detected on the **production** branch.





## 400 - Conclusion

