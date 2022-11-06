### Jenkins
You should run Jenkins at first with the docker-compose that located in the project. After running Jenkins you should
copy the admins password for jenkins via logs of Jenkins.

### Configure Node
Jenkins by default has a built-in node. but it's better for us to config our local machine as a new node and run our pipeline
on that, to config node we should go through below steps:
* Go to Manage Jenkins Section from the left menu
* Go to Manage nodes and Clouds
* Click New Node
* Set node name and click permanent agent

Now we have to run jenkins agent on the local computer, to do that we have to run the following steps:
* Click on the node that we config previously.
* Now copy and run the commands that you see on your computer 

Congratulations you set up a node. now we have to disable the built-in node to run all pipelines with this node.
* Click on built-in node
* Go to configure section
* Change usage value from 'Use this node as much as possible' to 'Only build jobs with label expressions matching this node'


### Setup Pipeline
On this project we have different jenkins file for adding this files you should go through the following steps:
* Click on the new item bottom
* Set a name for your pipeline and click on pipeline and then click on create
* copy the jenkins file on pipeline section
