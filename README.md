# Bioconductor on Containers

# Instructor(s) name(s) and contact information

Nitesh Turaga* <nitesh.turaga@roswellpark.org> (Github: [@nturaga](https://github.com/nturaga))

# Schedule

NOTE: Since the workshop is broken into pre-lunch and post-lunch session, i've decided to break up the topics into two sessions. I recommend attending both to get a complete idea of the Bioconductor ecosystem on containers and how to use them.

https://bioc2019.bioconductor.org/schedule-developer-day

ROOM: Smilow Seminar Room/MSB large/SB G19

11:00 - 12:00 – Workshops I 
    Track 1: Bioconductor on Containers - Beginners

12:00 - 1:00 - Lunch

1:00 - 2:00 - Workshop II
    Track 1: Bioconductor on Containers - Advanced

# Workshop Description

Bioconductor provides Docker containers which aim to provide isolated
and reproducible environments for analysis. These containers avoid
complex installation issues for the user. This workshop will focus on
how to use Bioconductor docker images, describe the different flavors
of Bioconductor Docker images that are available, how to set up a
reproducible environment on a local machine, and as a final advanced
topic we will cover how to extrapolate these Docker images to be used
on cloud services and also on HPC infrastructure with Singularity.

## Pre-requisites

* Basic knowledge of R syntax / how to install packages the
  Bioconductor way (using `BiocManager()`).

* IMPORTANT: Docker needs to be installed on your local
  machine. Please [install](https://docs.docker.com/install/) Docker
  ahead of time. If you are planning to attend this workshop and are
  having issues installing Docker please email me ahead of time, I
  will help you through it. Please do not attend the workshop without
  installing Docker on your machine. 
  
  To [test installation of Docker](https://docs.docker.com/get-started/),
  please run on your command line, 
  
		$ docker run hello-world
		
		Unable to find image 'hello-world:latest' locally
		latest: Pulling from library/hello-world
		ca4f61b1923c: Pull complete
		Digest: sha256:ca0eeb6fb05351dfc8759c20733c91def84cb8007aa89a5bf606bc8b315b9fc7
		Status: Downloaded newer image for hello-world:latest

		Hello from Docker!
		This message shows that your installation appears to be working correctly.

* Some familiarity with HPC infrastructure (if this is relevant to
  participant).

#### Background reading

* (Required) Install Docker https://docs.docker.com/install/ ahead of
  time. Help will not be provided during the workshop.

* (Optional) Read about Bioconda and `conda` if you are interested.

## Workshop Participation

Participants are expected to launch Docker images on their local
machines, mount volumes, and set ports as needed for RStudio. They
will learn to selectively use a required set of packages for the
particular Docker image. There is going to be a live demonstration of
usage of Docker, and participants are exptected to follow along.

## *R* / *Bioconductor* packages used

* [BiocManager](https://cran.r-project.org/web/packages/BiocManager/index.html)

## Time outline

An example for a 1 hour 45-minute workshop:

| Activity                     | Time |
|------------------------------|------|
| Why Docker                   | 10m  |
| Bioconductor on Docker       | 10m  |
| Flavors of Bioconductor      | 10m  |
| Which flavor to use          | 10m  |
| How to mount volumes         | 10m  |
| Docker on the cloud          | 10m  |
| Mount volumes on the cloud   | 10m  |
| Localize select packages     | 10m  |
| HPC-Singularity containers   | 5m   |
| Launch and run parallel jobs | 10m  |
| Questions                    | 10m+ |

# Workshop goals and objectives

## Learning goals

Participants will understand **how** and **why** and **when** to use
Bioconductor with Docker images. The workshop will differentiate the
**flavors** of Bioconductor containers, and how set them up in a
reproducible fashion. The workshop will describe how to use
Docker images and mount volumes as needed from local machines,
and designing a working environment which does not need any
installation of system dependencies. The workshop will also briefly outline
how to use Docker on cloud services such as Google cloud and AWS,
allowing users to launch an image on a cloud instance, giving
them instant access to Bioconductor facilities. We will discuss
how to set up Singularity containers on high performance
computing platforms, and point out resources to enable parallel
computing with containers which taking away the burden to ask system
administrators to install resources for them.

## Learning objectives

Participants will learn how to use the Bioconductor Docker images.
Using these Docker images, they will practice important topics for
creating reproducible environments for their analysis, such as,
mounting volumes as needed from their local machine, adding additional
packages. They will be able to identify the correct flavor of the
Bioconductor docker image for their needs.
