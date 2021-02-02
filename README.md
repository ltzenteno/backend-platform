### Backend platform

based on [https://github.com/ltzenteno/python-dockerized-template](https://github.com/ltzenteno/python-dockerized-template)

Project that contains an API with:

1. Listing of Universities in MX
2. Group them by State
3. Retrieve collections

### Installing new Dependencies

to install new python dependencies, with poetry (i.e. "djangorestframework"):

	docker-compose exec backend sh -c "poetry config virtualenvs.create false && poetry add djangorestframework@^3.12.2"

you can use `-D` if the package is a development dependency

**NOTE:** _don't forget to commit `pyproject.toml` and `poetry.lock` changes after installing the new dependency_

#### Rebuilding images: 

	docker-compose build

#### Rebuilding existing container:

First remove the container (i.e. `backend` container)

	docker-compose rm -sfv backend

and re-run it again
	
	docker-compose up -d backend

**TODO: keep adding stuff to README**
