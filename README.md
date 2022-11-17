![RezilionLogo](https://user-images.githubusercontent.com/94110576/202431540-dfc99e77-69f4-4360-97db-b6bdc924455a.png)


With Rezilion orb, applications can be built securely by validating vulnerabilities early in the development process. 

developers can focus on exploitable vulnerabilities and reduce their backlog and patching by 85%. 

With Rezilion, you’ll gain a deep understanding of your environment, uncover and validate vulnerabilities in your applications and container images, 
explore dependencies and licenses, and export the output in auditing formats. 

To use this action, you need a Rezilion license.

## Installation guide
1. Install the Rezilion Extension from the following link
2. Add a Rezilion environment variable:
"REZILION_LICENSE_KEY"
3. Edit your pipeline yml:

      a. Add Rezilion license key variable per required Job
      ```
      name: test
    on: [push]
    jobs:
      test_sanity:
        runs-on: ubuntu-latest
        container:
          image: nginx:latest
    ```

     b. Add Rezilion as a step for each command in your pipeline

     <img width="405" alt="image" src="https://user-images.githubusercontent.com/94110576/202431010-e1601ede-4c94-4b2d-afb3-3b04f253ce4e.png">

4. Add Rezilion as a Job

Make sure to add inside the "needs" field all the Jobs Rezilion Validate is used in

<img width="368" alt="image (1)" src="https://user-images.githubusercontent.com/94110576/202431283-20d2d9b8-2b40-4674-8564-365565cb6805.png">

For full user guide, please follow this link:
