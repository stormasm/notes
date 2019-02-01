

## Control Plane and Data Plane

[Explanation of Control Plane and Data Plane](https://learningnetwork.cisco.com/thread/33735)

Let's say you and I are in charge of public transportation for a small city.

Before we send bus drivers out, we need to have a plan.

##### Control Plane = Learning what we will do

Our planning stage, which includes learning  which paths the buses will take, is similar to the control plane in the network.   We haven't picked up people yet, nor have we dropped them off, but we do know the paths and stops due to our plan.  The control plane is primarily about the learning of routes.

In a routed network, this planning and learning can be done through static routes, where we train the router about remote networks, and how to get there.   We also can use dynamic routing protocols, like RIP, OSPF and EIGRP to allow the routers to train each other regarding how to reach remote networks.   This is all the control plane.


##### Data Plane = Actualy moving the packets based on what we learned.

Now, after the routers know how to route for remote networks, along comes a customers packet and BAM! this is were the data plane begins.   The data plane is the actual movement of the customers data packets over the transit path.   (We learned the path to use in the control plane stage earlier).

#### References

[Which Service Mesh Should I Use](https://thenewstack.io/which-service-mesh-should-i-use/)

[A Crash Course for Running Istio](https://medium.com/namely-labs/a-crash-course-for-running-istio-1c6125930715)

##### Istio Makefile

```
.PHONY: galley-test2
galley-test2: depend
	go test -count=1 -v ./galley/pkg/source/kube -run Builtin
```
