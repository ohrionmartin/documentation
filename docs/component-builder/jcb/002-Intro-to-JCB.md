
# Introduction to Joomla Component Builder

Welcome. My name is Llewellyn van der Merwe and I am the developer of the Component Builder for Joomla. I will be giving you instructions on how to use it.

### Component Builder was Built for Developers Who Know PHP

[00:00:18](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m18s)

Component Builder was built for those who know PHP. If you are not familiar with PHP, there are some places to get help like [Lynda.com](https://www.lynda.com/) and Udemy. You could go to their websites, search for PHP, and you would find courses that would help you on your way. To get acquainted with CSS JavaScript HTML, you need to visit these websites. It was not developed for those who have no developing skills. I actually developed it for myself as a developer of components, so that I could easily and quickly get most of the code done, while I could focus on the actual custom code which goes beyond the norm. This is what it is really made to do.

### API Understanding of Joomla is Needed

[00:01:29](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m29s)

If you don't have much knowledge of the Joomla API, it's not that difficult to get an understanding as long as you are able to read PHP. To learn more, open a Joomla website, go to libraries, start reading the classes. You can even go to Joomla's own components. Go to a Joomla install, then to components and to content manager. Look at the folder structures, open them, and you will see the controllers, the models, and the views. Open a view, open the script itself and read through it. If you are using NetBeans, you can hold onto a function like this one (getLayout) and press Ctrl+Shift. It will show you where in your Joomla website that function is declared. [00:02:34](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m34s) You can open that file and open source in editor. You can learn how codes interconnect to each other by just looking at Joomla's own components. [00:02:58](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m58s) (See video.)

### Ways of Implementation

[00:03:55](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m55s)

My aim is not to reinvent things but to stick to the conventions as far as possible. As I become aware of better ways of implementation I would like to add that again. So if you know a better way of doing it, please communicate with me. I would gladly update, include, and change whatever is needed.

### You Must Be Willing to Get Your Hands Dirty

[00:04:17](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m17s)

It is important to debug something if you had built something that did not work. Possibly you need to run a local sandbox environment. Ubuntu is my local sandbox on which I have PHP, Joomla, and MySQL installed. [00:04:38](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m38s) If I have to open a browser, [00:05:04](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m04s) I have a few sites here. This is just my own little script that I've dumped into my own server. [00:05:27](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m27s) Now I go to Builder.VDM. [00:05:43](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m43s) It is loading some of the test displays that I'm working on. If I add administrator to that, it will open the back end, and I can log in. So I'm running in a sandbox environment. The advantage of it is that if you don't have any internet involvement, you can work offline as well as add things like XD bug and other scripts which will help you debug your application. [00:06:07](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m07s) We are doing that in an off-site environment. It is time consuming, difficult, and expensive. [00:06:26](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m26s) It's much easier doing it offline; again, if you don't know how to do that, please visit Lynda.com and look at a course called "Up and Running with Linux for PHP Developers with Jon Peck." [00:06:59](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m59s) It is an excellent course to get your own local developing environment setup. I've watched it long ago [00:07:24](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m24s) and it's been very helpful to get my initial sandbox setup. With time you'd get better and find better ways, but this is a good place to start. 

### The Best Functional Place for Component Builder

[00:07:51](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m51s)

Component Builder's best place of being functional is offline. If you going to do it online, please realize that there might be security risks, especially if you have compiled an application. It places it into your temporary folder which can be accessed from anywhere. Anyone can access your temporary folder on the server of your website. [00:08:14](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m14s) You can delete the application there immediately with a button which I will show you later. In spite of that, I still feel unsafe. The purpose of the application was live in a developing environment where you have Joomla installed and where you can test it intensely. I would suggest you do it that way none the less.

### Help Me to Ensure the Future of the Component

[00:08:51](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m51s)

Since it's free, please help me to ensure the future of this component by not sharing the training videos online or with anyone else. This is the only way that I can sustain this development. If you have an organization or if you're a company and others are viewing it, I can't stop you, but I would encourage you to consider making a contribution when you are starting to reap the benefits of the time that this application saves you so that this application can be further developed for the rest of the community and also for yourself. [00:09:28](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m28s)

### Be Involved On Github

[00:09:50](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m50s)

We would also like to involve you on Github. You can go to github.com/vdm-io/joomla-component-builder. If you have any issues, requests, or anything else, please come here. Go to issues and open a new issue. [00:10:12](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m12s) I want to be sure you can do that if you've got an account with GitHub. Our discussions would be public so that others can see it and so that we can come back to it for reference.

### Feature Requests

[00:10:34](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m34s)

If you want to make a feature request, you can start that feature request here in the issues. If it exists, I'll point it out to you, and if training is needed, we will add it to this training video set. But if there is a feature request that has started here and you can't wait (because we will create milestones and we'll add feature requests to milestones) and you want to ensure that a feature request ends up being done before anyone else's, then you need to communicate with me at this email, llewellyn@vdm.io, and I can send you a link to make a donation, or I'll give you an invoice if needed; so we can ensure that that feature request be done before others. [00:11:09](https://www.youtube.com/watch?v=9evJkBTnKxE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m09s)

If you have questions please let me know. Not questions regarding the component itself, but these points I've mentioned. I'll be grateful.
