# **Virtual Box Introduction**


To setup your virtual laptop you have 2 options one is laptop (either office or home) and 2nd is Cloud. 

There are many cloud providers like Google and AWS who offer to create virtual machines for free. 

For now, let's discuss how to setup a virtual machine on a home laptop. 

**Why do we create a virtual machine:** 

When you are in devOps learning process you need certain tools to be downloaded like git for version control, build tools like jenkins for running for builds programming languages like java, python or node.js, their dependent libraries or packages, web servers like apache servers, nginx, or DBs like MongoDB, MySQL etc, or containerization tools like Docker, kubernetes and automation tools like ansible,  chef or puppets. As well as cloud management tools, like cloud sdks, cmd line tools and even different Operating systems such as Ubuntu, Centos, fedora.  

You can install all these in your local computer and keep playing with them. But at some time, your laptop will have performance issues de to more storage usage.  

To overcome these issues, you can install them in your VM. This way you can delete your VM if anything goes wrong or take a back-up of this, so it will not affect your laptop compatibility issues.

In all of these tools, you need to install some of them on your local system like: **git** and a few other tools you need to install for your day to day basis for development purposes.

The software that helps you create these virtual machines, these are called **Virtualization** software **Hypervisors**.

There are **2 types of Hypervisors**, they are:
1. 
Type 1 --> These are directly installed directly on bare metals like laptop or server and the VMs are created on that now. Examples for this are: **vmware ESXi and Microsoft Hyper-V**.

These are used in **enterprises and production** where you need to create and manage large number of VMs and these hypervisors have high resource requirments. They also need to be installed and configured directly on the laptop and are expensive.

2. 
Type 2 --> These are the Hypervisors that run on the existing OS.Examples are **Oracle virtual box, vmware workstation**. These will hel you to get started quickly without any need to install any Operating systems or re-imaging the laptop.

Going forward when we say host OS, we are reffering to the main OS on our laptop and when we talk about guest OS we are referring to VMs that are created on the Hypervsiors which are on the OS.

The Virtual boxes you can use are Oracle virtual box or vmware workstation.

**Oracle VM:**
- It is free
- Open Source
- Can be installed anywhere - Windows, Linux, MAC
- Supports backu, and snapshots & Clones
- Run multiple VMs
- Networking

**vmware workstation:**

- Commercial
- Can be installed anywhere - Windows, Linux
- It supports features like snapshots and clones.
- there is a free version of vmware workstation that is known as **vmware player** for **Windows and Linux** and **VMware fusion** for **MAC** but it doesn't have many features that are vmware workstation or Virtualbox supports such as running multiple vms at the same time or taking snapshots or performing advanced networking configuration.