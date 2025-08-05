# AUG-05-25

Training -  33mins of Zone 2 (5% incline, 4km/h),
Bench Press - 50kg - 4 reps
Push-ups - 10 reps
Skull Crusher - 10Kgs, 20 reps
Curl - 10kgs, 20 reps

Leetcode - Longest Repeating Character Replacement

Udemy 10mins 

we do not store file in the db, we store the path to the file in db

const multer = require('multer');
const storageConfig = multer.diskStorage({
    destination:function(req,file,cb){
        cb(null,"images")
    },,
    filename: function(req,file,cb){
        cb(null,file.originalname)
    },
})

const upload = multer({dest: storageConfig})

router.post('/profiles', ,function(req, res){

    const uploadedImage = req.file;
    const userData = req.body;

    db.getDB().collection('users').insertOne({
        name: userData.username
        imagePath: uploadedImage.path
    })
});

Project - Figured out with clerk problem.
English Reading - 'The Giver' 15mins


