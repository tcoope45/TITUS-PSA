# TITUS-PSA
This is a repository for an assessment from PSA.

##STEPS TO RUN THIS CODE USING CLOUDFORMATION

 --use the given link to download the code from git to a local machine(safe file in any directory)
 
 --login to aws console and go to cloudformation and click CREATE STACK
 
 --keep the template is ready option but we are not using S3 as our source, instead upload a template file
 
 -- choose the location of where the file was save, you could veiw in designer to either convert the json to ymal or validate the code
 
 --create the stack
 
 --To make the code more dynamic, I parameterize some values that reuseable like the vpccidr, subnetcidr AZ to name a few, these value should be given by the the engineer that will run the template.
 
 Note: To ensure Ngnix is in the an ec2 instance in the private subnet, I could have leveraged the userdata component of my EC2 instance creation, in my expereience, I have a separate team that creates that userdata component for me depending on the application that is needed for the instance. This is done through an OKTA project. the Link is given to me and I just add it to my parameter file. This has led me to have little usage of how those are passed but again, when given the opportunity and time, I can get up to speed with those.
