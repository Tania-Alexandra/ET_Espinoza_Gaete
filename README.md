# ET_Espinoza_Gaete
@echo off
cd Suculovers/proyectosDjango/TestDjango
#echo Activando el entorno virtual...

echo Aplicando import...
pip install django
pip install django-crispy-forms
pip install crispy-bootstrap5
pip install pillow
pip install djangorestframework


echo Aplicando migraciones...
python manage.py makemigrations 
python manage.py migrate 
python manage.py collectstatic


echo Iniciando el servidor...
python manage.py runserver
