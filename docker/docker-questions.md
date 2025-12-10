1. What is Docker and how it is diff from VM?

- Docker is an containerization platform that packages application and their dependencies into a lightweight portable containers.Unlinke VM it shares host OS kernel.

2. What is Docker image and how it is differ from containers?

- Docker image is a read-only template used to create containers while container is running instance of image.


  Image vs Container:

Aspect	   Docker Image  	              Docker Container
State	   Static, immutable	           Dynamic, mutable
Purpose 	Template/Blueprint          	Running application
Layers	   Read-only layers 	           Read-only + writable layer
Storage 	Stored on disk  	           Running in memory
Lifecycle	Built once, used many times	    Created, started, stopped, deleted

3. What is the diff bet CMD and ENTRYPOINT ?

Both CMD and ENTRYPOINT defined what command runs when container starts. But, they behave differently when additional arguments passed.

Key Differences:

Aspect	    CMD  	                                       ENTRYPOINT
Override	Completely replaced by docker run args	     Args appended to ENTRYPOINT
Purpose  	Default command or arguments	             Fixed command that always runs
Flexibility	High - can be completely changed             Low - command is fixed
Use Case	Default behavior that can be overridden	     Core application that always runs