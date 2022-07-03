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
 8. Done. Now check on your live website (Events page) whether it has been updated! :)

## Preview

https://nusmss.github.io/website-events-timeline


**For Mobile Responsive Sizes**
We will need to change the height for the different screen sizes:
 1. Desktop (width: 1200 pixels & beyond)
 2. Tablet (width: 768 to 1200 pixels)
 3. Mobile (width: 490 to 768 pixels)
 4. Smaller Mobile (width: 380 to 490 pixels)
 5. Smallest Mobile (width: 330 to 380 pixels)
 6. Smallestest Mobile (width: up to 330 pixels)

For non-technical:
Perform the heights changing trial-and-error via Edit Widget > Red Square Icon > Click 'Code' on the top right in your web builder. For each trial-and-error fixing of height values, adjust your browser (i.e. Chrome) window size to immitate all the above different screen sizes. Proceed with height value changing for the respective screen size (i.e. Desktop), for each change to be seen, click on the 'Save' button. And see if your newly updated events timeline is being showed as expected (i.e. scroll to the bottom and see if any content being cropped out). Alternatively, you may refer to the tutorial video by Ramadhan.

Technical & Faster Steps (using 'Inspect Element') <-- Watching Tutorial Video is recommended for visualisation
 1. Open https://nusmss.micronify.com/events
 2. Right-click on the events timeline, and click 'Inspect', revealing side developer console
 3. On the side developer console, on its most top left hand side, second button from the left, click on the 'mobile' icon. <-- this will show you the different mobile sizes
 4. Now, on the top left side, change the 'Dimensions' to 'Responsive'.
 5. You will be able to see on the screen, there are draggable right tool and draggable bottom tool for you to adjust the screen sizes accordingly.
 6. Use this screen sizing tool to simulate all of the 6 different Mobile Responsive Sizes indicated above.
 7. For trial-and-error of height values, you will need to find the '<iframe' word in the code display panel, and then change the height values accordingly. While doing this, you will notice the events timeline in the screen display will change in real-time. Hence, this method is more technical but faster steps.

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
                height:5202px;
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
                height:5926px;
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
                height:6390px;
                width: 100%;
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
                height:6630px;
                width: 100%;
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
                height:7190px;
                width: 100%;
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
                height:7400px;
                width: 100%;
                overflow: hidden !important;
            }
        }

    </style> 
