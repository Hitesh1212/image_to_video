# image_to_video
generating image to video using AI video model

#aiml video model name = runway/gen4_turbo 
-this model only required image url , and that prompt is optional.
-It supports high-quality, temporally coherent video generation from a single input image.

#pipeline
-User signUp/Login 
-Logged In user can go to dashboard
-Users upload a clothing image via a simple interface in dashboard.
- Form submission sends the image to the backend.

 #backend
 -User data create and save in database using mongoose.
 - Accepts image upload using multer and save it in cloudinary.
 - get image url from cloudinary.
 - Passes the image to a AI video inference module.
 - Returns the generated video file or video url.

#requirements
 - nodejs
 - reactjs
 - antd
 - express
 - mongodb
 - multer
 - cloudinary

## clone the repo
git clone https://github.com/Hitesh1212/image_to_video.git
cd image_to_video

##install frontend
cd client
npm install

## install backend
cd server
npm install

#.env file
cd server/.env

## env data

PORT=
MONGO_URI=
JWT_SECRET=
URL=
CLOUDINARY_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_SECRET_KEY=
AIML_URL=
AIML_MODEL_NAME=
AIML_API_KEY=



