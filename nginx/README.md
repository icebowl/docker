https://hub.docker.com/_/nginx

https://docs.docker.com/samples/library/nginx/

https://www.dailysmarty.com/posts/steps-for-deploying-a-static-html-site-with-docker-and-nginx
move html filw to ~/html
docker build -t html-server-image:v1 .

docker run -d -p 80:80 html-server-image:v1
docker run -d -p 8080:80 html-server-image:v1


Step 1 - Create a Directory for the Website

Make sure that you have your HTML files already in the current directory.
Step 2 - Create a file called Dockerfile

Place the following contents into the Dockerfile

FROM nginx:alpine
COPY . /usr/share/nginx/html

These lines of code represent the image we're going to use along with copying the contents of the current directory into the container.

 
Step 3 - Build the Docker Image for the HTML Server

Run the following command:

docker build -t html-server-image:v1 .

You can confirm that this has worked by running the command:

docker images

And it should show you output something like this:

 
Step 4 - Run the Docker Container

Run the following command to run the HTML container server:

docker run -d -p 80:80 html-server-image:v1

 

 
Step 5 - Test the Port with cURL

Run the following command to ensure the server is running:

curl localhost:80

You can also view it in the browser now by going to localhost:80 and you should see your HTML file, as shown below:
