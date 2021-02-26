Site with static content.

Instruction for run in your computer

1) Copy the files from Git repository in your location
Example for Linux:

...{your_location}$ git clone https://github.com/Ivanmc-007/{repository_name}


2) Use Docker to run the application on your localhost
Example for Linux:

- Build Docker IMAGE 
...{your_location}$ sudo docker build -t "simple_site:latest" .

- run IMAGE in CONTAINER on port 8090
...{your_location}$ sudo docker run --detach --rm -p 8090:80 simple_site

- open your browser on http://localhost:8090
