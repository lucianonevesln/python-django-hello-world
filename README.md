# Estudo: Django

## Objetivo:

### Dar os primeiros passos na aquisição de conhecimento desse framework.

## Comandos Úteis:

### python -m venv venv: criando ambiente virtual;

### .\venv\Scripts\activate: comando para ativar o ambiente virtual;

### deactivate: comando para desativar o ambiente virtual;

### pip install Django: comando para instalar o framework;

### python -m --version Django: comando para verificar versão;

### django-admin startproject helloworld: comando para criar um projeto novo;

### python manage.py startapp home: comando para criar nova pasta;

### python manage.py runserver: comando para executar a aplicação web;

### helloworld/home/views.py: inserir 'from django.http import HttpResponse';

### helloworld/home: criar arquivo urls.py e inserir from 'django.urls import path', 'from . import views' e

urlpatterns = [
    path('', views.index, name='index')
];

### helloworld/urls.py: inserir 'from django.conf.urls import include' e 'path('home/', include('home.urls')),' em urlpatterns, conforme abaixo

urlpatterns = [
    path('admin/', admin.site.urls),
    path('home/', include('home.urls')),
];

## Imagem:

![alt text]()