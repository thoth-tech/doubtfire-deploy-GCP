# OnTrack Deployment on GCP with Watchtower

Watchtower is a container based solution for automating docker container base image updates.
[Watchtower Documentation](https://containrrr.dev/watchtower/)

## Steps

1. Create a VM within GCP Compute Engine section
2. ssh into machine
3. Update machine `sudo apt update && sudo apt upgrade -y`
4. Install Docker by following the steps to install docker and docker compose with the convenience script on at [this link](https://docs.docker.com/engine/install/debian/#install-using-the-convenience-script).
5. Follow the steps in the DEPLOYING.md file to complete the setup but instead of using the `docker compose up` command use the `docker compose -f docker-compose-watchtower.yml up`.