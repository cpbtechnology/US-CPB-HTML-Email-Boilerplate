# US CPB HTML Email Boilerplate

This is an email template that is based on the HTML Email Boilerplater. (http://htmlemailboilerplate.com/)

CP+B has made some updates and guidelines to allow for more compatibility with email clients. 


#Instructions 
<h3>Photoshop</h3>

	1.) Use the slice tool in photoshop to cut up the image. Makes sure there are't any gaps between boxes.
	
	2.) Select any call to action boxes with the slice tool, Right click > Edit Slice Options. From here you can set the Name, URL, Target, Message Tex, and Alt Tag. 
	
	3.) When you are done, Save for Web & Devices > all images to JPG with a quality of 80.
	
	4.) Once you have the correct image format, select save. You will be prompted with an image save location and how you other settings. Choose -> Format: html and images, Settings: XHTML, Slices: All Slices.
	
	Photoshop will generate a nice html page with the table and images in it. 
	
	 
	
<h3>Development & Testing</h3>
	1.) Now that photoshop has generated your table with images, you need to update 3 files: boilerplate-email.html, boilerplate-online.html, and boilerplate.txt. The email template will be the page that is viewed in the email, the online template is the page that is linked to from the email template as "Problem Viewing? Click Here", and the boilerplate.txt is for displaying plain text.
	 
	2.) Start with a browser test and make sure it looks good locally. Once you have the site looking good then you can move to production. 
	
	3.) Each email requires a Content Delivery Network to host all the images and html. Use the CDN provided, upload all the images. Once you have the images uploaded, find and replace all the image locations paths with the absolute urls.
	
	4.) Often times the Call to action links require Omniture Codes or special link prefixes for analytical data.
	
	5.) All of the copy from the psd(s) needs to be added to the alternate text tags within the pertaining table cell. 
	
	6.) All the links need to open in a new tab: target="blank"
	
	7.) Take all the copy in the PSD and add it to the .txt file  without any html markup. 
	
	8.) Once you think your email is all buttoned up, send out a few test emails through the CDN. 
	
	9.) You can fire up your VM and view the email in different browsers and email applications to further QA your code. http://litmus.com/email-testing also offers a nice testing suite. 

	

<h3>Production + Deployment</h3>
	1.) Once the Email has passed QA have a senior developer send out the email within waves based on location to prevent flooding the server. 



