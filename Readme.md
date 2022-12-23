Hi,

You are on a document to explain how my website work.

First we have a simple architecture based on that:


	    |->cv.html
	    |->portfolio.html
index.html->|->categories.html	
	    |->hobbies.html	|->sort_file.txt
	    |->projects-------->|->0------------>|0.html  	|0i0.jpg
				|		 |images------->|0i1.jpg
				|
				|->1------------>|1.html  	|1i0.jpg
				|		 |images------->|1i1.jpg
				|
				|->2------------>|2.html  	|2i0.jpg
						 |images------->|2i1.jpg
							  	|2i2.jpg

HTML files:						 			
index.html: It is a simple page to introduce the different way to visit my website
cv.html: It is just my CV
hobbies.html: A little page about my favorite sports, music instrument ...
portfolio.html is a little introdution about a part of the projects in the projects folder
	It will give a link to each presentated projects if more informations are needed.
categories.html Is a page with every projects sorted by catergories each projects can be in
	some categories.

PHP structure:
The sort_file.txt is created to replace a mysql database that is too much in this simple project.
	it is made to make a link between the projects names, the projects numsers and the 
	categories of that projects.
In each projects of each folders named from 0 to N with N the last project created we can see a 
	folder named images and who contain the images named with three fields: The first field
	for the project number. The second to specify that is an image a split the first and the
	last field who specify the number of the image in that project.
In each N.html document from each N folders the different informations from sort_file are used to 
	create the simplest .html as possible with the less number of modification if for example
	the name of the project change.
	 
