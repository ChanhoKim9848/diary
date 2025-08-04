# AUG-04-25

Training -  30mins of Zone 2 (7% incline, 4km/h),
Barbell Lunges - 30KGs 8 reps, 45kgs, 4 reps 

Leetcode - Best Time to Buy A Stock, Longest Substring Without Repeating Characters
English Reading - 'The Giver' 15mins

Udemy 10mins 

we do not store file in the db, we store the path to the file in db

const multer = require('multer');

const storageConfig = multer.diskStorage({
    destinations: function(req,file,cb){},
    filename: function(req,file,db){},
})

const upload = multer({ dest: storageConfig});

router.post(/new-user, upload.single('image'), function(req,res){
    const uploadedImageFile = req.file;
    const userData = req.body;
    res.redirect('/')
})

Project - 3 hours

fixed uploadthing social-media-app project
solution:
fixed logic of uploadthing in next.config.mjs




