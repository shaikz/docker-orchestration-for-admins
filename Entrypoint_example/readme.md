to convert the dos file to unix format file use below  command
sed -i -e 's/\r$//' entrypoint.sh
chmod +x entrypoint.sh

docker build -t cowsay .

docker run -it --rm --name moo cowsay

docker run -it --rm --name moo cowsay you rock!