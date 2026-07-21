# feed-this-much
## How to feed your pets?  
II1305 Project 

View Figma prototype [here](https://www.figma.com/proto/Mjxv02iieleyZnnUAyROZ9/KTH-II1305---Feed-This-Much?node-id=2033-1210&p=f&t=2Xsp7OIooKN6pQoU-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=2004%3A748&show-proto-sidebar=1).

watch the demo video here:

[![DEMO VIDEO](http://img.youtube.com/vi/x_qqiNi8j6I/0.jpg)](http://www.youtube.com/watch?v=x_qqiNi8j6I "Feed this much app demo")

# Windows
If you are using Windows, you can install WSL and follow the rest of instructions. 

# Folder structure

**backend**: all the code regarding the django backend
**frontend**: all the code regarding the react frontend

# How to set up local env
Project has some dependencies that need to be installed. We use `uv` package manager to handle the dependencies. 

**uv**: Use the link (https://github.com/astral-sh/uv) to install

Create the virtual environment by running `uv venv`
Activate the virtual environment by running `source .venv/bin/activate` and run `uv sync` to install the dependencies

Navigate to `frontend/feed-this-much-client` and run `npm i` and `npm install next`

## How to run django development server locally
Set the following env var by running `export DJANGO_DEBUG=True`.

Navigate to `backend` folder and run `python manage.py runserver`

### How to run backend unit tests locally
Navigate to `backend` directory and run `uv run python manage.py test`

### How to run python linter (ruff) locally
Run the command `uv run ruff check .` in the root folder

## How to run NextJS (ReactJS) development server locally
Navigate to `frontend/feed-this-much-client` folder and run `npm run dev`

### How to run javascript linter locally
Navigate to `frontend/feed-this-much-client` folder and run `npm run lint`
