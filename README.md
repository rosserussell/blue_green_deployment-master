<H1>README</H1>
<H1>Repo Name: blue_green_deployment </H1>
<P>Purpose: To demostrate how to provision a blue-green deployment using a Jenkinsfile and terraform on AWS.  
</P>

<H1>This repo will:</H1>
<UL>
<LI> Create a new VPC
<LI> Retrieve an existing DNS Zone
<LI> Create VPC gateway
<LI> Create two CIDRS: one for the blue environment and one for the green environment
<LI> Create a complete new BLUE Environment including:
    - item
    - item
<LI> Create a complete new GREEN Environment including:
</UL>

  
  
<H1>Before running this repo on your own repository:</H1>

<UL>
<LI>Update the Jenkins File to specify your own Nexus Repository URL (1 location)
<LI>Update the jenkinsfile to specify your own GitHub Repo URL and name (1 location)
<LI>Add your Jenkins IP webhook to each repo (1 location)
</UL>
  
<H1>Assumptions:</H1>
<UL>
<LI>Terraform v0.11.11 is install on the Jenkins server
<LI>The Jenkins Server EC2 instance has an instance role with sufficient permission to provision AWS Resources 
</UL>
  
<H1>How to run</H1>
<UL>
<LI> Create a "Pipeline" Job in Jenkins
<LI> Under the "Pipeline" section, select "Pipeline script from SCM", click on "git" and select your copy of this repo
<LI> Create a ssh-key jenkins credential on your Jenkins Server and select it for this job
<LI> Click apply
<LI> From the Jenkins Menu, select the job
<LI> Click on "build now" from your Jenkins left menu
</UL>
