## HOW TO EDIT TIMELINE
**If new event contains photo, please upload the files in the following url**

 1. Go to https://github.com/nusmss/website-events-timeline/tree/main/CLICK_HERE/img
 2. Click 'Add file' at the top right side of the text editor
 3. Click 'Upload files'
 4. Choose the photo(s) in your computer
 5. Press Enter
 6. Upload successfully!

**Edit Event Data**

 1. Go to file at https://github.com/nusmss/website-events-timeline/blob/main/CLICK_HERE/edit.js
 2. Click the edit 'pencil' icon located at the top right side of the text editor
 3. Copy the Sample Code below for EACH of your new event

    	{
			time: "YYYY-MM-DD",
			header: "TYPE_HEADER_HERE",
			body: [
				{
					tag: "p",
					content: "TYPE_CONTENT_HERE",
				},
				{
					tag: "p",
					content: "TYPE_MORE_CONTENT_HERE_IF_NEED_OTHERWISE_REMOVE_FROM_3LINES_ABOVE_AND_1LINE_BELOW",
				},
			],
		},

 4. Understand that the codes you see is in sequence to the timeline displayed. Find the place where you would like to insert the new content
 5. Paste in that area (Take note that for every opening curly brackets "{" and closing "}", there does not exist any extra commas)
 6. Edit the respective values
 7. Save the file, by clicking on the 'Commit changes' green button at the bottom.
 8. Done. Now check on your live website (Events page) whether it has been updated! :)


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
        and (max-width : 768px) { 
            .timeline-iframe{
                border: none;
                overflow: hidden;
                position: relative;
                border: 0;
                height:8361px;
                width: 100%;
                overflow: hidden !important;
            }
        }
    </style>


## Preview

https://nusmss.github.io/website-events-timeline