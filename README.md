Rashmitagudinho
b7de2dbcea694057b3663ddc47bfa19c

dockerfile
echo FROM httpd:2.4 > Dockerfile
echo COPY index.html /usr/local/apache2/htdocs/ >> Dockerfile

terraform
provider "aws" {
region = "us-east-1" # Change to your desired region
}
resource "aws_s3_bucket" "example_bucket" {
bucket = "my-unique-bucket-name" # Replace with a globally unique name
acl = "private"
}

7th jenkins
echo ^<html^>^<body^>^<h1^>Hello from Dockerized Web App!^</h1^>^</body^>^</html^> > index.html

echo FROM nginx:latest > Dockerfile
echo COPY index.html /usr/share/nginx/html/index.html >> Dockerfile

build steps
docker rm --force container1
docker build -t nginx-image1 .
docker run -d -p 8081:80 --name=container1 nginx-image1

5th jenkins
built steps
echo "Deploying from C:/ci-cd-webapp to Apache htdocs..."
rm -rf /c/Apache24/htdocs/*
cp -r /c/ci-cd-webapp/* /c/Apache24/htdocs/
echo "Deployment completed!"
 trigger
 cd C:\ci-cd-webapp
echo <p>Deployed by Jenkins webhook</p> >> index.html
git add .
git commit -m "Update content via webhook"
git push


cloud
steps:
-name: 'gcr.io/cloud-builders/gsutil'
args: ['-m', 'rsync', '-r', 'web-pages/', 'gs://your-bucket-name']

