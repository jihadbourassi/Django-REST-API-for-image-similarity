
HOW TO INSTALL AND USE THIS PROJECT :


- INSTALLATION :


1- INSTALL PYTHON 3.7.1  (https://www.python.org/downloads/)

2- INSTALL PIP (https://pip.pypa.io/en/stable/installing/)

3- CD INSIDE THE PROJECT AND USE THE PIP COMMAND TO INSTALL THE REQUIREMENTS VIA THE FOLLOWING COMMAND (pip install -r requirements.txt)
   note : for the annoy library you will need to install "visual c ++ build tools" first


- USAGE : 

(SKIP 1-2-3 IF YOU WANT TO TEST WITH THE EXISTING MODEL AND DATABASE OF VECTORS)


1- CD INSIDE THE APP FOLDER (/app), DELETE THE /image_vectors  FOLDER AND VECTORIZE THE DATABASE OF IMAGES VIA THE COMMAND (python vectorize_database.py "/path/to/the/database/of/images")

2- RENAME THE VECTORS BY PUTTING THE FULL PATH TO THE /image_vectors FOLDER IN THE rename.py FILE AND USE THE FOLLOWING COMMAND ( python rename.py) note : only rename the files that contain two "." in the name

3- DELETE model.ann FILE IF IT EXISTS AND CREATE THE MODEL BY USING THE COMMAND ( python database_model.py)

4- CD .. BACK INTO THE MAIN DIRECTORY

5- RUN THE LOCAL SERVER VIA THE COMMAND (python manage.py runserver)

6- OPEN THE FOLLOWING LINKS : 

- http://127.0.0.1:8000/vector_img/ FOR UPLOADING AND VECTORIZING AN IMAGE

- http://127.0.0.1:8000/similarity/ FOR UPLOADING THE VECTORIZED IMAGE (.npz file) AND COMPARING IT TO THE DATABASE
