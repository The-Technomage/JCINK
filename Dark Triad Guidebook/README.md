Thank you for downloading my Dark Triad Tabbed Guidebook! Getting this guidebook set up on your site is super simple. Just follow these steps:
1. Open dark-triad.css and dark-triad.html in the notepad program of your choice. Using Word, WordPad, LibreOffice, or a similar editor may cause the code to break.
2. Create a new webpage on your site if you don’t already have one set up.
3. Add the contents of dark-triad.css to the bottom of your site’s stylesheet.
4. Add the contents of dark-triad.html to the webpage you’ve created, and input your information.

Customizing
Customizing fonts and accent colours is done through variables, which can be found at the very top of the dark-triad.css file. If you’re unfamiliar with how CSS variables work, simply find the section below, and replace the bold part with the font or HEX/RGB code of your choice. It will automatically update throughout the CSS for you.
```  --main-font: Verdana, "Verdana Ref", sans-serif;
  --second-font: Impact, "Arial Black", sans-serif;
  --text-colour: #aaaa;
  --accent-colour: #a22c29;
  --border-colour: #222222;```

Adding More Tabs
Your new guidebook is equipped with 5 sections to start with. If you’d like to add more sections, that’s also super easy! First thing is to find this in your dark-triad.html file:
```    <label for='tab-4'>Tab 4 Link Title</label>
    <label for='tab-5'>Tab 5 Link Title</label>```

These are how new “links” to the various tabs of the guidebook are created. All you need to do is add a few more labels, ensuring that you change the “for” section to the next highest number, such as:
```    <label for='tab-6'>Tab 5 Link Title</label>```

Now, if you scroll further down the page, you’ll find something that looks like this:
```    <! -- Tab 5 contents start -->
    <input type='radio' name='tab-group' class='guide-radio' id='tab-5' />
    <div class='guide-content'>
      <h2>Tab 5 Title</h2>
      Tab 5 contents go here
    </div>
    <! -- Tab 5 contents end -->```

You’ll simply need to duplicate this, and make sure that the number in the ID matches up in the “for” section of your label, like this:
```    <! -- Tab 6 contents start -->
    <input type='radio' name='tab-group' class='guide-radio' id='tab-6' />
    <div class='guide-content'>
      <h2>Tab 6 Title</h2>
      Tab 6 contents go here
    </div>
    <! -- Tab 6 contents end -->```

And now you should be ready to go! Thanks again for downloading the Dark Triad Tabbed Guidebook!
