[Back to homepage](index.html)

## Table of contents

* [Milestone 1](#Milestone-1)
* [Milestone 2](#Milestone-2)

## Milestone 1 

See the Project Board here : [M1](https://github.com/orgs/manoa-fixed/projects/3)

We have three members working on this app: Yuuma, Roman, and Corben. For our first Milestone, we will assign our members individual responsibilities. Each member will specialize in a certain app area. Also for this Milestone, we will start creating rough mock-up webpages to help get a sense of the project.

Member Responsibilites:

* Yuuma : Front-End designer. Codes the visual side of the site. Must have the page look visually appealing. Also can work on implementing categories for the various types of submitted reports.
* Roman : Will incorporate the mapping aspect of the site. Also implement the photo uploading.
* Corben : Back-End engineer. Will manage the database information. Implements Email Notification feature.

Within the first week of starting the project, we managed to get a working landing page. We also managed to get something that we deemed visually satisfying.

Going forward, we still need to get it working database-wise. We will also need to work on the other two tabs because, as of now, they have no connection to the overall goal of the site. This is in part to time constraints, as well as a higher difficulty in implementing them. 

*** UPDATE ***

As of now, we have officially deployed our app to Galaxy. See it [here](http://manoafixed.meteorapp.com/#/).

So far, these are our default pages available to all users. These features are available to users who do not sign-in.
Click on the term to get linked to the site :

[Landing Page](http://manoafixed.meteorapp.com/#/)

<img src="galaxy.PNG">

Note that we have added an actual button in addition to the tab. The button is more visually stimulating, and catches a user's eye moreso than the smaller Add tab.

[Add tab](http://manoafixed.meteorapp.com/#/add)

<img src="add.PNG">

We still need to get the image upload working. Need to also incorporate location coordinates.

[About tab](http://manoafixed.meteorapp.com/#/list)

<img src="about.PNG">

Got the beginnings of the About tab working.

Overall, this was a successful first milestone!

## Milestone 2

See the Project Board here : [M2](https://github.com/orgs/manoa-fixed/projects/4)

Condensed To-Do List for Milestone 2:

* Add Report : Location and Image should probably not be of type String. May need to change.
* List Report : Edit feature should only be available to admins. 
* View Map : Possibly the hardest feature of the app. Need to break ground on this sooner rather than later.
* Email Notifications : Send out a notification via email to admin account when new report is added.
* Image Upload : Lets try to implement a "Drop Zone" for image upload.

*** UPDATE ***

Now that we are halfway through Milestone 2, I would like to give an update on the our current progress:
So far, I have had success using [Cloudinary](https://cloudinary.com/) to help with image uploads in Add Report. Essentially Cloudinary allows for cloud-based image storage that can be used for websites and apps. So far, it is not completely working, but I have gotten the Drop-Zone feature implemented. To do this, I brought code over from the RadGrad repo, which also uses a Cloudinary widget. Though their code was a good base to work off of, it was also quite difficult to have it working for my site. Since the RadGrad code was written in TypeScript, I had to completely rewire the code for my site's JavaScript needs. At the end of the ordeal, I was satisfied once the "Upload" button was finally working and I could see uploaded images being posted on my Cloudinary account.

Next, though this was not initially planned, I added a Donate tab to the app. This allows a user to donate to the maintanence department via Paypal, Debit, or Credit to an already made Paypal account. Since I do not know if the maintanence department has an account, I may just change this to donate to our development team. I should mention that I got this code from Paypal's website. I think this was a nice and interesting touch.

Lastly, I want to add a few lessons/tips I have learned during this milestone:
1. Be sure the password in the settings.production.json file matches the password in the online Mongo Database. I was stuck on this for awhile because the Command Prompt does not specify the error during upload. Rather it gives a generic error message that offers no clue to what went wrong during deployment.
2. Turning off your system's Virus Scanner greatly increases the speed during the deployment process. Don't forget to turn it back on afterwards!

Also, I forgot to mention that Yuuma got the Email Notification feature working. Upon adding a report, an email is sent out to a specified address. Great job!

