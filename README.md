# CS_548-Assignment1
## Csd4054

---

1.
  * a)

		docker pull nginx:1.23.3

		docker pull nginx:1.23.3-alpine

		docker images
			
	![1](task1/1.JPG)
		
  * b)

		Από το screenshot φαίνεται το 1.23.3-alpine είναι 40.7MB και το 1.23.3 είναι 142MB
			
  * c)
		
		docker run -d --name task1c -p 8080:80 nginx:1.23.3-alpine
		
		
	![2](task1/2.JPG)
		
		Μας απαντά μια default σελίδα του nginx όπου μας επιβεβαιώνει ότι ο web server τρέχει επιτυχώς
		
	![3](task1/3.JPG)
	
  * d)

		Από την εντολή docker ps παραπάνω μπορούμε να δούμε ότι το container τρέχει καθώς στο status λέει up 2 seconds.
		
  * e)
			
		docker logs [container_id or name]
		docker logs task1c		
			
	![4](task1/4.JPG)
	
  * f)
		
		docker stop [container_id or name]
		docker stop task1c
		
		Όπως βλέπουμε το container status είναι exited 7 seconds ago άρα σταμάτησε
		
	![5](task1/5.JPG)
	
  * g)

		docker start [container_id or name]
		docker start task1c
		
		Όπως βλέπουμε το container status είναι up 2 seconds άρα τρέχει
		
	![6](task1/6.JPG)
	
  * h)

		docker rm -f task1c
		
		Όπως βλέπουμε το container σταμάτησε και διαγράφτηκε από το σύστημα
		
	![7](task1/7.JPG)
	

2.
		
