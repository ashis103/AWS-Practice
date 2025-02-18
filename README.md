# AWS-Practice
Lab Practice


echo "# AWS-Practice" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ashis103/AWS-Practice.git
git push -u origin main


…or push an existing repository from the command line
git remote add origin https://github.com/ashis103/AWS-Practice.git
git branch -M main
git push -u origin main

1. 1st We will create S3 bucket and put a index.html file .
   --- what to do ? We will run and edit index file from GIT it will automatic update globally ...mean s3 bucket update and run ..

 Git---> S3 Bucket ----> Globally Access .

2. Go Bucket Propertise ---> Static Web site hosting --Enable IT .
   Index Document a need to set default side page .

3. S3 Permission set Edit Bucket policy . We can find from Aws example policy .

   {
   "Version":"2012-10-17",
   "Statement":[
     {
       "Sid":"PublicReadGetObject",
       "Effect":"Allow",
       "Principal":{"*"},
       "Action":"s3:GetObject",
       "Resource":"arn:aws:s3:::amzn-s3-AWS-Practice/*",

         
       }
   ]
}

5. run from link file.
