# Arem-TallerPatronesArquitectura

#### Developed by:
>Diego Andrés Borrero Muñoz - 2103110  
Student of System Engineering   
Escuela Colombiana de Ingeniería Julio Garavito.

## AWS Instructions
Have the EC2 virtual machine created with the security permissions to access to the 61616 port

Power on your machine

Use the terminal to connect by ssh to the virtual machine

Use the following lines in the terminal to get the 7.0.1 version of ServiceMix, set the correct routing for the messages and execute the ServiceMix:

```bash
wget https://www-us.apache.org/dist/servicemix/servicemix-7/7.0.1/apache-servicemix-7.0.1.zip  
unzip apache-servicemix-7.0.1.zip  
cd apache-servicemix-7.0.1/deploy/  
wget https://raw.githubusercontent.com/DxMortem/Arem-TallerPatronesArquitectura/master/MessageRoute.xml  
cd ..  
./bin/servicemix```

Then clone the repository, change "localhost" on the connection factory constructor for the virtual machine ip (in Client and HelloWorldConsumer classes).

Execute first the Client class and then the HelloWorldConsumer class, you have to see printed the message previously sended by the Client.

Please dont forget of terminate and delete all the things related of the EC2 machine after the test.
