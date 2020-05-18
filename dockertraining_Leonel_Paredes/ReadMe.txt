docker build --tag dockertrainingleonelparedes .
docker run -dt -p 8484:80 --name Site1 dockertrainingleonelparedes
docker run -dt -e "CustomStoreSettings:StoreName=Plano" --name Site2 -p 8585:80 dockertrainingleonelparedes