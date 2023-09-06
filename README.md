# my2-Baddam
# Vennela Reddy Baddam 
###### Favourite vacation spot : India
I love India because my family ,friends and everyone whom I love lives there . Most importantly I am a **devitional person** . I like to visit **temples** every month atleast thrice

----
## Best Tourist spots i love visiting.
1. Favourite Spot
    1. Bejjanki
    2. Chirala
    3. Hyderabad
    4. Karimnagar
    5. Bali

* Food at Vacation Spot
    * Chicken Biryani
    * Paneer Biryani
    * KFC
    * Taco Bell 

    [click on the link for more info](MyStats.md)

    ----
    # Table for Recommending 4 sports
    I am Recommending these 4 sports because of its importance towards healthy lifestyle

    |Name of the sport| reason for recommend|Total hours|
    |-----------------|---------------------|-----------|
    |1.cricket        |concentration        |2hrs       |
    |2.running        |fitness              |2hrs       |
    |3.swimming       |fitness              |1hr        |
    |4.cycling        |Strength             |1hr        |

    ----
    # Pithy quotes.
> 1."No great discovery was ever made without a bold guess." ― *Isaac Newton*

> n2."If I could explain it to the average person, I wouldn’t have been worth the Nobel Prize." - *Richard Feynman*

    ----
    # Code fencing
    **Why do my CSS media queries not work on all mobile devices?**

    In my external stylesheet I have the following media query codeblock at the very end, which changes styles of previously defined classes

    [click on the link](https://stackoverflow.com/questions/77048496/why-do-my-css-media-queries-not-work-on-all-mobile-devices)

```
    (function($) {
    $.fn.drags = function(opt) {

        opt = $.extend({handle:"",cursor:"move"}, opt);

        if(opt.handle === "") {
            var $el = this;
        } else {
            var $el = this.find(opt.handle);
        }

        return $el.css('cursor', opt.cursor).on("mousedown", function(e) {
            if(opt.handle === "") {
                var $drag = $(this).addClass('draggable');
            } else {
                var $drag = $(this).addClass('active-handle').parent().addClass('draggable');
            }
            var z_idx = $drag.css('z-index'),
                drg_h = $drag.outerHeight(),
                drg_w = $drag.outerWidth(),
                pos_y = $drag.offset().top + drg_h - e.pageY,
                pos_x = $drag.offset().left + drg_w - e.pageX;
            $drag.css('z-index', 1000).parents().on("mousemove", function(e) {
                $('.draggable').offset({
                    top:e.pageY + pos_y - drg_h,
                    left:e.pageX + pos_x - drg_w
                }).on("mouseup", function() {
                    $(this).removeClass('draggable').css('z-index', z_idx);
                });
            });
            e.preventDefault(); // disable selection
        }).on("mouseup", function() {
            if(opt.handle === "") {
                $(this).removeClass('draggable');
            } else {
                $(this).removeClass('active-handle').parent().removeClass('draggable');
            }
        });

    }
    })(jQuery);

```


[Source for the above snippet](https://css-tricks.com/snippets/jquery/draggable-without-jquery-ui/)

[Click on the link](https://css-tricks.com/snippets/jquery/draggable-without-jquery-ui/)
