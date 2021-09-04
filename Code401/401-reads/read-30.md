## Docker 

    Docker is used to isolate and run entire applications. The entire development environment is isolated: programming language, software packages, databases, and more. With Docker we now longer have to mess around with virtual environments. We can faithfully reproduce a production environment locally
    Downside: Complexity

## Containers vs Virtual Environments

    Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great. But virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version.

## Docker Installation

    sudo pip install docker-compose

## Django REST API

    Django REST Framework works alongside the Django web framework to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured. he most important takeaway is that Django creates websites containing webpages, while Django REST Framework creates web APIs which are a collection of URL endpoints containing available HTTP verbs that return JSON.

## Views 

    Next up is our views.py file which relies on Django REST Framework’s built-in generic class views. These deliberately mimic traditional Django’s generic class-based views in format, but they are not the same thing.

## Serializers 

    A serializer translates data into a format that is easy to consume over the internet, typically JSON, and is displayed at an API endpoint. We will also cover serializers and JSON in more depth in following chapters. For now I want to demonstrate how easy it is to create a serializer with Django REST Framework to convert Django models to JSON.

