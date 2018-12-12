# Administration IT
## Laboratoire n°3 : 

> Auteurs : Loic Frueh - Koubaa Walid	
> Enseignant : Graph Marcel   
> Assistants : Bastien	
> Date : 15.12.2018  

### Objectives

Pedagogical objectives
Deploy a web application in a two-tier architecture for scalability

Configure a load balancer

Performance-test a load-balanced web application

In this lab you will perform a number of tasks and document your progress in a lab report. Each task specifies one or more deliverables to be produced. Collect all the deliverables in your lab report. Give the lab report a structure that mimics the structure of this document.

##Task 1

First we downloaded vagrant and Jmeter on both are laptops.
Once we cloned the repository, we execute the command:
	
	vagrant up
	
(insert image 1)
	
we obtain the same result as specified.

Some occasional error messages from dpkg-preconfigure, debconf or invoke-rc.d, appeared. We safely ignore them.

Then we log into the ubuntu VM with the command 

	vagrant ssh
	
(image 2)
	
Here is all the docker inside

image 3

Nous obtenons en lancant sur postant un requete sur l'adresse http://192.168.42.42/ 

le JSON suivant :

	(image 4)
	
Nous ouvrons ensuite JMETER

(image 5)


1. When you open and refresh the URL http://192.168.42.42 in your browser. Add screenshots to complement your explanations. We expect that you take a deeper a look at session management.
2. dw
3. dw
4. dw
5. dw
6. dw

##Task 2

1. We chosed the first way : use the SERVERID provided by HAProxy. 
These two objects proposed are both cookies to separate requests.
SERVERID is controlled by HAProxy and NODESESSID is controlled by Node server.
The main difference is the cookie "maker". For the first one, proxy makes 



2. The only modifications made were to add the following lines to the haproxy.cfg file .



