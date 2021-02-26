Site with static content.

Instruction for run in your computer

1) Copy the files from Git repository in your location
Example for Linux:

...{your_location}$ git clone https://github.com/Ivanmc-007/Site_about_company


2) Use Docker to run the application on your localhost
Example for Linux:

- Select a new folder (copied from the repository) - usually this folder has the same name as the repository name
...{your_location}$ cd Site_about_company/

- Build Docker IMAGE 
...{your_location}/Site_about_company$ sudo docker build -t "simple_site:latest" .

- run IMAGE in CONTAINER on port 8090
...{your_location}/Site_about_company$ sudo docker run --detach --rm -p 8090:80 simple_site

- open your browser on http://localhost:8090
