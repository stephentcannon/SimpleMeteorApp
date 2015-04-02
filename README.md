# SimpleMeteorApp
This tutorial will walk you through deploying a simple HelloWorld Meteor Application to any server with <a href="https://www.distelli.com" target="_blank">Distelli</a>.

<a href="https://www.distelli.com" target="_blank">Distelli</a> makes it fast and easy for developers to deploy code to any server with the push of a button. Our platform empowers developers and their teams to spend less time building and maintaining complex deployment tools and homegrown scripts so they can focus their valuable time and effort on creating the software that powers their business. Distelli is funded by <a href="http://www.a16z.com" target="_blank">Andreessen Horowitz</a>.

##Prerequisites:##
* <a href="https://www.meteor.com/install" target="_blank">Install Meteor on your local machine</a>.
* <a href="https://www.distelli.com/signup" target="_blank">Sign up for a free Distelli account</a>.
* <a href="https://www.distelli.com/docs/setup" target="_blank">Install the Distelli CLI Tool</a>.
* <a href="https://www.distelli.com/docs/agent-setup" target = "_blank">Install the Distelli agent on your server</a>.

##Deploying Your Meteor Application With Distelli##

1. Enter the following commands to clone this repository onto your local machine:
<pre>git clone https://github.com/Distelli/SimpleMeteorApp.git</pre>
You should see the following message on successful clone:
<img src="https://monosnap.com/file/IVkm2GyrDPOWv6xLFNBA0uLhiTi8sa.png">
Then, use the cd command to enter the directory:
<pre>cd SimpleMeteorApp</pre>

2. To create an application with Distelli, enter the following command into your terminal replacing <username> with your Distelli username:
<pre> $ distelli create <username>/SimpleMeteorApplication
You should see the following message on successful app creation:
<img src="https://monosnap.com/file/cAtiueLSEnuRP3aAEKcV1qJc5U5eCT.png">

3. To create an environment with Distelli, <a href="https://www.distelli.com/login" target="_blank">login to your Distelli account<a>. Once logged in you should see the Meteor application you just created. Select the SimpleMeteorApplication:
<img src="https://monosnap.com/file/62C7YNcTLbM0fKzERMwy38w8wbEHqM.png">
Select the environments tab:
<img src="https://monosnap.com/file/mndKKqpXetldIn46QHvInlWn9fJOmJ.png">
Create a new environment by selecting "New Environment":
<img src="https://monosnap.com/file/lxsCrBn5IBptXR6h40RuTR8VosmHA8.png">
Name the environment "MeteorEnvironment" then select the "Create Environment" button:
<img src="https://monosnap.com/file/q8MCSvI0JRNq9pOvAxxYmw0x0BJUJc.png">

4. Now, let's add a server to the environment. Select the "Servers" button on the top right of the page:
<img src="https://monosnap.com/file/72MP9xzaLwXAc1kH3ZMEXDRg7PnOF9.png">
Now select the "Add/Remove Servers" button on the top right of the page:
<img src="https://monosnap.com/file/mlBY0gOOaCJIZAbctYRafLzvhfiym6.png">
You should see the server you installed the agent on prior to starting this tutorial. Add that server to the environment by selecting the add button:
<img src="https://monosnap.com/file/8p6wYuziTvsievb5eWxKzLDwnD6Npb.png">

5. Open the distelli-manifest.yml file with your favorite text editor. Replace <username> with your Distelli username:
<img src="https://monosnap.com/file/7aVg6lS9nLaHp3n6t6lBdQeQoFrrDe.png">
<i><b>Note:</b> This is not the email you used to sign up for your Distelli account, this is the unique username selected after signup.</i>

7. Now we're ready to deploy our sample application. Enter the following command into your terminal:
<pre>$ distelli deploy -m "First deployment with Distelli" -e MeteorEnvironment</pre>
<img src="https://monosnap.com/file/tQLsBhx2mbOorMn2cUa6p5DPpEoVNR.png">
Enter the email and password associated with your Distelli account:
<img src="https://monosnap.com/file/j5vJJRVf1I6taDIRBdmtWcCereBpK9.png">
Enter "Yes" when prompted if you are ready to start the deployment:
<img src="https://monosnap.com/file/bz4ABxHmClhv9hpkMcTftJ72aw4rfU.png">
You should see the following message on successful deployment:
<img src="https://monosnap.com/file/lFkdyKHNHshRKAJElRc98qPcmRAwI0.png">


Questions? Shoot us an email at <a href="mailto:support@disteli.com" target="_blank">support@distelli.com</a>.
