### Backend platform

based on [https://github.com/ltzenteno/python-dockerized-template](https://github.com/ltzenteno/python-dockerized-template)

Project that contains an API with:

1. Listing of Universities in MX
2. Group them by State
3. Retrieve collections

### Installing new Dependencies

to install new python dependencies, add them to the `pyproject.toml`

then rebuild the image with `docker-compose build`

then remove backend container with:

	docker-compose rm -sfv backend

and re-tun it again
	
	docker-compose up -d backend

**TODO: Create README**
