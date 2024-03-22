---
layout: distill
title: Pacific corals and SCTLD
description: Experimental notebook to test susceptibility of Pacific corals to SCTLD  
categories: research
tags: Pocillopora, ETP, SCTLD
giscus_comments: false
date: 2024-01-10
featured: true

authors:
  - name: Ana M. Palacio-Castro
    url: "anampc.github.io"
    affiliations:
      name: CIMAS, UM, AOML
  
<!---##bibliography: 2018-12-22-distill.bib -->

# NOTES:
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
#   - we may want to automate TOC generation in the future using
#     jekyll-toc plugin (https://github.com/toshimaru/jekyll-toc).
# toc:
  - name: Coral collection
    # subsections:
       - name: Permits
       - name: Travel
## - name: Citations


# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
_styles: >
  .fake-img {
    background: #bbb;
    border: 1px solid rgba(0, 0, 0, 0.1);
    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
    margin-bottom: 12px;
  }
  .fake-img p {
    font-family: monospace;
    color: white;
    text-align: left;
    margin: 12px 0;
    text-align: center;
    font-size: 16px;
  }
---

## Coral collection

Colonies were collected by Juan Mate and collaborators and brought to the STRI in [NAOS](https://stri.si.edu/facility/naos)

* Porites lobata: 6 colonies collected on February 26, 2024 
* Pocillopora: 10 colonies collected on March 1, 2024 
* Pavona clavus: 7 colonies collected on March 7, 2024

/Users/pachacuti/Documents/GitHub/anampc.github.io/assets/img/notebooks/Panama_SCTLD
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/notebooks/Panama_SCTLD/Plob_1.jpeg" title="Plob" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/notebooks/Panama_SCTLD/Plob_2.jpeg" title="Plob" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/notebooks/Panama_SCTLD/Plob_3.jpeg" title="Plob" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Pdam not looking so good on March 21. New colonies will be collected on March  25th. 

## Permits

### Export: CITES permits requested by Juan Mate

### Import:

* Make sure the CITES export permit from Panama is validated before the shipment leaves the country.

* Contacted fwsole_miami@fws.gov to make them aware of the samples coming. Instructions:  
	
	-	File a 3-177 Declaration (https://edecs.fws.gov/) prior to the import
	-	As part of the declaration, upload documents (you will have to combine them in one PDF) including:
		1. scans of the CITES permits
		2. specimen list (including scientific names, quantities, and description (live)
		3. scan of the air waybill or plane ticket (is this shipment being hand carried?)
		4. a short description of the research

	-	If landing on a weekday (M-F 8:00am to 4:00pm) Customs may call us to ask if we are aware of the shipment as the person is carrying the specimens through. 
	- 	If the shipment is outside of normal working hours, we may have to contact Customs to let them know to expect the shipment and the shipment will be assigned to the overtime inspector. 
	-	The original permits will need to be submitted to our office and then the declaration will be cleared in the computer. 
		You may either bring them into the office or send them through a reliable service such as FedEx with a tracking number.
	-	The management authority or Customs will sign off on the bottom portion of the permit and validate the number of animals being exported. 

At least 48 hours in advance, please email us again to remind us of the shipment as we require a 48-Hour Notice of any live or perishable imports. 


## Travel

* Arriving in Panama City on March 26th 
* Packing colonies in two coolers with paper towels, bubble wrap and some water. 
* Packing list -  Panama 

- ~~Passport~~
- ~~NOAA/UM IDs~~
- ~~Coolers~~
- ~~Ziplock bags~~ 
- ~~Bubble wrap~~
- ~~Paper towels~~
- ~~Copy of permits~~ 
- ~~Zip ties~~
- ~~Duct tape~~ 
- ~~Flights~~
- Hotel reservation

---

<!---## Citations

>Citations are then used in the article body with the `<d-cite>` tag.
The key attribute is a reference to the id provided in the bibliography.
The key attribute can take multiple ids, separated by commas.

The citation is presented inline like this: <d-cite key="gregor2015draw"></d-cite> (a number that displays more information on hover).
If you have an appendix, a bibliography is automatically created and populated in it.

Distill chose a numerical inline citation style to improve readability of citation dense articles and because many of the benefits of longer citations are obviated by displaying more information on hover.
However, we consider it good style to mention author last names if you discuss something at length and it fits into the flow well — the authors are human and it’s nice for them to have the community associate them with their work.

---

-->

!## Footnotes

Wrap the text you would like to show up in a footnote in a `<d-footnote>` tag.
The number of the footnote will be automatically generated.<d-footnote>This will become a hoverable footnote.</d-footnote>

---

!## Code Blocks

Syntax highlighting is provided within `<d-code>` tags.
An example of inline code snippets: `<d-code language="html">let x = 10;</d-code>`.
For larger blocks of code, add a `block` attribute:

<d-code block language="javascript">
  var x = 25;
  function(x) {
    return x * x;
  }
</d-code>

**Note:** `<d-code>` blocks do not look good in the dark mode.
You can always use the default code-highlight using the `highlight` liquid tag:

{% highlight javascript %}
var x = 25;
function(x) {
return x \* x;
}
{% endhighlight %}

---

!## Interactive Plots

Add interative plots using plotly + iframes :framed_picture:

<div class="l-page">
  <iframe src="{{ '/assets/plotly/demo.html' | relative_url }}" frameborder='0' scrolling='no' height="500px" width="100%" style="border: 1px dashed grey;"></iframe>
</div>

The plot must be generated separately and saved into an HTML file.
To generate the plot that you see above, you can use the following code snippet:

{% highlight python %}
import pandas as pd
import plotly.express as px
df = pd.read_csv(
'https://raw.githubusercontent.com/plotly/datasets/master/earthquakes-23k.csv'
)
fig = px.density_mapbox(
df,
lat='Latitude',
lon='Longitude',
z='Magnitude',
radius=10,
center=dict(lat=0, lon=180),
zoom=0,
mapbox_style="stamen-terrain",
)
fig.show()
fig.write_html('assets/plotly/demo.html')
{% endhighlight %}

---

!## Details boxes

Details boxes are collapsible boxes which hide additional information from the user. They can be added with the `details` liquid tag:

{% details Click here to know more %}
Additional details, where math $$ 2x - 1 $$ and `code` is rendered correctly.
{% enddetails %}

---

!## Layouts

The main text column is referred to as the body.
It is the assumed layout of any direct descendants of the `d-article` element.

<div class="fake-img l-body">
  <p>.l-body</p>
</div>

For images you want to display a little larger, try `.l-page`:

<div class="fake-img l-page">
  <p>.l-page</p>
</div>

All of these have an outset variant if you want to poke out from the body text a little bit.
For instance:

<div class="fake-img l-body-outset">
  <p>.l-body-outset</p>
</div>

<div class="fake-img l-page-outset">
  <p>.l-page-outset</p>
</div>

Occasionally you’ll want to use the full browser width.
For this, use `.l-screen`.
You can also inset the element a little from the edge of the browser by using the inset variant.

<div class="fake-img l-screen">
  <p>.l-screen</p>
</div>
<div class="fake-img l-screen-inset">
  <p>.l-screen-inset</p>
</div>

The final layout is for marginalia, asides, and footnotes.
It does not interrupt the normal flow of `.l-body` sized text except on mobile screen sizes.

<div class="fake-img l-gutter">
  <p>.l-gutter</p>
</div>

---

!## Other Typography?


[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links.
http://www.example.com or <http://www.example.com> and sometimes
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

Here's our logo (hover to see the title text):

Inline-style:
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style:
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

Inline `code` has `back-ticks around` it.

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting.
But let's throw in a <b>tag</b>.
```

Colons can be used to align columns.

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |   centered    |   $12 |
| zebra stripes |   are neat    |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| _Still_  | `renders` | **nicely** |
| 1        | 2         | 3          |

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a _separate paragraph_.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the _same paragraph_.
