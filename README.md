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
