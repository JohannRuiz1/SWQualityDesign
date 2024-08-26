#### Readings and Notes:
[The link between software quality and software maintenance](https://canvas.vt.edu/courses/196107/files/34303068/download?wrap=1 "rg49-51.pdf") by Robert Glass

- A software with good quality has (ranked on how it relates to maintenance):
	- Understandability: Comments and Documentation
	- Modifiability: Configuration as Code, modular/decoupled components, 
	- Reliability: Unit testing, integration testing, system testing
	- Efficiency: Use optimal algorithms for time and space, free up resources when unneeded, test software for speed and space 
	- Testability: Design concept, use interfaces to be able to mock, abstract code into methods for more testable components (No monolithic methods)
	- Human engineering: UI/UX design 
	- Portability: Containerization of software (Docker), make it platform agonistic   
- Software Maintenance: keeping software functioning to the standard of a user, ie meeting Service Level Agreements (SLAs)
- Software quality and software maintenance go hand in hand
- Poor quality = future maintenance that will be needed
- Ensuring the software quality standards are met will result in less time needed to maintain the product

[Can you MANAGE quality into a software product?](https://canvas.vt.edu/courses/196107/files/34303074/download?wrap=1 "rg147-149.pdf") by Robert Glass
- You cannot manage quality into software product
- The attributes that ensure quality (seen above) are technical concepts that are not (and should not) be of concern to a manager
- For example, a manager shouldn't be concerned if your code is containerized, or if they are properly using Javadocs, they should be concerned with managing the person
- Personally, there are some managers that are more technical ie they also do the work, so it could be managed in some sense if they are the ones approving merge requests and providing the definition of done for certain tasks
- Managers job is to create quality climate
	- Processes are in place to facilitate and ensure quality
	- Tools are provided to assist in quality
	- People who think quality are hired
	- Quality is a top priority in conversation
- Delay in software products often result in a loss of quality
	- Normal Equation: Software Product = on schedule + within budget
	- Should be: Software Product = quality + on schedule + within budget
- 

[Chapter 14: Quality Concepts](https://canvas.vt.edu/courses/196107/files/34303093/download?wrap=1 "Pressman-quality.pdf") by Roger Pressman


#### Questions:
1. Robert Glass does not include all of the quality attributes that are in McCall's list of quality factors. Do you believe the extra attributes in McCall's list are necessary for "quality" software, or is Glass' definition sufficient? Justify your answer.
    
2. In Glass' definition, which single attribute do you believe is most important, and why?

I believe *reliability* is the most important software quality attribute within the list. The way I landed on this was by thinking about a software product that lacks one of these attributes, and determining which have the biggest impact on maintenance. If the perspective was shifted onto the biggest impact on the user instead of maintenance, then obviously *human engineering* would be the most important attribute; therefore, it's necessary we focus on maintenance. In personal experience, there is nothing more frustrating about software when it doesn't behave on to your expectations. If a software product is not reliable on performing the actions it was created to do, then it's essentially useless because it will not find it's way to production. And if the unreliable product was in production, then it would be the maintainer's job to fix it every time it started to misbehave. In the realm of Site Reliability Engineering (SRE), software services in production have to meet a Service Level Agreement (SLA), which is a contract stating metrics your software has to meet. For example, there could be an SLA that latency of your product would go over one second for end user interactions. It's not a coincident that SRE has the world reliability in the name; there has been an entire career created out of ensuring software products are reliable. Therefore, I believe without reliability in your software, then software's value automatically degrades, or your software maintainer is going to start looking for a new job.
#### Answer:

