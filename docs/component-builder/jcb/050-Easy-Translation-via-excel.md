<div style="text-align: justify">

# EASY TRANSLATION VIA EXCEL


### New Implementation Added To JCB To Do Translation Via Excel Spreadsheet

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

A quick overview of the new implementation that we have added to JCB that allows you to do translation via an excel spreadsheet. [00:00:19](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m19s)  It is to make it easier to build your component, extract your language strings and to give it to someone else and have them do the translation to the language you like and have them give the spreadsheet back to you and import it into JCB without the necessity of struggling with INI files or any of that. [00:00:47](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h00m47s)

### Need To Know - JCB Doesn't Work With Placeholders - Works Directly With English String

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=51" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

JCB does not really work with placeholders when it comes to these translation strings. It works directly with the English string because the placeholders in the INI file are, for example, this word 'BACK'( `COM-EXPERTDATABASE-BACK`) [00:01:13](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m13s)  This English word(`back`) might end up being used in multiple views, the same English word, but with a different placeholder. [00:01:37](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h01m37s) What we did instead was to ensure that you always translate this specific English string only once, we will only add the string and wherever it reoccurs, will replace the string itself.

### 1. Need To Translate Create New Once

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=126" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

When you think about Create New, Create New is used in many places over in relation to these placeholders. But you only need to translate Create New once. We will add it. The compiler will add it correctly in every other place where it belongs.  That is the first thing you need to keep in mind.

### 2. Translate Strings: Back, Cancel or Close Once - It is Used In Many Components

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=156" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The second thing which is almost as important is that you often have strings that are across multiple components. The string '`back`' for example again or '`cancel`' or '`close`'. It is not only used in one component but in many components but we want to still translate `close` once. [00:03:00](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m00s) Then in every other component where it is used, it will automatically be used. If you have a fresh installation of JCB, and you scroll down and open Language Translations, there are no values and the same when Languages are opened, there are also no values.

### JCB Populate Dynamically The Language Translation, English Strings - Where Does It Get Them?

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=206" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you want JCB to populate the translation. I will get the English strings from the Fields and from the Site views, and from any other place, either the Admin View or any other place where you use Translation strings. [00:03:38](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h03m38s) Then it dynamically populates the Language Translation. It is never necessary to click 'New' to create any.

### The Way To Populate The Language Translation

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=239" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to the compiler and select the component that you would like to compile. Click compile and you need to do that only once and clear that out again. Return to the Language Translations, there are almost 249 strings, and it has not been translated.  Like I said 'close' will only show up once. [00:04:37](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h04m37s) It is so with every other string. If Demo is opened, it can be seen that the English string cannot be edited. There had been a request that people would like to edit the string. It does not really make sense because if the string is being used in a field, how would we be able to know that their relationship needs to change? [00:05:06](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h05m06s) For example if you update a string, JCB needs to know in that field it needs to update the label. There is no way for us to determine that. If the string is changed and it will not be useful because JCB on compilation will detect that this string does not exist, and it will create it again.

### The Way To Change A String - Where it was Created - Fields, Site View, Admin View

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=334" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The way that you would change a string which is found, is you need to go and change it in either the Fields where it was created or in Site View or in Admin View. In this case, we know that this word Demo is the component's name.

* Example Change Demo String

To change that Demo string, for example, I am going to change Demo to Demoo. Save and close. [00:06:14](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m14s)  Compile it again and clear it out and then go back to our Language Translation. You will see the Demo is gone because Demo is no longer being used anywhere, in no other component either so the system will automatically remove it. If you go to the end of the string, you will see the new ones have been added. That is how to [00:06:48](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h06m48s) change an English string, by going back to where you had set it, and then from there have it changed. I am going to change it back, compile it again, clear it out again and go back to Language Translations. You will see that it removed the other one and it added the correct one back.

### Allow Language To Be Set Dynamically - Create Or Use As You Like

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=443" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If only this one Demo string should be translated.  You will see that there is no Language available. We decided to allow the Languages to be set dynamically meaning that you would manually create them and use them as you like. There is an area called Languages. Click 'New', then you will give the Language Name and its Tag. The Language Tag(en-GB) is given as an example but if you do not know how this should look, there are ways to find out.

### Joomla Translation Packs

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=477" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

One of the easiest ways is to go to Joomla's Translation area. If you go to https://community.joomla.org/translations.html. Select the latest one(Joomla 3.x Translation Packs).  There is quite a number of languages. Clicking on any of these will take you down to that language. [00:08:24](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m24s) This is (af-ZA)  the little tag that you would be looking for. If you want to do for example Dutch, then this (nl-NL) is the Tag that you would use. You would use the Dutch as the Name, and then (nl-NL) as the Tag.  For example, I am going to set up 'Afrikaans', it is my native language. [00:08:54](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h08m54s)  'Afrikaans' would be the language we want to create. Then (af-ZA) is the Tag. You can create any of the languages that you would like to use. At some point, a few major languages can be added here and shipped like that, but you could just create a language. A translation can not be created for that language unless this had been done.

### Focus On Translation String Area

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=571" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

For example, take a string that would look different in Afrikaans. Let's take 'Author'. If there are more components that the word Author is used in, it will all be linked in here and it all be done automatically. You will only need to focus on this Translation String area. Author translated in Afrikaans is 'outeur' [00:10:11](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m11s) Then you will select the Language (Afrikaans) for which that string belongs. Then save and close. From now on in any component where the word author is used, if the Afrikaans translation with relation to the other strings is enough, [00:10:35](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h10m35s) it will dynamically add this language to the component and you would not need to translate it again. This is all been the way it has been working up till now.

### New Area - Export And Import Strings From Spreadsheet - Dynamically Been Added

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=651" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

What is new, is that you can export these strings to a spreadsheet, and import them from the spreadsheet and it will dynamically be added. [00:11:04](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m04s)  I am going to select a few strings. You do not need to select any of the already translated strings, but if you do, it will also be used if it does not really matter.

 I am going to select a few and click export data. This will create an Excel Spreadsheet, which you can then save. [00:11:32](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h11m32s) I have opened the spreadsheet that has a number of IDs, then it has English. It got the tag of the language, and it got the value that we already set. I am going to set the value for these others in the spreadsheet. You got your Language file back from your translators. [00:12:00](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m00s)  They translated it to this column (See video). You can have multiple languages, every language will have its own column.

### Important - Top Header Is Language Tag/Langauge Is Created And Published

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=733" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Ensure that this top header is the language tag. It is important that this language is created and published in your system. Do not let them change the English string. [00:12:29](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h12m29s) When you import this file the system will look for the ID and the string, to identify that this value exists. If it does not exist it will simply ignore it. If you change 'author', even though the ID remains, the same, it will not find it and it will simply ignore this line.

### Demonstration

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=771" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

To demonstrate this, I am going to change the spelling of Back to have two k's. Save this document and go back and import it. [00:13:00](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m00s) The import is simple, just click on Import Data. Then select the file from our system, click Upload File and it should dynamically map the columns in your spreadsheet to the table columns. You would have your language strings if you got multiple language. It should automatically be mapped in.

 If you have multiple languages and you only want to import the one language, [00:13:35](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h13m35s) then all you need do is, add this 'Ignore This Column' next to the language you do not want to import. Then you click continue. You will now see that it has added translations, except for 'Back'. At first, I did not add these so I had to quickly go and add a little fix to the import.  [00:14:06](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m06s) I did not realize that at the moment it would stop at the first failure and not import further. But I have just fixed that and within the next update, this should be resolved.

The point is once you have imported it, you will see that it has added the translations to those Strings and it is also mapped to the correct language. [00:14:27](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h14m27s)  But 'Back' was not imported because the English string did not correspond. If we go back to our spreadsheet and fix this little error, and make a little tweak to one of the other strings, just for example sake, and then go back and import this file after it has been saved. [00:15:02](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h15m02s)  Again Import Data and Browse. It may be seen that back has been done. The other one that we also played with was 'Close & New'. We added the 'tt' there. You are able to export these language strings, translate them in a spreadsheet and easily import that spreadsheet, which would automatically update your values.

### Changing The Percentage

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/q5NwKGnOHoQ?start=938" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you have updated more than 50% of the English strings to a specific language, it will automatically be added to your component. You can change this percentage by going to Options in JCB and then change Add Language: 'Select percentage any language should be translated before the system should add the language to the component during compilation'. [00:16:12](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h16m12s) If more than 50% of your English strings have been translated, it starts adding it to the component. If not, it will just ignore it. That is giving you a quick demonstration of the new Import/Export Option in translating the strings in your system and knowing that if you have translated any of these strings, [00:16:41](https://www.youtube.com/watch?v=q5NwKGnOHoQ&list=PLQRGFI8XZ_wtGvPQZWBfDzzlERLQgpMRE&t=00h16m41s) you need to do it once and it will dynamically be available to every other component that uses that field or that view and therefore these English strings.

</div>
