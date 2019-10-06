<h1>Resize an instance<h1>
  
first to resize, stop the instance 

>in navigation pane selesct instances , and select the instance.
>Choose Actions, select Instance State, and then choose Stop. If Stop is disabled, either the instance is already stopped or its root device is an instance store volume.

![kil](https://github.com/kilzol/Amazon-web-services/blob/master/images/Screenshot%20(63).png)

**warning  When you stop an instance, the data on any instance store volumes is erased. To keep data from instance store volumes, be sure to back it up to persistent storage.**
>In the confirmation dialog box, choose Yes, Stop. It can take a few minutes for the instance to stop.

![kil](https://github.com/kilzol/Amazon-web-services/blob/master/images/Screenshot%20(64).png)

To resize
>With the selected instance, choose Actions > Instance Settings > Change Instance Type

>From the Change Instance Type dialog box, choose which instance you would like to resize to.

*If the desired instance class is not listed, then it isn’t compatible with your existing instance configuration.

![alt](https://github.com/kilzol/Amazon-web-services/blob/master/images/Screenshot%20(65).png)

>Once applied, start the stopped instance - it will now be running on the new instance class you chose.



The instance ID will not change, even though the underlying hardware is changed.
If your instance is running in a VPC and has a public IPv4 address, it will receive a new public IPv4 address but retains its private IPv4 addresses, any Elastic IP addresses, and any IPv6 addresses.
If the instance is in an Auto Scaling group, you must suspend Auto Scaling otherwise the stopped instance will be marked as unhealthy and may be terminated before you can resize the instance.
