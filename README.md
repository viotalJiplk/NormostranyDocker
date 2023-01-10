# Docker container for "WEB TOOL FOR ESTIMATION OF DOCUMENT SIZE"
Original project: https://github.com/SimonaK11/Normostrany
This project is based on *python:3.7.3-stretch* so it is not going to run on Windows.
## How to run the project
### With docker compose
1. Install **Docker**
2. Download `docker-compose.yml` from root of this repository
3. Run `docker compose up -d`
The application is going to run on the adress `http://127.0.0.1:8080`. The tool is on the /standardpages endpoint.
4. Setup reverse proxy for accepting traffic from other ports and ips. Sample nginx config is in `src/nginx`.

### How to run the project Manualy
1. Install **Docker** 
2. Clone this repository
3. Go to subfolder src
3. Rename `.env-template` to `.env` 	
5. *Change port in .env*
6. Run `docker compose build`
7. Run `docker compose up -d`
8. The application is going to run on the adress `http://127.0.0.1:8000`. The tool is on the /standardpages endpoint.
9. Setup reverse proxy for accepting traffic from other ports and ips. Sample nginx config is in `src/nginx`.
