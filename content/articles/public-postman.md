---
title: "Public Postman"
date: 2023-05-02T03:35:58-04:00
# weight: 1
# aliases: ["/first"]
tags: ["Postman", "APIs", "documentation", "developer experience"]
author: "Jason Gannon"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: true
hidemeta: false
comments: false
description: "Desc Text."
canonicalURL: "https://jasongannon.me/content/articles/public-postman.md"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
    image: "/images/postman-logo.svg" # image path/url
    alt: "Postman" # alt text
    caption: "Postman — an API Platform to design, build, and test APIs" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: false # only hide on current single page
editPost:
    URL: "https://github.com/jasongannon/personal-site/content/articles/public-postman.md"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link

---
## Introduction

This guide provides instructions for creating a public workspace in Postman, importing OAS files into collections, and making those collections publicly available.

Also, this guide covers how to provide a link in your API documentation so users can to import your collection (or fork it) into their own workspace and test your APIs.

## Setting up a Public Workspace in Postman

### Create an account and sign in to Postman

1. If you haven’t already, [sign up for a free Postman account](https://www.postman.com/postman-account/).
2. Sign in to your account.

### Create a new workspace

In this example, we'll create a public workspace.

{{< callout info >}}

#### You can start with a team space or a public space

You can either create a Team workspace and change the visibility to Public, or you may create a Public Workspace, preset to Public visibility. 
{{< /callout >}}



To create a new Public workspace:

1. Select the **Workspaces**.
2. Select **Create New**.
3. Give your workspace a name and an optional description.
4. Select **Public**.
5. Select **Create Workspace**.


{{< figure src="/images/create-public-workspace.gif" title="Add a public workspace" >}}

## Importing OAS Files into Collections in Postman

Now that we have a public workspace, we need to import a collection or an OAS file to create a collection in the public workspace. 

From here, we'll look at importing an OAS file into your public workspace to build the public collections.

### Import OAS files into Postman

1. In your public Postman workspace, select **Import**, located in the top-left corner of the screen.
2. In the Import dialog, click Choose Files,  select your OAS file, and click Open.
3. To make sure Post will add collections based on the OAS file, click Show Import Settings and make sure Copy collections to workspace is selected.
4. Click Import to upload the files into Postman. You will see your collection in the Collections window.


![Build collections from your OAS file]()

## Integrating Postman Collections with Your Documentation

### Create hyperlink to share collection

1. Click on the collection you want to share, and click Share Collection. 
2. In the pop-up box, click the Via Run in Postman tab. The window allows you to select either an HTML or Markdown snippet that you can embed in your website.

![Copy HTML or Markdown snippet]()

### Edit the API documentation

1. Locate the appropriate section or page in your API documentation where you want to provide the link to your Postman collection.
2. Paste in the HTML or Markdown snippet into your documentation.


![Add Postman button to your Documentation]()

After clicking the button, users have the option to view, import, or fork the collection.

For more information on adding Postman buttons to your website, see [Creating Run in Postman buttons](https://learning.postman.com/docs/publishing-your-api/run-in-postman/creating-run-button/#creating-a-run-in-postman-button).

## Conclusion

You have now successfully set up a public workspace in Postman, imported your OAS files into collections, and made those collections publicly available. 

Additionally, you have integrated the Postman collection link into your API documentation, allowing users to view, import or fork  your collection and test your APIs.

Remember to update the Postman collections whenever there are changes in your APIs and to keep your API documentation. This will ensure that your users always have access to the most current version of your API.
