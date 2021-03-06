# Toolchain for Workshop 'Deploying Java Microservices to OpenShift on IBM Cloud - Lab 4'

This project contains a toolchain that is run on the IBM Cloud to deploy a lab of an OpenShift workshop for Developers.

Here are pointers to the workshop:

* Workshop: [Deploying Java Microservices to OpenShift on IBM Cloud](https://github.com/IBM/openshift-on-ibm-cloud-workshops/tree/master/2-deploying-to-openshift)
* Lab 4 instructions: [Deploying to OpenShift via 'oc' CLI](https://github.com/IBM/openshift-on-ibm-cloud-workshops/blob/master/2-deploying-to-openshift/documentation/4-openshift.md)
* Lab 4 video: [Deploying to OpenShift via 'oc' CLI](https://youtu.be/4MDfalo2Fg0)

**TL;DR**

In order to use this toolchain, you need an [IBM id](https://cloud.ibm.com/registration) and an OpenShift cluster in the IBM Cloud. Check out the [instructions](https://cloud.ibm.com/docs/openshift?topic=openshift-getting-started) how to create it.

If you understand how toolchains work, you can click this button to create a toolchain on the IBM Cloud which deploys the lab to your cluster.

[![Create toolchain](https://cloud.ibm.com/devops/graphics/create_toolchain_button.png)](https://cloud.ibm.com/devops/setup/deploy?repository=https%3A%2F%2Fgithub.com%2Fnheidloff%2Fopenshift-on-ibm-cloud-workshops-toolchain)

### Step 1

After clicking the button above, the following page will be opened. 

If this is your first time you use this functionality, you need to grant the toolchain access to your GitHub account. In this case click the 'Authorize' button:

<kbd><img src="documentation/flow1.png" /></kbd>

Grant IBM-Cloud access:

<kbd><img src="documentation/flow2.png" /></kbd>

After this the GitHub integration will be valid:

<kbd><img src="documentation/flow3.png" /></kbd>

### Step 2

On the Delivery Pipeline tab create a new API key or refer to an existing one:

<kbd><img src="documentation/flow4.png" /></kbd>

When creating a new key, simply click the 'OK' button:

<kbd><img src="documentation/flow5.png" /></kbd>

### Step 3

After the key has been defined, your Kubernetes clusters and OpenShift clusters will be displayed in the combobox. Make sure that you select an OpenShift cluster:

<kbd><img src="documentation/flow6.png" /></kbd>

After this click the 'Create' button in the upper right corner:

### Step 4

The pipeline will automatically be triggered. Click on the Delivery Pipeline icon to see the deployment status:

<kbd><img src="documentation/flow7.png" /></kbd>

After the pipeline has run, open the OpenShift web console to see the deployed microservice:

<kbd><img src="documentation/flow10.png" /></kbd>

You can open the log of the last job to see the URL of the API explorer of the authors service:

<kbd><img src="documentation/flow8.png" /></kbd>

The URL opens the API explorer:

<kbd><img src="documentation/flow9.jpg" /></kbd>