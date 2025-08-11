# Load_Balancer_And_Auto_Scaling_Group_In_AWS  

# TASK 1. Create Launch Template :
1. Log into te aws management console.

2. Navigate to the EC2 service .

3. in the left navigation pane, click on launch tamplate

![launch-template](./New-pic-21/1.launch-template.png).

4. click the create launch template  button
5. configure the launch template setting , including the AMI , instance type, and user data.
![naming-the-template](./New-pic-21/2.Naming-the-template.png)

![setting-AMI](./New-pic-21/3.Seting-AMI.png).

![setting-instance-type](./New-pic-21/4.Setting-instance-and-key-pair.png).

![Network-and-sg](./New-pic-21/5.Network-and-SG.png).

![set-user-data](./New-pic-21/6.Set-user-data.png).

# TASK 2. SET UP AUTO SCALING GROUP:
1. In the aws managemant console, navigate to the ec2 service.

2. click on auto scaling group

3. click the ctreate auto scaling group button.
![Asg](./New-pic-21/7.Auto-scling-group.png).

4. choose use launch template and select the launch template created .

5. configure the auto scaling group setting , including the group name, desired capacity and innitial instance .
![Name-ASG](./New-pic-21/8.Name-ASG.png)

6. set up additional configuration suh as netwrok setting , subnets, and scaling policies.
![Network-setting](./New-pic-21/9.Network-setting.png).

Now , you have successfully created an Auto  scaling group.
![created-ASG](./New-pic-21/10.created-ASG.png).

# TASK 3. Configure Scaling Policies.
1. In the Auto scaling group configuration, navigate to the scaling policies section.
![create-scaling-policy](./New-pic-21/11.create-saling%20policy.png)

2. Click on create scaling policy and configure policies for scaling in and scaling out based on demand .
![setting-the-policy](./New-pic-21/12.setting-the-policy.png).

# TASK 4. Attach ALB To Auto scaling Group:
1. In the auto scaling group configuration, navigate to the load balancing section.
![load-balancer](./New-pic-21/13.Load-balancing.png)

2. click om Edit and select the ALB to associate with the autro scaling group.


# TESTING AUTO SCALLING
1. Generate traffic to trigger scaling policy
![Testing](./New-pic-21/14.Testing.png).

2. monitor the autor scaling group and verify that the number instances adjusts based on demand .


