# Media Streaming Server Solution by The Water Cooler
[Powerpoint Presentation](https://docs.google.com/presentation/d/10wmty7K7HCv-a3p8OxNH3ZqIrVCZ4bPY/edit?usp=sharing&ouid=104961336018066608218&rtpof=true&sd=true)

[Video Link](https://youtu.be/Nk0SmgugNwU)

[Test Server](http://lyve-cloud-frontend.s3-website-ap-southeast-1.amazonaws.com/)

## Introduction
A middleware solution designed to stream videos stored in Lyve cloud bucket in real-time where users can anonymously access the content.

## Requirements
Details of your environment: 

* Windows | Linux Compatible 
* NodeJS Version > 14
* Npm Package Manager 

## Known Limitations 
Streaming will be interrupt when client's network becomes unstable


## Running Steps
**Step 1:** Get your Lyve Cloud bucket credentials.   
Here's what you'll need:
* Access Key
* Secret key
* Endpoint URL

**Step 2:** 
Make a new file named ".env" in the root directory. Fill up the variables accordingly. 
Refer to below for example.
```bash
 ACCESS_KEY=
 SECRET_KEY=
 ENDPOINT_URL=s3.ap-southeast-1.lyvecloud.seagate.com
 REGION=ap-southeast-1
 AUDIT_LOGS_BUCKET=x-auditlogs
 NEW_BUCKET=x-media-files
```
**Step 3:**
Install NPM Packages 
```bash
  npm install
```

**Step 4:**
Start the middleware
```bash
  npm start
```

**Step 5:**
Upload video to Lyve Cloud Bucket

**Step 6:**
In order to use the middleware on your local machine, 
http://localhost:4040/api/video/videoname.mp4

Example Video Name = cat.mp4

To stream cat.mp4, enter http://localhost:4040/api/video/cat.mp4 as the source to the HTML video element 

### `/code`
This folder contains all the code files.

### `/documentation`
This folder contains the demo video and presentation file.

### `/images`
This folder contains all the images.
