# static-site-docker

`Learning Resources for DevOps, SRE, Cloud & Engineering Management`

[![BINPIPE](https://img.shields.io/badge/BINPIPE-YouTube-red)](https://www.youtube.com/channel/UCPTgt4Wo0MAnuzNEEZlk90A)
[![Learn DevOps!](https://img.shields.io/badge/BINPIPE-Learn--DevOps-orange)](https://github.com/BINPIPE/resources/blob/master/devops-lesson-plans.md)
[![BINPIPE](https://img.shields.io/badge/Live--Classroom-blue)](https://forms.gle/tDJxDyj2nJyfsgsk7)
---

**A static website supposed to run as a docker container! (Manual Steps)**

```
git clone https://github.com/BINPIPE/static-site-docker.git
cd static-site-docker
chmod +x wrapper.sh
```

```script
docker build --tag binpipe/static-site-docker:1.0 .
docker run -p 8888:80 binpipe/static-site-docker:1.0
```

Open browser at `http://IP-Address-of-Docker-Server:8888/` to view the website.


**A static website supposed to run as a docker container! (Run Via Jenkins Freestyle Job)**

Follow the tutorial video to get the configuration done. Essentially, the following steps are to be followed:

1. Define the github repo url/credentials in the Jenkins Freestyle Job.
2. In the build phase select the `shell script` option and run the `jenkins-cicd.sh` script as below.
3.  ```
    chmod +x jenkins-cicd.sh
    bash jenkins-cicd.sh
    ```
4. Save the job and execute the build. Follow the execution via console logs.

<pre>
<a href="https://www.binpipe.org">BINPIPE</a> aims to simplify learning for those who are looking to make a foothold in the industry.
Write to me at <b>nixgurus@gmail.com</b> if you are looking for tailor-made training sessions.
For self-study resources look around in this repository, <a href="https://www.binpipe.org/">the Binpipe Blog</a> and <a href="https://www.youtube.com/channel/UCPTgt4Wo0MAnuzNEEZlk90A">Youtube Channel</a>.
</pre>

___
:ledger: Maintainer: **[Prasanjit Singh](https://www.linkedin.com/in/prasanjit-singh)** | **www.binpipe.org**
___

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
