Title: Using Linux - Basic Command 1
Date: 2013-01-18 02:03 

##List the files in the directory##
This one of the most used command in the CLI (command line interface) it shows everything in the current directory.  
You type

	$ls

You get

	folder/    test.txt    photo.jpg

However sometime this is not very useful as it displays a limited amount of data (other than file/folder name it has nothing), so here are some option you might want to consider using.

	$ls -l

This will give you the long format of the data including ownership, creator, file size, modified date/time

	drw-------	1	Ubuntu Ubuntu 	890 Jan 18 13:22	folder/
	-rw-rw-r--	1	Ubuntu Ubuntu 	135	Jan 18 13:51	test.txt
	-rw-rw-r--	1	Ubuntu Ubuntu 	455	Jan 18 13:51	photo.jpg

If you really want to see something you should not see (like hidden files), then you can use

	$ls -a

However this will not give you the long format of the file listing, therefore what you really want is 

	$ls -la

So you will be able to see the hidden file in the directory (usually the configuration files and upper level folders)
	
	drwxr-xr-x+	1	Ubuntu Ubuntu	0	Nov 23 11:05	.
	drwxr-xr-x+	1	Ubuntu Ubuntu	0	Nov 23 11:05	..
	drwxr-xr-x+	1	Ubuntu Ubuntu	0	Nov 23 11:54	.svn
	drw-------	1	Ubuntu Ubuntu 	890 Jan 18 13:22	folder/
	-rw-rw-r--	1	Ubuntu Ubuntu 	135	Jan 18 13:51	test.txt
	-rw-rw-r--	1	Ubuntu Ubuntu 	455	Jan 18 13:51	photo.jpg