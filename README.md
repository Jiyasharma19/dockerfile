# dockerfile


1: to create a docker file


mkdir dockerfile

cd dockerfile

touch dockerfile

2. to write command in our dockerfile


vim dockerfile

#press i(to insert commands)

FROM alpine

RUN apk -U upgrade

CMD["echo","HELLO WORLD"]

#for exit:esc wq enter

cat dockerfile

3:to build an image:

docker build -t[image name:tags]

4:to check for the image and can run it

docker images

docker run -i -t[image name with tags]

5: deploy on docker hub via docker login

docker tag imagename

dockerhubusername/imagename docker images

docker push dockerhubusername/imagename
##your image is now pushed on repository of imagename
