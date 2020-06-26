<div style="text-align: justify">

# ADDING DYNAMIC-GET TO A SITE VIEW

### Checking The Target Dataset

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Now that we have the dynamicGet in place, let's add it to a site view and look at the initial implementation. Go to site view and click on new. Since we already have what you created, we will just open preacher.

### Populate Fields From Get's

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=32" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

On the right-hand, there are three fields you can populate with your dynamicget methods. The first is where you'd add all the custom dynamicgets. There you can add multiple custom dynamicgets. The second is where you add your main dynamicget as we explained in the dynamicget tutorial. You can add one main get method per site view since it will be built in the model, either as a getitem or getitems. [00:00:57](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m57s) It depends whether the main get it is a list or an individual item. Whatever the case, you may include as many custom dynamicgets as you like. You have this data available in your view. (See video.) These two first fields are used to load the dynamicget to the view.

### Dynamic Values

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=96" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The third is used to display. You might want to implement the code of a specific dynamicget option. This one displays main gets; this one customer gets; this both the custom and the main kind of gets. [00:02:04](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m04s) If you select one of these main gets you will see that it shows a list printout of the possible ways you might use the result set. [00:02:32](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h02m32s) (You can copy
each of these by clicking on it; right click and copy or ctrl C and command C to copy the content.) Perhaps you only want to use part of it and not include the echo statement: click from the area where you want to copy and before letting go click on control C or command C. [00:03:05](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m05s) In a mac once you let it go it will select the whole block; if you copy it then, you will copy everything.

### Inserting Values Into View

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=216" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

We use Dynamic Values code in the default view to display the data in a PHP way. You can get the customerget here. The value is going to be in this preacher. (Make sure you have a preacher.) This block deals with displaying the data related to the information. This one here checks whether the main items are on the page. (See video.) [00:04:08](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m08s) The main items are sermons, preacher.id, getlist, etc. If you go down to the sermon preacher, you'd get list; the values are in items. It's an array. You can loop through it and target the object values. That's what's being done here. First, check whether the values are on the page. [00:04:38](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m38s) If we see that it is there, we make use of templates to display the various layouts. [00:05:01](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m01s)

### Making Use of Data Being Passed Through to the View

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=319" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This data structure is the data structure you can expect from each one of these Custom Gets. (See video.) If you were to take number sermons as the method you want to see, it shows the way that it might be packed into the data set. [00:05:36](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m36s) It'll be found in this 'numbersermons'. It could change depending on the custom implementation in your components custom coding areas. You might move this data from that position to something else. The reality is that Dynamic Values gives you a chance to see how it would have looked without leaving the normal path.

### Var Dump

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=373" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This is proposing the dataset structure: Ideally, you had this value here, and do this in the code. (See video.) Do a var_dump, exit, do a build, and look at the view to see the structure. [00:06:45](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m45s) If you are finding that this structure isn't working as we expected, this might help map the array and see where which value is found. The same goes for any of the others. Grab that area that you want to peek into, place it in var_dump, do a build, and look at the page in the front of your site. You can see the structure of the object here, whether it's an array, an array with objects, or whatever is placed inside this value set through the dynamic get method. (See video.) [00:07:20](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m20s)

### Gets In The Code eg: Preacher.php

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=453" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Let's look at how Custom Gets methods are becoming available in your view by going to the code and looking at some of the implementations that we've done. We've gone to the front of the site. (See video.) [00:07:55](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h07m55s) We open and use the preacher model. As you scroll down you see that a getListquery. This getlistquery gets sermon as the 'a' table, series as the 'c' table, preacher is the 'd' table, and categories as the 'b' table. [00:08:18](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m18s) Now it looks for value in id, sets it equal to preacher, ensures that the person has access level to the item that's published, and returns it. [00:08:41](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m41s) That is the getListquery in the model. If we go back to our interface, we have sermon (preacher.id)(getlist) as the main.

### Looking At The Dynamic Get

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=546" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

I've opened that dynamic get here. Sermon is set as 'a,' the main table. If you open Join View Table - Add, series is set as 'c' looking for selection values. Preacher is set as 'd', only selection values. Statistics 'e' is a list. It is multiple. [00:09:36](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h09m36s) These (preacher, series) single ones are part of the list query whereas the multiple of it would have its own method. In the Join DB table add the category as single and 'b' those values. [00:10:01](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m01s) Going back to the code, this is the getListquery in the getitem. After we received the items we look through them in getSermonstatistics and a generated string to ensure no conflicting with other methods on the page. Place the values in 'id sermonsstatisticsE'. [00:10:30](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m30s) This is where the values are placed. (See video.) We have a custom method here. Like we had shown in the dynamic get you can add custom methods and return the items to the page.

### Preacher view.html.php Generated Code

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=655" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

In the page, you have the file, view.html.php. If you open it there is a get items method being used to place the items in items. At the moment we are in the view which means that you can access this set of values inside of that class field. [00:11:26](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m26s) If we go back to our Component Builder, and select that method the items would be corresponding to our code. The id. and the asset_id, etc, are in there.

### Checking The Target Datasets

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=708" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you scroll down there is a 'idsermonstatisticsE' which means that in the array there is a key-value which has another set of array values in it. [00:12:03](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m03s) You can target these data sets by corresponding pointing values. That's just the main get. [00:12:28](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m28s) If we look at the other custom get that has been added, we'll see preacher, a custom method that has been added. It also has a set of values and database structure. (Remember we set it to be linked to the preachers id.) I can check for the id, then set it to id, and return to result. [00:12:53](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m53s) The same goes for the number of downloads. It's also a custom method that set to this view because of the custom get that was added. As we go back to our view.html.php file, those values are respectively being added to preacher number downloads and number sermons. [00:13:21](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m21s) You can use these values in the view by targeting with this number sermons.

### Site Preacher Tmpl Folder

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vEJZe6XqHJE?start=813" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The view itself is under the views preacher inside of the template folder. This main view, or default view, is where the code is on the page. [00:13:50](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m50s) These others are the templates extending the site view. They are extended through layouts available in the layouts folder. [00:14:24](https://www.youtube.com/watch?v=vEJZe6XqHJE&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m24s)

</div>
