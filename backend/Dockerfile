## recover node image from dockhub, version is specified
FROM python:3.13.0

# define the working directory inside the contener as being /code The app will lives here
WORKDIR /app

# copy the requirements.txt file from the current directory
COPY requirements.txt ./

#first run pip upgrade to update the pip packet manager then install all dependencies from the requirements.txt file
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# copy all the file of the app
COPY . .

# run the flask run command once everything else is done
CMD ["flask", "run"]