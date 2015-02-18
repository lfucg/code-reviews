# Let's create a simple form
## Is anything is wrong with the current page?

#### Like this government website asks:

<img width="600px" src="https://raw.githubusercontent.com/lfucg/code-reviews/master/images/is-there-anything-wrong.png" alt="is there anything wrong with this site">

### Sign in to a google account (create one if needed)

* Google Drive > [Create a new form](http://docs.google.com/forms/create?usp=about_productspage&authuser=0)
* You're now in the form designer
* Form Settings > allow for anyone to see the form

### Add questions

* `What you where doing`
* `What went wrong`
* Let's set the form title to `Help us to improve LexingtonKY.gov` with subtext `Don't include personal or financial information`
* Create the confirmation text: `Thank you for your help!`
 


### Let's add it to our Computer Services demo from last week

* File > Embed > Copy the iframe snippet to the clipboard
* Visit your index.html from last week and paste the iframe above the footer.
* Open index.html in the browser
* Not terrible, but the form takes up a lot of space on the page.

### Let's hide the form until someone clicks the `Is there anything wrong` link

* Create the link above our iframe


```
  <a class="feedback" href="#">Is there anything wrong with this page?</a>
    
  <iframe style="display:none" id="feedback-form" src="https://docs.google.com/forms/d/1zREHXRmHdxVNBcObm2OEerW8PEtW2rrIviQVfSL6uC0/viewform?embedded=true" width="760" height="500" frameborder="0" marginheight="0" marginwidth="0">Loading...</iframe>
```

### Let's add the jQuery javascript library to select elements from the page

* below the footer add

`<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>`


### Add a javascript section that programs our document

When someone clicks on the link, it tells the feedback form to show itself:

```
      <script type="text/javascript">
        $('a.feedback').click(function(e) {
          e.preventDefault();
          $('#feedback-form').show();
        });
      </script>
```

### Now click the link and submit the form to make sure it works!



### Ideas for improvement

* Improve the style of the form so that it matches the surrounding page better
* Make `what you were doing` required in the google form editor
* Email yourself when someone submits a form entry
