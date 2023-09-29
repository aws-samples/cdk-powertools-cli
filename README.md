# IaC Developer Tools CLI for CDK (IDT)

This command line interface tool automates many of the tedious tasks of building, adding to, documenting, and extending AWS CDK applications. It is an opinionated tool that integrates Well-Architected principals of cloud native software design by default.

## What is does

1. Automates templated build of a basic multi-stack CDK application with integrated security, devops, and pre-formatted documentation.
2. Automates templated build of a starter CDK stack
3. Automates templated build of a starter CDK construct
4. Automates templated build of DevOps tooling for CDK deployment on Github or Gitlab

## How to use it

### 1/ Install the repository globally

To install directly from the git source you can also use the command below. Coming soon this will be available via npm.

```sh
npm i -g https://github.com/aws-samples/iac-devtools-cli-for-cdk.git
```

### 2/ Check install

```sh
npm ls -g
```

You should see a version of `iac-devtools-cli-for-cdk` listed in your node packages.

### 3/ Navigate to the directory you want to work from

If you are creating a new app you will need to create a new directory to work from

```sh
mkdir your-directory-name
cd your-directory-name
```

If you are adding a construct or stack you will need to navigate to the directory to work from

```sh
cd path/of/your/directory
```

Run the tool!

```sh

idt

```

You should see some options that look like this:

![IDT setup GIF](./assets/documentation/images/idt-start.gif)

Follow the prompts to:

- Create a whole application
- Create an application stack
- Create an application construct
- Create devops tools

![IDT create project GIF](./assets/documentation/images/idt-create-project.gif)

### 4/ Review what you have created

You will now see a full populated template in your working directory.

![IDT tour GIF](./assets/documentation/images/idt-project-tour.gif)

## 🌅 How to update

Since this is not yet in a public npm registry the easiest update method right now is to remove and then reinstall 😢. We are working on making this a little easier.

## 🗑️ How to remove

```sh
npm uninstall  -g @aws-energy-solutions/iac-devtools-cli-for-cdk
```

## 🗺️ Planned Features

- [x] Build projects from templates
- [x] CDK Typescript template
- [x] CDK Typescript construct template
- [x] CDK Custom Resource Template
- [x] Github and Gitlab DevOps tools templates
- [ ] Run security checks
- [ ] BYO template directory
