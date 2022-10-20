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

## Principle Of Least Privelage:
### Explanation of Principle of Least Privelage
This principle is based on the concept of giving no access to an application or service to any user to begin with, and slowly granting access on a need to access basis as the application develops. This shores up possible holes in the security of your application by giving access purposefully, rather than restricting access based on a users permissions.


### AWS
Aws is a great example of this, for nearly every service on AWS by default access is incredibly restricted. In company accounts, you have to explicitly give access to even the tools that AWS has to sub users which may seem a bit overkill with how difficult it is to access AWS in the first place, but in reality adds much needed security to what could be considered one of the most vulnerable aspects of any application. By restricting access by default, AWS keeps sub users in a company from accidentally, or possibly maliciously, destroying months or even years worth of work.

### Benefits of The Principle Of Least Privelage:
The largest benefit to this principle is the knowledge that your application is far more secure from conception than it would be if the application was constructed with open permissions. If you have to explicitly give access to manage your application, the odds of an attack against your application decrease exponentially.


## IAC
### Explanation of IAC
IAC stands for infrastructure as code. The idea behind it is to remove the human error that comes from manual configuration of infrastructure. This can realate to a multitude of tools and applications used in DevOps but essentially it replaces the manual configuration of environments or instances with coding tools which have the benefit of not only being reusable, but consistent.

### Terraform
- Created AWS EC2 instances using Terraform

### Vagrant 
- Created multiple VM's using Vagrant that utilize provisioning scripts to create reusable easy to access environments.

### Benefits of IAC
THe largest benefit of IAC is that your environment will always be configured exactly the same every time you run your IAC config file. Whereas before you would have to create something like an EC2 instance manually, slecting the AMI, VPC, and security groups inside the AWS console, tools like Terraform allow the creation of identical instances with a single command. These config fills can be re used and re tooled depending on the use case, which decreases the time spent setting up environments for testing or deployment.


## Terraform and Packer
### Explanation of Terraform and Packer
Terraform and Packer are tools that help orchestrate infrastucture configuration. These tools allow us to take a snapshot of an applications desired state then utilize it in a IAC config file to make deployment to cloud providers like AWS both quick and easily reproduceable.

- Created multiple Packer AMI's
  - NodeJS
  - MongoDB
  - MySQL
- USed Terraform to deploy these AMI's to an EC2 instance

### Benefit of Terraform and Packer
The main benefit of Terraform and Packer is that you never have to access your specific cloud providers console to spin up an instance. WIth a single command you can recreate an environment for your application and destroy it just as easily. This saves you time, and keeps every single instance you create consistent since it removes the possibility of human error when configuring an instance in between changes.


# Extended Glossary

## AWS
### Explanation of AWS
AWS is a cloud provider that has too many uses to list here. I have primarily used AWS for file storage and web hosting. The tools AWS provides are invaluable, allowing anyone in the DevOps space to efficiently host web applications.

- Created multiple EC2 Instances
  - SQL Database
  - MongoDB Database
  - Node App
  - React App
- Utilized S3 Bucket for File Storage

## Benefits of using AWS
Simmilar to Cloud, the benefits of AWS mainly include the Pay as You go model of web hosting, as well as removing the need for infrastructure held directly on your companies property. Load balancing is far easier, and monitoring is more streamlined and easier to set up. AWS is also easily connected to a multitude of Devops applications such as Terraform, Ansible, or Packer.

## Javascript
### Explanation of Javascript
Javascript is a programming language that is closely tied to web applications. It is a high level programming language and one of the more easy to grasp programming languages for beginners. You can modify HTML code with Javascript and add programming fucntionality to your web applications. Most of the internet today uses Javascript in one form or another.

- Created a WebApp game utilizing pure JS and HTML
- Created Multiple WebPages

### Benefits of using Javascript
There are many benefits to using javascript but perhaps the most important is the ability to progmatically audit web pages. This allows web pages to become more advanced in what they can do, from items like conditional rendering, to mapping over API data in order to quickly and easily insert data from the internet into a website. Without Javascript the internet would be a very different place and it's use case has only increased in the past decade.


## React
### Explanation of React
React is a JS library that is commonly used. It was developed by Facebook (now Meta) and is Open Source. The idea of React was to compartmenalize every single section of a webpage, and allow the HTML to be written alongside the Javascript. React uses Containers and Components to render each section of a webpage and utilizes tools such as State, Effect, and Props to make displaying information cleaner and more readable. React apps are far more maintainable than pure Javascript HTML Web Apps.

- Created Multiple React Applications
    - Beer search page that connects to a public API and maps over all the data and allows searching and filtering through that data
    - Weather Log Page that connects to a public API and then logs over the data to create a history of everytime a location has been searched.
    - Instagram Profile Page clone (limited functionality)

### Benefits of using React
The largest benefit of using React is that your code becomes far more maintainable. Instead of one gigantic JS file and however many HTML files, you combine HTML and Javascript into one easy to read JSX file structure. Along with this idea, your components and containers are REUSEABLE, meaning you can call that same component wherever you want in your webapp multiple times and pass it different information each time. This streamlines the construction of web applications in React making it a far better choice than pure JS.
