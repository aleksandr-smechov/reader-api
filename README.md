# Reader API

> Custom reader mode with a single GET request.

![Image of a book](https://cdn.pixabay.com/photo/2015/06/02/12/59/narrative-794978_1280.jpg)

Reader is a free readability-style API built on top of ![Extract Article Text](https://extractarticletext.com) and uses the same ![random-forrest-based ML model](https://github.com/aleksandr-smechov/vellichor) to extract relevant body text from editorial content like news articles, blogs, press releases, and so on.

Here's how it works:

1. Start with the base URL: https://extractarticletext.com/api/reader/
2. Add the API key: ?apikey=b6809899e431be42a883912aa148c6be03e16e9b
3. Add any parameters (see below).
4. Add a URL: &url=https://example.com

So, putting it all together, you get something like this (go ahead and give it a try!):

https://extractarticletext.com/api/reader/?apikey=b6809899e431be42a883912aa148c6be03e16e9b&url=https://example.com

![API example image 1](https://i.ibb.co/xXFWDLj/Annotation-2020-02-17-131944.png)

Pretty simple so far, right? Let's add some parameters to get funky with the results.

# Parameters

Say you're not too happy with that white background and Open Sans font. You can add the following parameters *between* your api key and url query strings. Like this (give it a click!):

https://extractarticletext.com/api/reader/?apikey=b6809899e431be42a883912aa148c6be03e16e9b&mode=night&font=lato&url=https://example.com

![API example image 2](https://i.ibb.co/wYxCCDX/Annotation-2020-02-17-132725.png)

Here are all the customization options:

* **mode**=*night/light*
* **font**=*opensans/roboto/lato/oswald/sourcesanspro/montserrat/ptsans/raleway/lora*
* **font_size**=*24px* (can be any size, just use "px" - 12px, 14px, etc.)
* **title_size**=*1/2/3/4/5/6* (heading sizes)

And that's it! Enjoy.

# TODO

- [x] Add a night mode
- [ ] Add author
- [ ] Add bold/italics options for first paragraph
- [ ] Add option to return HTML string
