:title: FOSS Concepts Intro
:author: D. Joe Anderson
:css: iat-style.css

---- 

.. note: (Name and title slide)

Free & Open Source Software Concepts
====================================
A brief introduction
--------------------

D\. Joe Anderson
................

University of Rochester
October 2017

.. note: running heads:

.. note: FOSS Concepts Intro GIS XYZ

---- 

Rough outline
=============

 - Software freedom: What is it?
 - Legal restrictions
 - Expanding rights: Licensing
 - Example projects

.. note: In this talk I hope to draw out at least a little more what the
         "freedom to fork" means, to legal conditions that require us to
         take specific steps to exercise that right; the legal tools that
         have been created to open room for exercising that right, called
         "licenses"

----

Terminology note
================

.. note:  People occasionally try to come up with different ways of saying
          largely the same thing.

.. image:: images/standards.png
    :width: 500px
    :height: 283px

.. note: standards.png PNG 500x283 500x283+0+0 8-bit sRGB 256c 24.3KB 0.000u 0:00.000
.. note: https://imgs.xkcd.com/comics/standards.png
.. note: https://xkcd.com/927/

https://xkcd.com/927/

---- 

Terminology note
================


 - *free software*
 - *open source*
 - *free and open source software* (FOSS)
 - *free, libre, and open source software* (FLOSS)
 - *public software*

Think **free** as in **freedom** rather than  *available at no (additional) cost*.


.. note: These terms are used differently within the field to indicate
         differences in philosophy or approach that are too abstruse to get
         into for a general audience.  Of course I have opinions about all
         of this and would love to talk about it, but to do so would keep us
         from the fundamentals.  I'll generally use "free software" or "FOSS
         but usually the other terms would do.

---- 

What is "software freedom"?
===========================


The 4 R's
---------

----

What is "software freedom"?
===========================

 - **Run**
 - **Read**
 - **Revise**
 - **Redistribute**

----

What is "software freedom"?
===========================




Run
---

----

What is "software freedom"?
===========================


.. image:: images/Screenshot_from_2017-10-17_15-24-23-osd-small.png

---- 

What is "software freedom"?
===========================


.. image:: images/Screenshot_from_2017-10-17_15-25-38-osd-big-no-discrimination.png

----

What is "software freedom"?
===========================


*Run*

Read
----

----

What is "software freedom"?
===========================

*Run*

*Read*

Revise
------

----

What is "software freedom"?
===========================

*Run*

*Read*

*Revise*

Redistribute
------------

---- 


What is "software freedom"?
===========================

 - **Run**
 - **Read**
 - **Revise**
 - **Redistribute**

.. note: A brief preview of an idea we'll expand on later, bears repeating because it's the essence of the subject.

Or, to put it most briefly, the essential freedom for FOSS is the:

**Freedom to *fork***

.. note: In the most simple terms, the essence of free software and free culture is the **freedom to fork**, which is to say, to take a work, make a copy of it, and work on it as if it were your own.

.. note: and to make or improve works with the intention of allowing others also to fork

.. note: This broadens what can be done with any given work, and it broadens who can do it.

.. note: There's something counter-intuitive here, almost a paradox, that I think
         academics in particular get wrong: Sure, this enables the lone
         genius to go off and reshape or recreate something from the pieces
         and parts from various projects.  Going in the other direction,
         though, the freedom to go off and do your own thing is crucial to
         creating the conditions for the kind of meaningful, sustainable
         collaboration and cooperation that is so crucial for so much
         academic work.

.. note: here we've answered one question but created another: What do we
         mean by the freedom to fork.

  
.. note:  Slide with 4 R's listed (the What)

.. note: refer to FSF 4 freedoms, to open content 5 Rs, to DFSG and OSD.

.. note: warn against "free" for specific user licenses.

.. note: maybe a slide of OSD or DFSG with just no discrimination clause.

.. note: Slide with IP categories listed. (the Why) ok maybe not

.. note:  DFSG with no discrimination highlighted 

---- 

Software freedom: Practical constraints
=======================================
Rights, restrictions, and licensing
-----------------------------------

Rights without restrictions

  - public domain

.. note: eg GRASS

Rights for some, restrictions for others

  - trade secret
  - patent
  - copyright
  - trademark

... which require *licenses* (mostly).

.. note: put concepts list here, for a little more detail, the reason we
         have to worry about this, can't just say "I don't care what someone
         does why do I have to bother with all this" or "I just want to use
         it for this one little thing, I don't see what the big deal is."

.. note: mostly means NDA, contracts, right-of-first-sale.

---- 

End User License Agreement
==========================

.. image:: images/terms_1.png
    :width: 300px
    :height: 190px


Robert Sikoryak_ 

.. _Sikoryak: https://en.wikipedia.org/wiki/Robert_Sikoryak

.. note: https://www.drawnandquarterly.com/sites/default/files/styles/creation-gallery/public/images/creations/gallery/Terms%20and%20Conditions/terms_1.png?itok=6XB4lN40

.. note: https://itunestandc.tumblr.com/



---- 

.. note: RRL gives rise to things like this
.. note: 108 pages, graphic novel unabridged version at the time of his writing it

.. note: TMNT https://itunestandc.tumblr.com/image/134588049070 
.. note: https://78.media.tumblr.com/96c42c8373049e01f5a83c0f606e207c/tumblr_nyqn70RGPx1ugej69o1_1280.jpg

.. image:: images/tumblr_nyqn70RGPx1ugej69o1_1280.jpg

---- 

.. note: MLP https://itunestandc.tumblr.com/image/133927463577 
.. note: https://78.media.tumblr.com/4257efd86ce979895d533f42798fac8e/tumblr_ny6cfwI3WS1ugej69o1_1280.jpg

.. image:: images/tumblr_ny6cfwI3WS1ugej69o1_1280.jpg

---- 

End User License Agreements
===========================
The problem with proprietary EULAs
----------------------------------

Great big documents to allow you to do very little.

**Red tape** around a **black box**

They prevent or make difficult:

 - peer review
 - scutiny
 - accountability
 - reproducibility
 - incremental progress

One thing they tend to get right

 - attribution

.. note: credit doesn't mean control, or recompense

---- 


Rights, restrictions, and licensing
===================================

 - *Who?* 
 - *What?*
 - *Why?* 
 - *When?*
 - *How?* 

.. note: Who can get the rights, who gets limited by them
.. note: What is covered by what restrictions
.. note: Why create restrictions
.. note: Where do these restrictions apply
.. note: When and how does it expire
.. note: How and when does something become covered

---- 


.. note: Excerpt from Constitution

Patent and Copyright Clause 
===========================
U.S. Constitution 
-----------------

[The Congress shall have power] "To promote the **progress of science and useful arts**, by securing for **limited times** to **authors and inventors** the **exclusive right** to their respective **writings and discoveries**."

*Article I Section 8. Clause 8*

.. note: This is US federal jurisdiction. Used to be more localized, with
         state and even local law in the US weighing in.  Now
         internationalized and harmonized through for instance the Berne
         Convention (US 1989), though still with differences from
         country-to-country.

----


Patent and Copyright Clause 
===========================
Summarized
----------

 - *Who?* **authors & inventors**
 - *What?* **writings & discoveries**   
 - *Why?* **progress** 
 - *When?* **limited time**
 - *How?* **exclusive rights**

---- 


Patent and Copyright Clause 
===========================

 - applies at the federal level
 - current law mostly supplants state & local law
 - current law implements international agreements
 - differs in subtle ways from international counterparts

 - USPTO
 - copyright.gov
 - Library of Congress

----


Rights, restrictions, and licensing
===================================
Focus on copyright
------------------


  - trade secret
  - patent
  - **copyright**
  - trademark
  - public domain

.. note: copyright: for authors
    applies to creative expression (very broadly: literature, art. cf djb vs us)
    not for facts or automatic work (cf phone books, databases)
    arises automatically (per Berne vide supra) on creation
    can be registered: damages vs injunctive relief
    life of author plus 70 (120 from creation, 95 from pub. Up from 14x2)
    not for US govt (cf Crown Copyright and OSM)
    limited by fair use (do ToS override fair use?)
 
.. note: trade secret, in principle for ever, cumbersome, rev eng, Coke formula
.. note: patent, 20 years, first to file, prior art, novel, practical, must apply
.. note: trademark, logos and brand names, start by using, protects consumers from "confusion", must defend from becoming generic. Xerox. Kleenex. Hoover.
.. note: public domain, US federal govt (but not UK!) works not copyrightable, when copyright, patent expires, trademark becomes generic.

.. note: Slide highlighting just copyright.

.. note: but where do these come from?


---- 

.. note: Freedom to fork: Reprise

What do we want?
================

- **Run**
- **Read**
- **Revise**
- **Redistribute**

How do we get it?
-----------------
  
.. note:  Slide with 4 R's listed (the What)

.. note: refer to FSF 4 freedoms, to open content 5 Rs, to DFSG and OSD.

.. note: warn against "free" for specific user licenses.

.. note: maybe a slide of OSD or DFSG with just no discrimination clause.

.. note: Slide with IP categories listed. (the Why) ok maybe not

.. note:  DFSG with no discrimination highlighted 

---- 



Free software licenses
======================

.. note: compare and contrast with proprietary EULAs

For software

 - Permissive, non-reciprocal
   - MIT expat or X11
   - BSD 2-clause or 3-clause
   - Apache
 - Copyleft
   - varieties of the GPL
   - Oracle (via Sun) CDDL

Non-software

  - GFDL
  - Creative Commons
    - BY attribution
    - [SA] share-alike (copyleft)
    - (NC) non-commercial (unfree)
    - (ND) no-derivatives (unfree)


---- 

Examples
========

Classic FOSS & Free Culture

 - Linux
 - Firefox
 - Wikipedia

FOSS for GIS examples

 - QGIS
 - OpenStreetMap

---- 

QGIS
====
 
  - cc-by-sa 3 for website
  - Wikipedia just says **GPL**
  - download, sources says GPL but not what version 
  - get involved --> development --> GIT Access --> Accessing the repository
  - v2 and above https://github.com/qgis/QGIS

.. note: very nice, there's a repo for the website

---- 

Open Street Map
===============

