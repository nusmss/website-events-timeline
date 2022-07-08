## HOW TO EDIT TIMELINE
**If New/Existing Event(s) Contains/Needs Photo, Please Upload the files in the following URL**

 1. Go to https://github.com/nusmss/website-events-timeline/tree/main/CLICK_HERE/img
 2. Click 'Add file' at the top right side of the text editor
 3. Click 'Upload files'
 4. Choose the photo(s) in your computer
 5. Press Enter
 6. Upload successfully!

**Edit Event Data**

 1. Go to file at https://github.com/nusmss/website-events-timeline/blob/main/CLICK_HERE/edit.js
 2. Click the edit 'pencil' icon located at the top right side of the text editor
 3. Copy and Modify the Sample Code below for EACH of your New Event(s)

    	{
            time: "YYYY-MM-DD",
            header: "[EVENT_TITLE_TOP_HEADER]",
            body: [
            {
                tag: "h1",
                content: "[EVENT_TITLE_IF_NOT_REQUIRED_REMOVE_2LINES_ABOVE_AND_1LINE_BELOW_INCLUSIVE]",
            },
            {
                tag: "img",
                attr: {
                src: "CLICK_HERE/img/[INSERT_UPLOADED_FULL_FILENAME_IF_EVENT_NO_IMAGE_REMOVE_4LINES_ABOVE_AND_4LINES_BELOW_INCLUSIVE]",
                width: "100%",
                cssclass: "img-responsive",
                },
            },
            {
                tag: "p",
                content:
                "[INSERT_FIRST_PARAGRAPH_TEXT]",
            },
            {
                tag: "p",
                content:
                "[INSERT_SECOND_PARAGRAPH_TEXT_IF_ANY_OTHERWISE_JUST_REMOVE_3LINES_ABOVE_AND_1LINE_BELOW_INCLUSIVE]",
            },
            ],
        },

 4. Understand that the codes you see is in sequence to the timeline displayed. Find the place where you would like to insert the new content
 5. Paste in that area (Take note that for every opening curly brackets "{" and closing "}", there does not exist any extra commas)
 6. Edit the respective values
 7. Save the file, by clicking on the 'Commit changes' green button at the bottom.
 8. Done. Now check on your live website (Events page) whether it has been updated!
    
    (In most cases, you will need to resolve the '**CROPPED OUT EVENTS TIMELINE**' issue described below. If necessary, follow the instructions)

## Preview

https://nusmss.github.io/website-events-timeline


## HOW TO RESOLVE CROPPED OUT EVENTS TIMELINE

**Solution (Steps might be slightly technical. Screenshots with instructions are provided to assist you)**
1. On your Website Builder, go to Events page.
2. Now click on the 'Events' element you see on the page and click on Edit Widget.
   
   ![](https://i.imgur.com/AtKyTYU.png)
3. Click 'Code' on the top right in your web builder.
   
   ![](https://i.imgur.com/KyRWGth.png)

Continue with the following steps (Open another tab, preferably now you have 2 windows side-by-side)
 1. Open https://nusmss.micronify.com/events
 2. Right-click on the events timeline, and click 'Inspect', revealing side developer console.
    
    ![](https://i.imgur.com/6Eeo0ul.png)
 3. On the side developer console, on its most top left hand side, second button from the left, click on the 'mobile' icon. <-- this will show you the different mobile sizes.
    
    ![](http://tiny.cc/t69tuz)
 4. Now, on the top left side, change the 'Dimensions' to 'Responsive'. Notice the 2 textboxes beside it, for manual input of [width x height].
    
    ![](http://tiny.cc/q69tuz)
 5. You will be able to see on the screen, there are draggable right tool and draggable bottom tool for you to adjust the screen sizes accordingly.
    
    ![](http://tiny.cc/u69tuz)
 6. But to save time, we will set the dimension via 'width' textbox field in Step 7 instead. Below is the Sizing Chart. Take note of the bold "Use 'xxx'" value, where x represents the value you should use for input later.
    
    **Mobile Responsive Sizing Chart**
    
    We will need to change the height for the different screen sizes:
     1. Desktop (width: 1201 pixels & beyond) **<-- Use '1201'**
     2. Tablet (width: 768 to 1200 pixels) **<-- Use '769'**
     3. Mobile (width: 490 to 768 pixels) **<-- Use '491'**
     4. Smaller Mobile (width: 380 to 490 pixels) **<-- Use '381'**
     5. Smallest Mobile (width: 330 to 380 pixels) **<-- Use '331'**
     6. Smallestest Mobile (width: up to 330 pixels) **<-- Use '330'** (Which is same height as item above)
 
 7. For example, let's start with **Mobile**. Refer to the dimensions listed above, use the given number within quotes. Key in **'491'** into the width textbox field, and then press the 'Enter' key.
    
    ![](https://i.imgur.com/NyErCHf.png)
 8. Still on the developer console, use 'Ctrl + F' key to bring up the "search" console. In the search textbox, type '<iframe', and then press the 'Enter' key.
    
    ![](https://i.imgur.com/ZY1laJY.png)
 9. Now you will need to do trial-and-error of height values changing for each of the Mobile Responsive Sizes listed above. Increase or decrease the height value as needed, while paying attention to the preview screen on the left if the cropping/extra space issue has been fixed. (**ONLY CHANGE THE HEIGHT**, leave everything else as it is)
    
     ![](https://i.imgur.com/RLV7n01.png)
     
     ![](https://i.imgur.com/dR4Nc65.png)
 10. Once you have found the most suitable height value, copy that value and replace the existing value, inside your Website Builder's Code, with it.
  
     ![](https://i.imgur.com/XfmAMsL.png)
 11. Save your new Website Builder's Code for each time.

     ![](https://i.imgur.com/WxGIfmj.png)
 12. Repeat steps 7 to 11 for each of the six different mobile sizes shown in the above Mobile Responsive Sizing Chart.


**Testing of Different Mobile Sizes using Web Builder**
  1. Click 'Preview' button at the top to select; Desktop, Tablet, Mobile.
     
     ![](https://i.imgur.com/ugxEEan.png)
     
## FAQ ##
  1. I have completed all steps successfully but when I visit the website, it is still not updated?
     
     This is usually due to a problem with your browser's cache. You can either clear your browser cache or wait a while. You can also test the changes in an incognito window to see if they are reflected. The cache is not stored in the incognito environment.
     
------------
The codes below is a copy of what has been applied on your Web Builder. It is advised to update the codes below as backup whenever you made changes in the Web Builder, by editing this notes. <-- You can do so by clicking the 'edit' or 'pencil' button located at the top of this text viewer. After that, click the green 'commit changes' button.

**HTML Embed Code:**

    <iframe
    src="https://nusmss.github.io/website-events-timeline/"
    allowtransparency="true"
    scrolling="no"
    frameborder="0"
    allowTransparency="true"
    class="timeline-iframe"></iframe>

    <p>Your browser does not support iframes.</p>

    <style>

        /*DESKTOP*/
        @media only screen 
        and (min-width : 1200px)  { 
            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                min-height:11380px; 
                width: 1000px;
                overflow: hidden !important;
            }
        }

        /*TABLET*/
        @media only screen 
        and (min-width : 768px) 
        and (max-width : 1200px) { 
            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                height:16630px;
                width: 640px;
                overflow: hidden !important;
            }
        }

        /*MOBILE*/
        @media only screen 
        and (min-width : 490px) 
        and (max-width : 768px) { 
            .preview-content-holder.shrinker-content {
                width: 100%;
                margin: auto !important;
            }

            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                height:13250px;
                width: 440px;
                overflow: hidden !important;
            }
        }

        /*SMALLER MOBILE*/
        @media only screen 
        and (min-width : 380px) 
        and (max-width : 490px) { 
            .preview-content-holder.shrinker-content {
                width: 100%;
                margin: auto !important;
            }

            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                height:11724px;
                width: 340px;
                overflow: hidden !important;
            }
        }

        /*SMALLEST MOBILE*/
        @media only screen 
        and (min-width : 330px) 
        and (max-width : 380px) { 
            .preview-content-holder.shrinker-content {
                width: 100%;
                margin: auto !important;
            }

            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                height:11290px;
                width: 295px;
                overflow: hidden !important;
            }
        }

        /*SMALLESTEST MOBILE*/
        @media only screen 
        and (max-width : 330px) { 
            .preview-content-holder.shrinker-content {
                width: 100%;
                margin: auto !important;
            }

            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                height:11262px;
                width: 265px;
                overflow: hidden !important;
            }
        }

    </style> 
