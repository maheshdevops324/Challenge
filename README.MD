This package containins 3 files

1. userdata.json
2. serveJson.py
3. Dockerfile

Please ensure in your machin docker is installed
1. Place all the 3 files in one location and run below command

docker build -t pythonimage . 

please note that pythonimage is just the name, feel free to replace it with your own tag

2.Once the build is completed succefully, run the following command

docker run -d -t -i -p 80:80 pythonimage

3. Test is by using the below url

http://<YOUR_MACHiNE_IP>/users

It should display the contents of userdata.json file
