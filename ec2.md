### Questions

#### What is Placement Groups

1. Cluster Placement Groups:

A cluster placement group is a logical grouping of instances within a single Availability Zone. Placement groups are recommended for applications that benefit from low network latency, high network throughput, or both

We recommend that you launch the number of instances that you need in the placement group in a single launch request and that you use the same instance type for all instances in the placement group. If you try to add more instances to the placement group later, or if you try to launch more than one instance type in the placement group, you increase your chances of getting an insufficient capacity error.

If you receive a capacity error when launching an instance in a placement group that already has running instances, stop and start all of the instances in the placement group, and try the launch again. Restarting the instances may migrate them to hardware that has capacity for all the requested instances.

2. Spread Placement Groups

Spread placement groups are recommended for applications that have a small number of critical instances that should be kept separate from each other. Launching instances in a spread placement group reduces the risk of simultaneous failures that might occur when instances share the same underlying hardware. Spread placement groups provide access to distinct hardware, and are therefore suitable for mixing instance types or launching instances over time.

A spread placement group can span multiple Availability Zones, and you can have a maximum of seven running instances per Availability Zone per group.

----

Read create-deploy-docker-ecs with [elasticbeanstalk](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_docker_ecs.html#create_deploy_docker_ecs_platform)

Application Load Balancer (ALB) cross zone load balancing [reading](https://amazonaws-china.com/blogs/aws/new-host-based-routing-support-for-aws-application-load-balancers/)

Redshift use which blocks size for its columnar storage? 1024kb/1MB 

EC2 launch limit per region/AZ is 20.

EC2 AutoScaling peak load configuration.



