# feed-this-much
## How to feed your pets?  
II1305 Project 

A group project where we created a React web app for dog and cat owners. The Feed This Much web app helps pet owners create personalized feeding plans tailored to their pets' specific needs based on current (2024) scientific nutritional guidelines by the European Pet Food Industry Federation (FEDIAF).  It calculates the amount of food to give a pet, including a combination of two different foods, and can divide this over a custom number of meals.

I was the Product Owner for the project and as part of this role I divided the features of the product into tasks which could be completed within sprints, and communicated the needs of the users to the developers.  I was also a developer, and worked mostly with the front-end development to create the custom forms using React, JavaScript, TypeScript, Shadcn components, and Zod form validation.  I also did the research to get the formulas used to calculate the nutritional needs of the dogs and cats, assisted in the configuration of the database and API, and contributed to the functionality of the calculation logic and API connectivity in Python.  I also created an initial Figma prototype (not all the pages, due to time constraints, but it was used as a starting point so the team could visualize what we were aiming for).

Note: the app is no longer live, but a video demo is available.

[Expo Website](https://teamrecurrent.wixsite.com/feed-this-much-expo)

[Main Github](https://github.com/bobach/feed-this-much)

[My Contributions](https://github.com/bobach/feed-this-much/commits?author=aliciavanzijl)

[Figma Prototype](https://www.figma.com/proto/Mjxv02iieleyZnnUAyROZ9/KTH-II1305---Feed-This-Much?node-id=2004-748&starting-point-node-id=2004%3A748&t=fMw60tPSMevIzzOb-1)

watch the demo video here:

[![DEMO VIDEO](http://img.youtube.com/vi/x_qqiNi8j6I/0.jpg)](http://www.youtube.com/watch?v=x_qqiNi8j6I "Feed this much app demo")


## Setup Notes:
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
