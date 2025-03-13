MINIMAL FLASK CHATBOT (DOCKER VERSION)  

This is a Dockerized version of the Minimal Flask Chatbot, allowing users to run the chatbot without manually setting up dependencies or installing Python packages.  
Instead, everything is packaged into a Docker image, making it easy to deploy anywhere.

This image was built using the source code from the original repository:  
https://github.com/Aleexc12/minimal-flask-chatbot

The prebuilt Docker image is available on Docker Hub:  
https://hub.docker.com/r/aleexc12/minimal-flask-chatbot

FEATURES  

- Fully containerized using Docker  
- No need to install dependencies manually  
- Uses Hugging Face Transformers for generating responses  
- Simple chat interface  
- Minimal setup – just run a single command with docker-compose  

INSTALLATION AND USAGE  

1. Clone the repository  
```sh
git clone https://github.com/Aleexc12/minimal-flask-chatbot-docker.git
cd minimal-flask-chatbot-docker
```

2. Run the chatbot using Docker Compose  
```sh
docker-compose up -d
```
This will pull the chatbot image from Docker Hub (aleexc12/minimal-flask-chatbot) and run it in a container.  
The first time you run this, it might take a few minutes depending on your internet speed and system performance.  

3. Access the chatbot  
Once the container is running, open your browser and go to:  
```
http://127.0.0.1:5000
```

PROJECT STRUCTURE  
```
/minimal-flask-chatbot-docker
│── imgs/
│   └── image.png         Screenshot of the chatbot UI
│── docker-compose.yml    Docker Compose file for running the chatbot
│── LICENSE               Project license
│── README.md             Project documentation
```

STOPPING THE CHATBOT  
If you want to stop the chatbot, use:  
```sh
docker-compose down
```
This will shut down the container, but the image will remain downloaded, so next time you start it, it will be faster.

CONTRIBUTING  
Feel free to fork this repository and improve the project. Contributions are welcome.  

If you want to modify the code, check the original repo:  
[Minimal Flask Chatbot (Source Code)](https://github.com/Aleexc12/minimal-flask-chatbot)

LICENSE  
This project is licensed under the MIT License.
