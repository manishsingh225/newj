## The Makefile includes instructions on environment setup
# Create and activate a virtual environment
# Install dependencies in requirements.txt

setup:
	# Create python virtualenv & source it
	# source ~/.devops/bin/activate
	sudo apt install python3-venv
	python3 -m venv newj-assign
	source newj-assign/bin/activate

install:
	# This should be run from inside a virtual environment
	# Install packages from pip, use requirements.txt
	pip install -r requirements.txt

docker-build:
	# add commands required
	docker build -t manish/newj-assign:v2 .
	sudo docker run -p 8000:8000 manish/newj-assign:v2
docker-push:
	# add commands required
	# change tag to have dokcer repo name
	docker tag manish/newj-assign:v2 manish225/newj-assign:v2
	docker push manish225/newj-assign:v2