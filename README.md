CD in the cloned repository

`docker-compose up -d `  
Ensure that http://your.DomainName.ext is up  
`docker exec -it certificate-generator bash`  
`certbot certonly --manual -d your.DomainName.ext`  

With GUI or another shell
- Create a file at `/nginx/well-known/acme-challenge` 
- Name it with certonly's shortest provided string. 
- Put the longest string as the content  

Hit enter  in the prompt  

📜 Find your newly generated certificate(s) in `/certificates` ! 🎉

NB: nginx and letsencrypt logs can be found in the `logs` folder  