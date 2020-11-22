## Netlify Deployment take-home project

My goal was to deploy a site to Netlify using the [setup guide](https://docs.netlify.com/site-deploys/create-deploys/#deploy-with-git).

Since this project was focused on the deploy process, I chose to use a starter template rather than build my own from scratch. One peril of using starter templates is you are relying on someone else's code. It is important to note that your code must run successfully in your development environment before trying to deploy. I tried several starter templates before I found one that worked for me, eventually cloning [this repo](https://www.gatsbyjs.com/starters/gatsbyjs/gatsby-starter-blog/) from Gatsby’s selection of starter templates to get up and running.

#### Configure Netlify with git repo

Before I started the deployment process, following the Netlify [Create Deploys](https://docs.netlify.com/site-deploys/create-deploys/#deploy-with-git) documentation for continuous deployment with Git, I needed to connect my local repo to GitHub and test the site on my local development server.  

I began by watching the video included in the documentation and then read the guide. I then logged in to my Netlify account dashboard and started by clicking the green button labeled “New site from Git”. The next page gave me options for choosing a git provider, as Github is my provider, I chose that option. Before I could connect to my repo, Netlify needed additional authorization from Github to access all my repos, but following the prompts made it easy. 

#### Deploy site to Netlify

Now that all my repos were connected, I used the handy search bar to find and select my repo for deployment. The next page displayed settings for branch, build command, and publish directory. I was pleasantly surprised that the UI had pre-populated the correct defaults, a very welcome feature. At that point all I had left to do was click the green “Deploy Site button”, the deployment started and ran for about a minute and a half. The deployment was successful and my site was published! I took a look at the deploy summary and the build log, had the deployment failed I could have used this log to troubleshoot any problems.

#### Summary

Overall, my experience was a very positive one. By reading the documentation and watching the video I felt well prepared to go through the process. I appreciated the integration with Github to connect my repos without leaving the page, and having the deploy settings set for me made it worry free. For me, the hardest part of the task was making sure my starter code was error free and ready to deploy.


Here is a link to the published site.
[https://hungry-morse-d2d48e.netlify.app](https://hungry-morse-d2d48e.netlify.app)


##### Step-by-step instructions

Below are screen shots of my deployment journey.

1. Log into your Netlify account, from the dashboard, click the green button labeled “New site from Git”.

![deploy-screenshot-1](/img/deploy-screenshots/1.png)

2. Choose your git provider for continuous deployment.

![deploy-screenshot-2](/img/deploy-screenshots/2.png)

3. Select the repo you want to deploy, If you can’t see your repo you may need to click the link to configure the Netlify app on your git provider.

![deploy-screenshot-3](/img/deploy-screenshots/3.png)

4. Check deploy settings for owner, branch, build command, and publish directory before clicking the green button labeled “Deploy site”.

![deploy-screenshot-4](/img/deploy-screenshots/4.png)

5. The production deployment window will display “Starting Up”.

![deploy-screenshot-5](/img/deploy-screenshots/5.png)

6. Once the deployment is complete the display message will change to “Published” and a link to the site will be available above.

![deploy-screenshot-6](/img/deploy-screenshots/6.png)

7. To access the deploy summary, click the arrow next to the Published message.

![deploy-screenshot-7](/img/deploy-screenshots/7.png)

8. A full deploy log is available below the deploy summary.

![deploy-screenshot-8](/img/deploy-screenshots/8.png)




