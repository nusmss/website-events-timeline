

## CDN
**CSS**

 - https://nusmss.github.io/website-events-timeline-mobile/

**JS**

 - https://nusmss.github.io/website-events-timeline/js/jquery-timeline.min.js
 - https://nusmss.github.io/website-events-timeline/js/data-nusmss-timeline.js


**iFrame Code:**

    <iframe
    src="https://nusmss.github.io/website-events-timeline"
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
                height:4610px;
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
                height:4610px;
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
                height:6000px;
                width: 375px;
                overflow: hidden !important;
            }
        }
    </style>

## Preview

https://nusmss.github.io/website-events-timeline