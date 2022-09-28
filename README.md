# Experience:
The following contains some brief information about my current experience in DevOps.

## Cloud & Dev Ops
### Explanation of cloud:
Cloud as a role involves the connection of applications to the internet put simply. This role involves taking applications that have been created and creating the necessary infastructure to connect them to dependant applications, such as a Database, as well as making the application accessible on the internet. This role involves the utilization of many different tools in order to create a product that can be easily updated, maintained and pushed to production. Cloud also utilizes a more forward thinking resource model, with data centers being used rather than on site server racks.

### AWS:
- Deployed multiple AWS instances.
- Created a VPC using terraform.
- Developed a pipeline that can automatically update an application based on a push to the main branch on github.


### Benefits of using Cloud
There are many benefits to Cloud but perhaps the most notable one would have to be the benefit of using Data centers over on site servers. The pay as you go model that many different cloud providers offer allows companies to better allocate resources to their applications and respond to demand much faster than they previously could using On Site resources. With this flexibility in the way companies can attack publication of their products, it has never been easier for companies of all sizes to maintain and publish their products.

## CICD
### Explanation of CICD:
CICD stands for continuous integration continuous development. It basically is the idea that every change we make to our application should be consistently pushed to the deployed verion of our application, meaning that small updates to an application are constantly being made and deployed. This benefits the company in many ways but perhaps the most invaluable is the feedback that they can procure from users. Since CICD pipelines make it a very simple manner to push the latest changes to deployment, the response to those changes are much faster and more accurate than traditional larger updates, the user in this situation is essentially the beta tester for whatever features or changes development teams are currently working on.

### Jenkins
- Created a Jenkins Pipeline that could automatically deploy an application when a push was made to the main branch on GitHub.
- Configured this pipeline to create an AWS instance.

### Packer
- Set up multiple AMI's that could be re deployed and utilized by programs like Terraform to make the instantiation of instances more efficient.

### Benefits of CICD:
The main benefit of CICD is that you are always updating your application. Every change you make will get feedback the moment you finish a working version of that change after it's deployed using a CICD pipeline. This allows companies to rollback changes that recieved negative criticism from users, or to focus more on changes that recieved positive feedback from users.



## Jenkins
### Explanation of Jenkins:
Jenkins is a tool that is used to create CICD pipelines. It facilitates the connection between your github repository and your production instances, allowing your main branch changes to be pushed to production.

- Created a pipeline that connected a GitHub application to AWS, instantiating the changes made whenever a change was made to main.
- Created a couple basic projects using Jenkins, utilized scripts to rsync the files to the AWS instance.


### Benefits of using Jenkins
THe main benefit of Jenkins coincides with the benefits of CICD. Your changes are always pushed to production, at least in the use case I have experienced. Jenkins is heavily configurable, and can be made to do all sorts of actions depending on the use case. It is an invaluable tool when it comes to automating traditionally strenuous time consuming tasks.




## Provisioning
### Explanation of Provisioning:
Provisioning is a term used to describe the setting up of an environment in order to make it useable by anyone who wants to either use, test or develop an application. Provisioning in Cloud specifically let's us create scripts and utilize tools that install all the dependancies needed for someone to get a working version of our application with a single command.

### Vagrant
- Created multiple Vagrant Environments, and interconnected them.
  - NodeJS Env
  - MongoDB Env
  - MySQL Env
  - React Env
- Wrote bash scripts for each of the environments that install the required dependancies.


### Terraform
- Created multiple terraform environments.
  - AWS Instance creation
  - MySQL 
- Utilized packer for the AMI selection.

### Benefits of Provisioning:
The largest benefit of creating infastructure for provisioning is that you do not need to worry about user specific errors when it comes to handing your application to someone else. The provisioning scripts in conjunction with tools like Vagrant allow any user with Vagrant installed to recieve a working version of your application without having to worry about installing all the dependancies needed, as well as not worrying about any OS environment errors that could have occured if they had tried to run your application on their host machine. 


## Networking
### Explanation of Networking:
Networking is the act of creating connections between different applications and managing those connections. It involves manging the networks that applications themselves utilize to interact with each other and the user base.

- Created a VPC using terraform
- Learned about the importance of the composition of an IPV4 address and how each individual octave affects subsequent octaves.

### Benefits of Networking:
The main benefits of Networking are that the person working on the Network can better serve the needs of each application. From forwarding ports to creating security rules that prohibit or allow access in to your application, you can better regulate traffic and prevent possible security risks based on the Network you have created. Without networking, the internet would not be able to regulate this traffic nearly as efficiently if at all. A basic understanding is required to create any sort of connection on the internet.
