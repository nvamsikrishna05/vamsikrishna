---
title: How to create virtual environments in python
description: A simple guide for creating virtual environments in python
categories: [python, tutorial]
toc: true
layout: post
---

## Introduction

Python virtual environments enable us to create a new isolated python installation and install packages into this isolated environment without affecting the global python installation and it's packages. 
This gives us the clear benefit of eliminating dependency version conflicts between multiple projects in the system. We can have 1 virtual environment per project and keep all of them isolated in their own python environments.

## Prerequisites

Before going ahead with the tutorial, you need to have the following installed:
    - Python 3.6+

## Creating a Virtual Environment

We can create virtual environment in python in multiple ways. One of the easy way way is by using the inbuilt venv module in python.

```
python -m venv my_virtual_env
```

That's it. It creates a new virtual environment called my_virtual_env

If you check your directory where the command was run, you'll notice a folder created with the virtual environment name.

### Activating the Virtual Environment

Now that we have created a virtual environment, we need to activate it,To activate a virtual environment,Run:

If your using windows

```
my_virtual_env\Scripts\activate
```

For Unix, Run the following:

```
source my_virtual_env/bin/activate
```

Do note, If your in any other directory from where you created the virtual environment, use a full path rather than a relative path

Once virtual environment is activate, In most terminal programs you'll notice the virtual environment name gets prepended to the prompt indicating the activated virtual environment.

Once inside a virtual environment, any python packages you have installed will be local to that particular environment only. 

You can activate virtual environment from any folder just run the command above with the correct path where your environment is created.

### Decactivating the Virtual Environment

To deactivate a virtual environment, Run

```
deactivate
```

That's all. Your now good to use the virtual environment in python.

## Further Reading:

- [venv](https://docs.python.org/3/library/venv.html)



