---
versionFrom: 7.0.0
versionTo: 8.0.0
---

# Working with a local clone of an Umbraco Cloud site

To work with a local copy of your site you'll need to use Windows and have a local web server installed (like WebMatrix / IIS). If you're not using Windows you can still work with your site's files (Templates, Css, JavaScript, etc...) but you'll need to deploy these to your development site before you can "see" your updates - head over to our chapter on [Working with UaaS Cli](../Working-With-Mac/index-v7.md) for more documentation on this.

## Video tutorial

<iframe width="800" height="450" title="Cloning down your Umbraco Cloud project" src="https://www.youtube.com/embed/e3spd6Nqrf8?rel=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Step-by-step

From the Umbraco Cloud portal, copy your development environments git repository endpoint using the **Clone project** option using your favorite Git client. We like [Fork](https://git-fork.com/),  [SourceTree](https://www.sourcetreeapp.com/), [Git Extensions](https://gitextensions.github.io), or [GitKraken](https://www.gitkraken.com/).

Here are the steps to clone your site (**We'll use Fork in this example.**):

1. Click on the arrow next to the **Development** environment and select **Clone project** to open the Clone project dialog.

    ![Connect my machine](images/connect-my-machine.png)

2. Copy the Clone Url from the portal for your dev environment

    ![clone dialog](images/connect-my-machine-2.png)

3. From Fork select Clone

    ![Fork Clone UI](images/Fork-Clone.png)

4. Set your destination path to where you keep your local work
5. Paste the URL in to the URL box
6. Choose a name for the local project folder (preferably using the project name)
7. Click 'Clone the repo!'

    ![Fork Clone UI](images/Fork-clone-2.png)
8. You’ll be prompted to log in - Use the same credentials as you use for Umbraco Cloud.

![Clone to local machine](images/clone-to-local.gif)

Now you have an exact copy of your Umbraco Cloud environment that you can run locally.

We like to use Visual Studio Code when working locally, but you can use Visual Studio or any other development tool or web server. When you run your local site for the first time, you’ll be prompted to restore your site's content. Wait until this process completes as it also creates the local SqlCE database for your site.

![clone dialog](images/restorecontent.jpg)

That's it! Now you can work with your site locally as you would with any other Umbraco site. You can create content, add media, even create your own custom code. When you're ready to deploy your changes make sure to have a look at the [deployments](../../Deployment/) documentation.

:::note
If you have multiple media items see our recommendations for working with [Media in Umbraco Cloud](../Media/).
:::

:::links
## Related Article

- [Working with Visual Studio](Working-With-Visual-Studio/)
:::
