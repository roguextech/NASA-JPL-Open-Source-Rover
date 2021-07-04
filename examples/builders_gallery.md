# Builders' gallery

OSRs in the wild and under construction! Please [add your rover](#Instructions-for-adding-your-build) and add updates and pictures here as it evolves.

## Robert the Rover ([Achille](https://github.com/Achllle))

| <image src="images/robert/robert1.png" height="150"> <image src="images/robert/robert2.jpg" height="150"> |
|:-:|

<details>
  <summary>Expand to learn more about this build!</summary>
  
  ### background
  * I started construction in December 2019. Robert took his first steps about 3 months later.
  * I use the rover for fun, 
  * I help maintain the two repositories. I'm a robotics engineer by training and happy to help with anyone stuck or with ideas. The best way to reach me is via Slack.

  ### modifications

  * **bigger battery**: Robert runs off of [this 9Ah LiPo battery](https://www.amazon.com/gp/product/B07YP73LMX/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
  * **RC**: For outdoor roving, I use a long-range [transmitter](https://www.amazon.com/gp/product/B08CKWZWPR/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1) and [receiver](https://www.amazon.com/gp/product/B07ZK1R32H/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&psc=1) from Spektrum.
  * **sensor stack**: I mounted a lidar on top of my rover to allow for 2D mapping, localization, and navigation. I also have mounted (variations of) two monocular cameras, an IMU, and depth cameras to it. Details in [my blog post](https://www.freedomrobotics.ai/blog/how-to-pick-navigation-sensors-for-autonomous-mobile-robot).
  * **toy trailer**: I bought this [toy trailer](https://www.amazon.com/gp/product/B0002HZQGO/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) so that Robert can carry a payload. I attached it to Robert using a repurposed wrench and a collar clamp. It's not very robust but [it does the trick](https://youtu.be/caqx-S-_gv8)!
  * **handle**: I used a strong piece of rope and a small piece of PCV tubing (handle) to lift the rover off the ground so I could carry it up and down stairs. 
  
  ### blogs
  1. [Deploying on Mars: NASA-JPL Open Source Rover](https://www.freedomrobotics.ai/blog/building-the-nasa-jpl-open-source-rover)
  2. [Deploying on Mars: How to Pick Sensors to Enable Navigation for Your Autonomous Mobile Robot (AMR)
](https://www.freedomrobotics.ai/blog/how-to-pick-navigation-sensors-for-autonomous-mobile-robot)
  3. [Deploying on Mars: Rock solid Odometry for Wheeled Robots
](https://www.freedomrobotics.ai/blog/tuning-odometry-for-wheeled-robots)
  4. [Deploying on Mars: Rock solid Odometry for Wheeled Robots](https://www.freedomrobotics.ai/blog/deploying-on-mars-mapping-localization)

</details>

## Your rover's name ([your name](github.com/yourgithubhandle))

| <image src="../images/rover-climbing.jpg" height="150"> <image src="../images/rover-silver.png" height="150"> |
|:-:|

<details>
  <summary>Expand to learn more about this build!</summary>
  
  Add whatever information about your build you'd like to share here!
</details>

## Instructions for adding your build

1. We'll be needing a little bit of git skills here. Although not strictly necessary, it helps to take a look at some tutorials on contributing using git & GitHub. Here are the basic steps.
   1. install git on your computer. On Linux, that means `sudo apt-get install git`
   2. Fork this repository by clicking the `Fork` button in the top right corner of the GitHub page.
   3. 'Clone' your fork to your computer by clicking the green `Code` button and copying the link. Type in `git clone ` into your terminal and paste the link you just copied.
   4. Create a new branch and switch to it. `git checkout -b ourrovername_gallery`
   5. You're ready to start making changes! You can use any text editor of your liking, like [VS code](https://code.visualstudio.com/).
2. copy over someone else's section and adjust it to include your build's information. Add your entry to the bottom, just above this section. To keep this compact, add any text and details to the collapsible section (within the `<details> </details>` tags).
3. Create a new folder within [the images folder](./images) and add your rover's pictures to it. 
4. Change the image links to point to your images. The format for that is `image src="images/your_folder_name/your_picture.jpg"`.
5. Commit your changes with git.
   1. in the terminal, navigate to this folder. `git status` should show that there are changes and new files. 
   2. use `git add folder_name/file_name` for each change you want to include to stage those files.
   3. Commit these changes: `git commit -m "Adding my rover to the OSR gallery!"`
   4. Upload them using `git push origin ourrovername_gallery`, replacing `ourrovername_gallery` with the branch name you created earlier.
6. Create a Pull Request (PR) to suggest merging your code into the main branch.
   1. Navigate to the repository's [pull request page](https://github.com/nasa-jpl/open-source-rover/pulls) on GitHub. Click 'New pull request'. 
   2. click 'compare across forks'.
   3. Select your fork from the head repository dropdown and pick your branch.
   4. click 'create pull request'. GitHub will take you to a page where you can create a title of your suggested changes and a description.
7. Wait for a maintainer to review your changes. They might ask you to make changes if something doesn't look right. Once the PR has been greenlighted, your changes will be added to the main branch!