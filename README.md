
# TALLER 9 LLM
# Descripción 
Para este proyecto se usa Python y la API de OpenAI con el fin de crear un prompt donde podamos hacer consultas propias con el fin de poder utilizar una base de datos vectorizada de Pinecone para obtener un contexto propio que retorne resultados personalizados sin hacer pública la información.
## DESARROLLADO CON
* [Python 3.11 o superior](https://www.python.org/) - Lenguaje de programación usado.
* [Pip 24 o superior](https://pypi.org/project/pip/)- Gestor de dependencias del proyecto

## Pasos para ejecutar
1. Debemos clonar este repositorio
```bash
git clone https://github.com/Sebasian-Cepeda/lab9.git
```
2. Hacemos un "cd" al repositorio clonado
```bash
cd lab9
```
3. Abrimos el proyecto en pycharm para mayor facilidad

4. Escribimos el siguiente comando para instalar las dependencias con pip
```bash
pip install -r 'requirements.txt'
```
5. Ahora podemos probar cada archivo para ver su funcionamiento, no obstante se nececita de una API key de OpenAI y de Pinecone válidas y activas de lo contrario no funcionaran los archivos
![image](https://github.com/Sebasian-Cepeda/lab9/assets/89321404/0bd21e01-ee4e-4b29-bbd7-229f6dbd736a)
![image](https://github.com/Sebasian-Cepeda/lab9/assets/89321404/e7b28407-744c-46d5-8be0-9772c06b98bf)

si corremos Llmmemorydb.py y OpenAI.py obtenemos el resultado de la imagen anterior, por desgracia no podemos ver el resultado del archivo restante pues la llave de OpenAI se vencio y no contamos con otras para mas pruebas
 
# Diseño
Llmmemorydb.py: Se utiliza como contexto la información de un repositorio de GitHub para luego con esa información hacer una consulta a ChatGPT para obtener un resultado personalizado.

OpenAI.py: Se hace una consulta directamente a ChatGPT por medio de su API.

Pinecone.py: Se usa un archivo "pinecone.txt" copiando el contenido del mismo para crear una base de datos vectorizada en Pinecone, para luego consultar sus vectores y obtener ese contenido como respuesta a la consulta "who is ricardo ajorna".

## AUTOR
Juan Sebastian Cepeda saray
