# Chapter 6

All of these notebooks were run on the image created from the docker container sad_nightingale. I did this because the first notebook required git and git-lfs, both of which install a ton of dependencies and I wanted an exit if they messed up the original container.
The new container is called fervent_murdock

	(base) rob@KAUWITB:~$ docker container ps -a
	CONTAINER ID   IMAGE               COMMAND                  CREATED       STATUS                     PORTS     NAMES
	6293391ef86c   hfcourse:latest     "/opt/nvidia/nvidia_…"   2 hours ago   Exited (0) 9 minutes ago             fervent_murdock
	c198335c5f35   pt1131:20230216     "/opt/nvidia/nvidia_…"   4 days ago    Exited (0) 2 hours ago               sad_nightingale
	...
	
	(base) rob@KAUWITB:~$ docker images 
	REPOSITORY                                TAG                            IMAGE ID       CREATED         SIZE
	hfcourse                                  latest                         5334d5165a84   2 hours ago     22GB
	pt1131                                    20230216                       2af8128e198b   7 days ago      17.9GB
	huggingface/transformers-pytorch-gpu      latest                         47dc5ba9a731   8 days ago      17.8GB
	...
