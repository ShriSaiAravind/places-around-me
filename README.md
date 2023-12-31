# Places Around Me
## AIM:
To develop a website to display details about the places around my house.

## Design Steps:

### Step 1:
Creating Repository:

    First, a path to make a folder where git needs to be created is identified.
    Fork the repository (https://github/gowriganeshns/places-around-me)
    Clone the repository

    git clone https://github.com/ShriSaiAravind/places-around-me 

After cloning the folder with the repository name places-around-me will be created
### Step 2:
>Write the following commands

    cd serverside

    django-admin startproj myproj

    >Then move into the folder myproj where manage.py file is located. Now give the commands to create myapp

    python3 manage.py startapp myapp

    .Then change the necessary settings in the settings.py.

    from pathlib import Path
    import os

    ALLOWED_HOSTS = ['*']

    INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'myapp'
    ]
    STATICFILES_DIR=[
    os.path.join(BASE_DIR,'static')
    ]

    >Now go to /home/sec/FWAD/ex04/places-around-me/myproj and type the following commands
     
     1. mkdir static
     2. cd static
     3. mkdir html
     4. cd html
     5. touch garden.html
     6. touch ground.html
     7. touch home.html
     8. touch lake.html
     9. touch park.html
     10.touch map.html

     >Select the image file required for the project, go to imagemap.org and use the tools provided to create html code for image mapping, and paste the code in map.html

## Code:


1. map.html 

        <html>
            <head>
                <title>Server test</title>
            </head>
            <body>
                <h1>imagemaps demo</h1>
                <img src="Locality.jpeg" usemap="#image_map">
                <map name="image_map">
                    <area alt="home" title="home" href="home.html" coords="669,502,772,555" shape="rect">
                    <area alt="lake" title="lake" href="lake.html" coords="598,115 816,120 925,5 612,3 " shape="polygon">
                    <area alt="park" title="park" href="park.html" coords="158,315,86" shape="circle">
                    <area alt="ground" title="ground" href="ground.html" coords="1163,703,201" shape="circle">
                    <area alt="garden plot" title="garden plot" href="garden.html" coords="439,632,131" shape="circle">
                </map>
            </body>
        </html>

2. park.html

        <!DOCTYPE html>
        <html>
            <head>
                <title>park</title>
            </head>
            <body>
                <h1>local park</h1>
            </body>
        </html>

3. lake.html

        <!DOCTYPE html>
        <html>
            <head>
                <title>lake</title>
            </head>
            <body>
                <h1>local lake</h1>
            </body>
        </html>

4. home.html

        <!DOCTYPE html>
        <html>
            <head>
                <title>house</title>
            </head>
            <body>
                <h1>This is my house </h1>
            </body>
        </html>

5. ground.html

        <!DOCTYPE html>
        <html>
            <head>
                <title>Cricket ground</title>
            </head>
            <body>
                <h1>local cricket ground</h1>
            </body>
        </html>

6. garden.html

        <!DOCTYPE html>
        <html>
            <head>
                <title>Garden</title>
            </head>
            <body>
                <h1>local garden</h1>
            </body>
        </html>

## Output:

Imagemap interface : 

![imgmap](https://github.com/ShriSaiAravind/places-around-me/assets/148180918/044f6fc7-25fa-4013-84cf-7ff7f8abc790)


House interface:

![Screenshot from 2023-11-27 13-16-12](https://github.com/ShriSaiAravind/places-around-me/assets/148180918/06bc82e6-e67c-4fd4-bbca-12bad845b765)


Garden Interface:

![garden](https://github.com/ShriSaiAravind/places-around-me/assets/148180918/35dc99dd-93a1-46ff-a39e-78f20030aaed)


Park Interface:

![park](https://github.com/ShriSaiAravind/places-around-me/assets/148180918/1987c39a-57d3-4117-a59a-fdaceb40f56e)


Ground Interface: 

![ground](https://github.com/ShriSaiAravind/places-around-me/assets/148180918/94c9a1e8-eeaf-45c2-8047-805e62a1ae15)


Lake Interface: 

![lake](https://github.com/ShriSaiAravind/places-around-me/assets/148180918/847bf366-0478-49ee-9685-10111f7f0dda)


## Result:

Imagemap interface has been created succesfully.
