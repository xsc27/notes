## Customer Obsession

> Leaders start with the customer and work backwards. They work vigorously to earn and keep customer trust. Although leaders pay attention to competitors, they obsess over customers.

* **Situation**: Many unused and old AWS resources, which was exacerbated from having term based contractors frequently rotating out.
* **Task**: As an engineer in operations, my customers were the service teams.
* **Action**:  Designed and implemented Policy-As-Code service for compliance enforcement.
	* MVP: Queried accounts to find resources I believed could be removed.
	* Identified early adopters, that would be open to test purging resources.
	* To gain buy-in/trust, I shared the report with the engineers and would only make the changes they approved.
	* To gain further trust/buy-in, shared report with wider org. Also, early adopters became advocates after seeing the impact to the AWS bill.
	*  Collaborated with account owners to identify their needs/requirements. Introduced security checks that would meet minimum resistance.
	* Gain more customers by reaching out to SecEng to demonstrate how they can approve and deny policy exceptions through git.
* **Result**: (Improved UX) Simplified management of the infrastructure, which customers did not know they needed.
	* Value: Lowered cost and improved security posture for service teams.
	* Empowered SecEng with visibility and approvals.
		* Growth: Expanded user base (new customer).
	* Improved relationships with customers enabling being able to suggest features rather than waiting for requirements.
	* Gave visibility to management (and broader company) through Datadog dashboards to see in vs out of compliance per account.
	* External customers data was now more secure, even though they would not know.

## Ownership

> Leaders are owners. They think long term and don’t sacrifice long-term value for short-term results. They act on behalf of the entire company, beyond just their own team. They never say “that’s not my job."

* **Situation**: Needed to spin up a test environment to develop the build of a new server type. The provisioning system for physical infra was owned by another team. The documentation was very verbose without a clear starting point.
* **Task**: As an engineer for the OpenStack tiger team, we needed automated builds of the infra.
* **Action**:  Wrote and created a PR for a quickstart guide.
* **Result**: Better documentation for another team. Also, empowered new engineers to quickly get started with a testing environment.

## Invent and Simplify

> Leaders expect and require innovation and invention from their teams and always find ways to simplify. They are externally aware, look for new ideas from everywhere, and are not limited by “not invented here." As we do new things, we accept that we may be misunderstood for long periods of time.

* **Situation**: Terraform setup had organically gain several layers of shims/wrappers to provide functionality.
* **Task**: My role was to help the ops team automate their workflows. While this was not directly my responsibility, it was adding cognitive complexity and tech debt to the provisioning for service team.
* **Action**: Audited the workflow, tracked down all the scripts being used to generate and execute the terraform. 
* **Result**: With minimal changes to the current terraform layout, all technical debt could be removed with newer versions of terraform and terragrunt. 
&nbsp;
* **Situation**: As a managed service provider, each client's needs had vastly different needs resulting in hand crafting infrastructure for each environment.
* **Task**: To provide support to the client.
* **Action**: Wrote cookbooks for config management.
* **Result**: Fast to provision infra. homogeneous base for all clients.

## Are Right, A Lot

> Leaders are right a lot. They have strong judgment and good instincts. They seek diverse perspectives and work to disconfirm their beliefs.

A more senior engineer designed a solution, for secrets propagation, that I was uncomfortable with.
I researched key pair technologies. I sought out feedback on my design from the principle engineer who had a reputation for not being satisfied with most implementations. I addressed all his concerns in a 2nd iteration and gained his support. Then presented the new architecture to the team.

* **Situation**: 
* **Task**: 
* **Action**:  
* **Result**: 

* **Situation**: The team was moving forward with a solution that did not sit well with me from a security perspective. The rational was it is better then what we have and it can be complete in the short expected delivery date.

## Learn and Be Curious

> Leaders are never done learning and always seek to improve themselves. They are curious about new possibilities and act to explore them.

Certified Scrum Product Owner

Recently learned:
* embed systems
* how to build a serverless service
&nbsp;
* **Situation**: The manager wanted individuals to be come Certified Scrum Product Owners.
* **Task**:  Role involved designing and maintaining provisioning services and tools.
* **Action**:  Petitioned to be sent to training.
* **Result**:  Improved conversations around requirements/mvp, and priorities.
&nbsp;
* **Situation**: Sole engineer creating a Policy-As-Code service for compliance enforcement.
* **Task**:  Role was design, deploy, maintain, and continue development on service.
* **Action**:  Learned how to design and deploy a serverless application.
* **Result**:  Deployed a product that was having a meaningful impact w/o infrastructure to maintain and painless deployments; giving more bandwidth to train team and continue development of features.
&nbsp;
* **Situation**: As someone formerly studying electronics I have a desire to bridge my development skill set with low level hardware.
* **Task**:  As a organizer in the Los Angeles tech scene, I regular aid groups with events.
* **Action**:  Joined the SCaLE A/V to help develop an interface to control the audio/video switches from the in-room recording /muxing computer.
* **Result**:  A system controlled from the A/V Noc, reducing the need for volunteers to run out to each room individually. And now able to focus on stream quality. Along with being able to sit back and enjoy the conference a little more.

## Hire and Develop the Best

> Leaders raise the performance bar with every hire and promotion. They recognize exceptional talent, and willingly move them throughout the organization. Leaders develop leaders and take seriously their role in coaching others. We work on behalf of our people to invent mechanisms for development like Career Choice.

Identify candidates to train in Python.

Provided opportunity for customer support staff to expand their role and skill set by teaching them how to do post new products on the website.


* **Situation**: Shortly after being hired, I was moved to a tiger team to aid in the automated build-out of a new private cloud infrastructure. Shortly after working on the tiger team, I was promoted and moved to the main provisioning team.
* **Task**: As a member of the automated provisioning team, we were responsible for low level self-healing of the CDN, and free up our system engineers to address other issues, ie. system tuning. This meant I now spent the majority of my time becoming a better software engineer.
* **Action**: Started bi-weekly trainings around Git, Python, Saltstack. Since I could not pull the entire team, I had to identify a few candidates.
* **Result**:  More engineers that were more efficient by leveraging development best practices. Share of code/scripts. And even a couple were promoted across the next 6 months.
* 
## Insist on the Highest Standards

> Leaders have relentlessly high standards — many people may think these standards are unreasonably high. Leaders are continually raising the bar and drive their teams to deliver high quality products, services, and processes. Leaders ensure that defects do not get sent down the line and that problems are fixed so they stay fixed.

* **Situation**: In a short time, we needed a mechanism to propagate secrets through the infrastructure. A designed was rushed out that had, to me, a glaring security issue.
* **Task**: As a member of the team to implement secret propagation, I was responsible for ensuring that best practices were used.
* **Action**: I researched the problem space and create a new design that would leverage the work that was already inflight w/o causing out delivery date to slip.
* **Result**: A product that I had confidence in and work that I was proud of.

Proper implementation of secret propagation. I was not satisfied with the proposed solution. Across the next few days I researched and designed a solution that was more secure and less technical debt.

## Think Big

> Thinking small is a self-fulfilling prophecy. Leaders create and communicate a bold direction that inspires results. They think differently and look around corners for ways to serve customers.

* **Situation**: A lot of old and/or unused AWS resources. Increasing opx and reducing security. 
* **Task**: As the developer with in operations, I automated processes and created tools for existing workflows.
* **Action**: Created Policy-As-Code service for compliance enforcement.
* **Result**: The security posture of our customer's data was increased. And internal customers overhead costs reduced.

Compliance enforcement

## Bias for Action

> Speed matters in business. Many decisions and actions are reversible and do not need extensive study. We value calculated risk taking.

* **Situation**: Received a complaint from an employee of a client that they were unable to access their documents from the file server. In the time to respond to the issue, another use reported that they could not access files from the file server and their local files were unable to open.
* **Task**: As an engineer of managed service provider my role was to assist clients with their infrastructure needs.
* **Action**: Connected to the file server and saw evidence of a ransomware attack. Immediately powered off the file server and closed the ports on the switch w/o first seeking approval.
* **Result**: While I caused the company to come to a halt, I prevented wide spread dataloss. The company was functional within a few hours. The local backup were still intact, enabling speedy recovery of encrypted data.

Cleaning up unused resources across all accounts.


## Frugality

> Accomplish more with less. Constraints breed resourcefulness, self-sufficiency, and invention. There are no extra points for growing headcount, budget size, or fixed expense.

* **Situation**: Building TDI MVP with no budget or dev environment.
* **Task**: As an engineer of a manage service provider, needed to build reliable infra for clients.
* **Action**: Added a server, that was a decommissioned from a client, to the VMware/vSphere cluster. Gave it, it's own spinning rust to avoid using the production SAN. And create a VLAN for the VMs on this hypervisor node to provide some level of segmentation.
* **Result**: Created a TDI pipeline and dev environment to build a base image for servers w/o having to build another environment or purchase additional hardware.

Converting data entry systems from EOL Windows and MS Office machines to running open source software that was receiving security updates.

## Earn Trust

> Leaders listen attentively, speak candidly, and treat others respectfully. They are vocally self-critical, even when doing so is awkward or embarrassing. Leaders do not believe their or their team’s body odor smells of perfume. They benchmark themselves and their teams against the best.

Putting myself out there by doing demo/presentations for the team when I was new. This encouraged more junior engineers to try. I provided accolades during our weekly retrospectives for the effort made and information shared.

* **Situation**: Several racks of kvm nodes needed the networking configured. This was a manual process to determine VLANs, IP ranges, etc. This needed to be delivered asap, as we were already out of capacity.
* **Task**: A new engineer on the team, I was task to configure the nodes. 
* **Action**: I setup the first node and the copied the config files to the rest of the servers. I accidentally skip a server resulting in two nodes w/ the exact same network configuration for the VMs. I ended up making a network loop and so much congestion, the control plain of one of the CDNs was inaccessible. But I did not know that or how I could have done that yet. The networking team quickly identified which switches had high congestion. When I realized it was my change that caused this, in a public channel I informed them that I believed the problem was a result from a change i did and that it was safe to close the ports on the top of the racks. Then I worked w/ the networking to track down what had happen and isolate the offending nodes. Prior to this incident, I was unaware spanning tree was disabled in our backoffice.
* **Result**: Trust was gained as I did not hesitate to speak up, ensuring the incident was mitigated b4 consumers were impacted. Team members shared w/ me outages they have caused, and if stuff does not sometime break we might not be moving fast enough. That said, its very important to learn and not repeat the same mistake. I also built a better relationship w/ the networking team as I went as sat w/ them to triage the situation. On top that, to remove this manual process increased in priority.

## Dive Deep

> Leaders operate at all levels, stay connected to the details, audit frequently, and are skeptical when metrics and anecdote differ. No task is beneath them.

Working with sysadmins to better understand their needs.

* **Situation**: Terraform setup had organically gain several layers of shims/wrappers to provide functionality.
* **Task**: My role was to help the ops team automate their workflows. While this was not directly my responsibility, it was adding cognitive complexity and tech debt to the provisioning for service team.
* **Action**: Audited the workflow, tracked down all the scripts being used to generate and execute the terraform. 
* **Result**: With minimal changes to the current terraform layout, all technical debt could be removed with newer versions of terraform and terragrunt. And better positioned the config-as-code to be deployed w/ Atlantis.

## Have Backbone; Disagree and Commit

> Leaders are obligated to respectfully challenge decisions when they disagree, even when doing so is uncomfortable or exhausting. Leaders have conviction and are tenacious. They do not compromise for the sake of social cohesion. Once a decision is determined, they commit wholly.

Advocating for a colleague to be promoted and move to automation team. I disagreed with the assessment that the team the engineer was could not afford to lose him. I felt it was unfair to engineer and that the company was risking loosing him all together. The next quarter he was the first promotion to a newly formed engineering team.

Disagreed with the design decision of secret propagation. While is was an improvement, it involved moving private keys and that did not sit well with me. I was the minority opinion so work began on the less than idea solution. Over the next few days I researched and designed an improved solution. I reached outed to a couple engineers for peer review and, in the process, gained their support. Then I presented the solution the team as a whole, illustrating a roadmap that would leverage the work that was in flight and a timeline that did not change our delivery date.

* **Situation**: The team was moving forward with a solution that did not sit well with me from a security perspective. The rational was it is better then what we have and it can be complete in the short expected delivery date.
* 

* **Situation**: 
* **Task**: 
* **Action**:  
* **Result**: 

## Deliver Results

> Leaders focus on the key inputs for their business and deliver them with the right quality and in a timely fashion. Despite setbacks, they rise to the occasion and never settle.

* **Situation**: Creating a pipeline to have consistence images across all environments (i.e. public and private cloud and baremetal) that start from the same base artifact. We were leveraging a tool from the Debian team on Ubuntu. As we developed, we kept discovering changes required to make the tool work for both OSes causing the project to be at risk of not making the delivery date.
* **Task**: Lead the project.
* **Action**: Proposed to focus on AWS and OpenStack. And drop Docker images and baremetal support. AWS and OpenStack is where the most new development and issues were occurring. Docker was still experimental in the org. Bare metal was already building from the internal repos.
* **Result**: We delivered a product on time that addressed the larger pain points atm. This also stopped the technical debt of workarounds teams were making to get their service to function in the new environments. Two ways I was able to verify this, was as we educated teams of the new images when they came for support, they would respond "oh, it works now". And by the PRs coming into the config mgnt repos stopped including conditional setup for the cloud environments.


On-prem and public cloud teams base images did not match the rest rest of the infrastructure causing deployment issues for service teams.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3Mjc1MjE0MTVdfQ==
-->