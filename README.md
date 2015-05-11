# dkr_test
This Repo. is created for testing puposes
## Repositories
1. [Gijeli Docker Repo.](https://registry.hub.docker.com/u/praqma/gijeli/)
2. [Gijeli GitHub Repo.](https://github.com/Praqma/docker-gijeli.git)(Docker Image Context Files)
3. [Pinside Repo.](https://github.com/Praqma/pinside.git)(Pinside Markdown Pages)

###Project Pinside
As a project Pinside and praqma/gijeli docker container are two independent and different things

* [Pinside](https://github.com/Praqma/pinside.git) is a plain git repository with markdown files based on our knowlegde to be rendered into nice webpages
* [Praqma/gijeli](https://registry.hub.docker.com/u/praqma/gijeli/) is a docker image we have developed to serve jekyll websites(markdown files mentioned above), offers git, ruby and ligquid tool support

###Pinside Contents
You may _Add or Edit_ the contents of Pinside by:

* **Opening [Praqma's pinside github private repository](https://github.com/Praqma/pinside.git)** (Permission Required)
	- browse it, edit or add and file

* **Cloning it**
	- edit the files with favorite editor
	- push content back to **[Praqma's pinside github private repository](https://github.com/Praqma/pinside.git)** (Permission Required)

While adding a new _markdown_ file in any **_ _post_** folder placed inside the folder of your concern, follow the [jekyll naming convention](http://jekyllrb.com/docs/posts/)

```
_**YEAR-MONTH-DAY-title.MARKUP**_

```
###Spining up Pinside
Two approaches can be adopted to render Pinside pages:

- Install _jekyll_ on your local machine and _serve_ the pages
- Install _docker_ and run Praqma/gijeli docker image __Recommended_ 

###[Gijeli Usage]() 
You can render your jekyll website from [\<site-source>]() by using the following command:

```
docker run --rm -v <site-source>:/data -p <port>:4000 praqma/gijeli:<version-number> serve --watch --force_polling -H 0.0.0.0

```

Available is a test script for running gijeli server image.

The [\<site-source>]() is the directory on the Docker host with the source for the site. The site can be view as html on [http://\<host-ip>:\<port>]()

###Support
* Praqma/gijeli docker image is maintained by Praqma, you can request features and support on [support@praqma.net]()

* Our knowledgebase project in Praqma is maintained in a [Trello board](https://trello.com/b/ZRHTTLuh/establish-a-praqma-knowledgebas), discuss and do feature requests there
