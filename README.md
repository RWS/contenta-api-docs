# contenta-api-docs

## What is it?

This the main repository for the Contenta Public API documentation.

## Can I contribute?

Anyone is welcome to contribute to the public Contenta API documentation by making a pull request into the master repository.


The documentation is split into the following sections:
- Articles
  - This section hosts a series of usefull article on:
    - how to get started with writing plug-ins for Contenta
    - how to best use the public APIs
    - how to troubleshoot common issues
- API Concepts
  - This section hosts the main guidelines on using the Public API along with the API References

### Getting started with your contribution
The documentation is built using a static documentation generator called [DocFX](https://dotnet.github.io/docfx/). 
The documentation content is saved in *Markdown* files and then built into a website using [DocFX](https://dotnet.github.io/docfx/). The table of content is saved into separate *toc.yml* files.

In order for you to make a contribution directly please follow the next steps:
- Create a local branch from the main repository
- Add your changes by modifying existing *Markdown* files or by adding new *Markdown* files
  - Adding new files will require updating the *toc.yml* files. Use the [guideline](https://dotnet.github.io/docfx/tutorial/intro_toc.html) provided by [DocFX](https://dotnet.github.io/docfx/) to learn more. 
  - You can use tools such as *Notepad++* or *Visual Studio Code* to edit the content
- Create a Pull Request with your changes. 
  - This pull request will be reviewed for correctness by one of our technical writers
- Once your pull request has been approved and committed into the *main* branch, an automatic pipeline will be triggered which will push your changes to the [live documentation site](https://rws.github.io/studio-api-docs/index.html)
- if you wish to test your changes locally you can follow the [DOCFX Installation guideline](https://dotnet.github.io/docfx/tutorial/docfx_getting_started.html) and [build the entire solution locally](https://dotnet.github.io/docfx/tutorial/walkthrough/walkthrough_create_a_docfx_project.html)
- Our documentation automatically fills in the product name and other details so you don't have to make the changes manually if we decide to update the product name. Use the '<var:VariableName>' construct to tell our documentation engine to fill in the info for you. Here are the constructs available at this point:

      var:ProductName - The product name, for example Contenta
      var:ProductNameWithEdition - The official product release name including the edition, for example 'Contenta 2021'
      
