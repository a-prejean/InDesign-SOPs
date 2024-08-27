# InDesign-SOPs
SOPs for InDesign


*Both instances should always match since they're created from the same source.*


## Auto Build GitHub Pages
- Changes made in ***root/docs/*** will be reflected in https://a-prejean.github.io/InDesign-SOPs/index.html once committed


## Saving Static Site to Server
- Use ***mkdocs build*** and copy contents of created ***site*** folder to server


---


# Examples
i.e., ("that is")
e.g., (“for example”)


# Getting Started

Open Terminal
pip install mkdocs-material
  or, pip install --upgrade mkdocs-material

In Project Directory, in terminal:
mkdocs new .

pip install mkdocs-glightbox
  or, pip install --upgrade mkdocs-glightbox
  If getting no such file or directory, try
  pip3 install --upgrade pip
pip install --upgrade pip


# Previewing as you write
mkdocs serve
OR
mkdocs serve --dirtyreload
    for current page only

Point your browser to http://localhost:8000/


# Building your site
mkdocs build


If you intend to distribute your documentation as a set of files to be read from a local filesystem rather than a web server (such as in a .zip file)


# Building for offline usage
Add the following lines to mkdocs.yml:
plugins:
  - offline

### Limitations
All features that use the fetch API will error.
Disable the following configuration settings:
- instant loading
- site analytics
- git repository
- versioning
- comment systems


# Customization
In order to make a few small tweaks to Material for MkDocs, you can just add CSS and JavaScript files to the docs directory.
https://squidfunk.github.io/mkdocs-material/customization/



# Formatting
*Italic*
**Bold**
***Bold_Italic***
==Highlighted==
***==Highlighted_Bold_Italic==***


{==

Highlighted_Text_Block

==}


keyboard keys: ++ctrl+alt+del++



# Images

https://squidfunk.github.io/mkdocs-material/reference/images/

![Image_Title](../media/Image.png){ width="800" }

<!-- Image Left or Right Aligned -->
![Image_Title](../media/Image.png){ align=left }

<!-- Image Centered -->
<figure markdown="span">
  ![Image_Title](../media/Image.png){ width="600" }
</figure>

<!-- Image with Caption -->
<figure markdown="span">
  ![Image_Title](../media/Image.png){ width="600" }
  <figcaption>Image_Caption</figcaption>
</figure>



<!-- Text on Left with Image on Right -->
<div class="grid" markdown>

- TEXT

![Image_Title](../media/Image.png){ width="340", align=right }

</div>

<!-- use div to organize grid items -->
<div></div>
<!-- or -->
<div markdown>

</div>



# Navigation
Pages will show up in order listed in mkdocs.yml:

nav:
  - index.md
  - page.md



# Grid Layouts

<div class="grid" markdown>

Some Text

![Image_Title](../media/Image.png){ width="340", align=right }

</div>



# Callouts / Admonitions
!!! note
    TEXT

???+ note
    TEXT

!!! note ""
    TEXT


---

# Dividers
!!! DIVIDER ""


---

# Future Additions


---
