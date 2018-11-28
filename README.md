# Penrose Domain Cookie Cutter Template

:cookie: :cookie: :cookie:

This is a :cookie: cookiecutter :cookie: template for making it easy to 
generate a Documentation and static API for a new Penrose domain. As an example,
here is the [domain-linear-algebra](https://github.com/penrose/domain-linear-algebra) 
repository. Look at it's [github pages](https://penrose.github.io/domain-linear-algebra/) 
to see the documentation and static api.

**under development** expect changes and further testing.

# Usage

```bash
$ pip install cookiecutter
$ cookiecutter https://www.github.com/penrose/cookiecutter-domain
```

## Step 1. Generate Codebase

### Quick Start
You don't need to download or clone anything - you can just install cookiecutter 
(a Python package on pip) and then run this command!

1. Install cookiecutter

```bash
$ pip install cookiecutter
```

You'll notice that all "templates" provided by penrose to make development
easier start with "cookiecutter." So the cookiecutter for a domain 
repository naturally looks like this:

```bash
$ cookiecutter https://www.github.com/penrose/cookiecutter-domain
```

### Development Start
If you want to customize the template before you fill it with your variables, you 
can also optionally first clone the template repository. You likely want to
fork the repository to your Github account, and then do the following

1. Install cookiecutter

```bash
$ pip install cookiecutter
```

2. Clone this repository

```bash
git clone https://www.github.com/penrose/cookiecutter-domain
```

3. Edit the cookiecutter.json file with your parameters. If you want to **add**
new parameters (meaning text or other fields that get rendered into the template)
just add a new key and value to this dictionary:

```json
cd cookiecutter-domain
cat cookiecutter.json
{
    "project_lead": "VanessaSaurus",
    "project_email": "vsochat@stanford.edu",
    "project_name": "Linear Algebra",
    "project_slug": "domain-linear-algebra",
    "project_short_description": "A domain for Penrose",
    "year": "2018",
    "version": "0.0.1",
    "repo_user": "penrose",
    "repo_name": "domain-linear-algebra",
    "twitter_name": "vsoch"

}
```

3. Create the repository from this one.

```bash
cookiecutter --no-input
```


## Step 2. Write Your Domain!

The instructions (and examples) for writing the domain, along with structure
of the repository, are included in its README. Generally you will want to:

 - add development files to `_dev`
 - add production files to `_src`
 - add markdown files to describe style, domain, and substance trios to `_domain`
