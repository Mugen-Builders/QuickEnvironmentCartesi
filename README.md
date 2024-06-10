# Quick Environment Setup for Cartesi

This repository provides a quick guide to set up a Cartesi environment using Gitpod and Oracle VirtualBox. Follow the instructions below to get started.

## Gitpod Setup

Gitpod is a cloud-based development environment that allows you to start coding instantly. To set up a Cartesi environment on Gitpod, follow these steps:

1.  Create a new workspace on gitpod.io. You want to put some repository link there, so you can either create on or use an existing one.

![image](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/78a164d9-1ee0-4f7d-807f-751765f5c7d4)

    
3. You can either choose between Desktop or browser versions of VSCode.

![image](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/ca7b63a9-5faa-4ed7-8c7c-85cd47c3e330)

    
4. Click next and deal with anything need for it to start. It is straightforward if it ask for some information in the first time usages. Then, with the vscode set up, open a terminal window and paste this:

```bash
docker buildx create --name mybuilder --use --bootstrap --platform linux/amd64,linux/amd64/v2,linux/amd64/v3,linux/386,linux/riscv64
```

The result will be like below:

![image](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/0b3b1bf3-8f64-428f-8c6b-c6a51c1b987c)

Then, you can install the cartesi cli with :

```bash
npm install -g @cartesi/cli
```

Now you will be able to run all the cartesi cli command. Cartesi doctor won't work but everything else will work.  Your environment is ready!
    

## Oracle VirtualBox Setup

Oracle VirtualBox is a free and open-source hosted hypervisor for x86 virtualization. Follow the steps below to set up the Cartesi environment using VirtualBox:

1.  Download and install Oracle VirtualBox from the official website: [Oracle VirtualBox](https://www.virtualbox.org/).
    
2.  Download the Cartesi VM template file from the link below: [Template-Cartesi.ova](https://drive.google.com/file/d/1vqJaAVcHQbvhthBeo1cSVRMYvbgggh7B/view?usp=sharing)
    
3.  Open Oracle VirtualBox and go to the `Tools` menu, then select the `Import` option.

![1](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/cecdc323-f993-4e3c-93a8-c741e00fe094)
    
5.  Select the `Template-Cartesi.ova` file you downloaded.
    
![2](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/14a76be5-1495-48ad-9ae0-6515408e21b1)


    
6.  Click `Next`.
    
![3](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/d7c51ab8-357f-44cf-ba61-7921abb5053f)

    
7.  The VM will show up in the side list as shown below:
    
![5](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/f0b257bf-36df-4f71-8274-9177942b4fcc)

    
8.  Select the VM and click `Start`.
    
Your Cartesi environment is now ready to use.

![6](https://github.com/Mugen-Builders/QuickEnvironmentCartesi/assets/4421825/bc02d95a-7b66-4c6a-9ee2-ba2f125e16a9)


