## HOW TO EDIT TIMELINE
**If New Event(s) Contains Photo, Please Upload the files in the following URL**

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

------------

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
