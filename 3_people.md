---
layout: page
title:  "People"
people:

  - name: Jenny Gallop
    cv: |
      **2011 - now**: Group Leader, Gurdon Institute  
      **2006 - 2011**: Postdoc and EMBO fellow in laboratory of Marc Kirschner, Harvard Medical School, Boston, USA  
      **2001 - 2006**: PhD and short postdoc in Harvey McMahon's lab, MRC Laboratory of Molecular Biology, Cambridge, UK  
      **1997 - 2001**: Masters degree in Biochemistry, University of Oxford, UK  
    research: actin polymerisation, membranes, filopodia formation, cell shape, cell movement, signaling to actin, the membrane-cytosol interface
    about:  I enjoy looking after my children, Pilates and organising old photographs.
    picture: jenny2014.jpg

  - name: Julia Mason
    cv: |
      **Position**: Lab Manager since the lab started in 2011  
      **Previous positions**: I have worked at the Gurdon Institute for many years supporting the research of a number of labs.  
    research: Molecular Biology, Cell culture and Xenopus in vivo studies
    about: I enjoy spending time with my family and my dog.
    picture: julia_profile.jpg

  - name: Iris Jarsch
    cv: |
      **Position**: ERC Research Associate, joined the lab in August 2014.  
      **Previous positions**: Diploma in Genetics at LMU Munich; Dr. rer. nat. in the laboratory of Thomas Ott, LMU, Munich, studying the role of remorin proteins and membrane compartmentalisation in plant defence.  
    research: Discovering functional connections between the components of the filopodial tip complex.
    about: I like sports, travelling, cooking, meeting friends and spending time out in nature.
    picture: iris-profile.jpg

  - name: Hanae Shimo
    cv: |
      **Position**: Funai Overseas Scholarship PhD student (Biochemistry), joined the lab in September 2014.  
      **Previous positions**: M.S. in Systems Biology at Keio University
    research: Investigating the molecular architecture of filopodia-like structures using super-resoultion microscopy
    about: I enjoy traveling, photography, and playing guitar.
    picture: hanae-profile.jpg

  - name: Jonathan Gadsby
    cv: |
      **Position**: ERC Research Associate, joined the lab in January 2015.    
      **Previous positions**: B.Sc. in Molecular Biology & Biochemistry at Durham University; M.Res. at Newcastle University; PhD and short postdoc in the lab of Mette Mogensen at UEA, Norwich, studying microtubule +TIPs in epithelial differentiation and cancer. 
    research: Examining how actin polymerisation is responsive to phosphoinositides and membrane curvature. 
    about: I enjoy cricket and playing the bassoon & clarinet.
    picture: jonathan-profile.jpg

  - name: Ulrich Dobramysl
    cv: |
      **Position**: Hershel Smith Postdoctoral Fellow, joined the lab in October 2015.     
      **Previous positions**: Postdoctoral Researcher at the Mathematical Institute, University of Oxford; PhD in Theoretical Physics at Virginia Tech; Diploma in Engineering Physics at Johannes Kepler University Linz, Austria.
    research: Data-driven modeling of actin dynamics inside filopodia, stochastic modeling of biological processes. [[personal website](http://ulido.github.io)]
    about: I enjoy spending time with my family, tinkering, hiking, skiing and reading a good book.
    picture: uli-profile.jpg

  - name: Benjamin Richier
    cv: |
      **Position**: ERC research associate, joined the lab in November 2015.  
      **Previous positions**: PhD in Gif sur Yvette, France in the lab of François Rouyer at the INAF studying circadian rhythms in Drosophila then Postdoc in the lab of Iris Salecker at the NIMR in London where I worked on the development and morphogenesis of glial cells in the Drosophila visual system.  
    research: I use Drosophila to study actin regulation and filopodia formation in vivo.
    about: I like climbing, hiking and all sports/activities that require a good balance.
    picture: ben-profile.jpg  

  - name: Bishara Marzook
    cv: |
      **Position**: ERC research associate; joined the lab in October 2017.  
      **Previous positions**: PhD student at The University of Sydney, Australia, in Virology and Cell Biology. I worked on generating recombinant fluorescent viruses to study how vaccinia virus interacts with the host cytoskeleton, particularly with cytoplasmic actin isoforms.  
    research: I am interested in all things actin-related, focusing at the moment on filopodia formation. Also keeping on eye on the virus world!
    about: I love to communicate (by writing, telling jokes, or through radio/social media), bake, and take long walks/hikes to offset said baking.
    picture: bishara-profile.jpg  

alumni_postdocs:
  - name: Astrid Walrant
    comments: |
      now Maître de conférences at Université Pierre Paris 6, Pierre et Marie Curie.
      Reconstituted SNX9 actin polymerization in vitro (PNAS 2013, Methods in Cell Biology 2015, JCB, 2017)

  - name: Yoshiko Inoue
    comments: |
      now staff at Research Organization of Information and Systems, Japan.
      Moved to us from Nick Brown's lab, our first Drosophila geneticist, established flies and CRISPR/Cas9 methods in the lab

  - name: Frédéric Daste
    comments: |
      now on career break for family and writing new research projects.
      Elucidated mechanisms of SNX9 in actin polymerization and membrane curvature (JCB review, 2016, JCB article, 2017)

  - name: Vasja Urbančič
    comments: |
      now moving into data science.
      Developed Filopodyan image analysis pipeline in Xenopus retinal ganglion cell growth cones (JCB tools, 2017)

  - name: Claire Mulvey
    comments: |
      now working on a Grand Challenge with Greg Hannon at Cambridge Research Institute.
    
alumni_phds_ras:
  - name: Daniel Saxton
    comments: |
      former research assistant, now PhD student at University of Berkeley, USA.
      Developed methods for looking at filopodia-like structure elongation (Methods in Cell Biology, 2015)

  - name: Helen Fox
    comments: |
      former PhD student, now a Project Manager at Eurofins.
      Looked at roles of Toca-1 interactions in actin polymerization (CSH protocols, in press, JBC, 2016)


header: |
  <style>
    div.person p {
      margin: 0em;
    }
    div.person ul {
      margin: 0em;
    }
    div.person h3 {
      margin: 0em;
    }
    div.person {
      margin-bottom: 2em;
    }
    div.person div.picture {
      float: left;
    }
    div.person div.picture img {
      width: 6em;
      margin-right: 1em;
    }
    div.person ul {
      overflow: hidden;
    }
    div.alumni ul li p {
      margin: 0em;
    }
    div.alumni h2 {
      margin-bottom: 0em;
    }
    div.alumni ul {
      margin-top: 0em;
    }
  </style>
---

{% for person in page.people %}
<div class="person" markdown="1">


### {{ person.name }}
<div class="picture"><img src="photos/{{ person.picture }}"/></div>

{{ person.cv }}
**Research area:** {{ person.research }}

**About me:** {{ person.about }}
<div style="clear: both;"></div>
</div>
{% endfor %}

<div class="alumni" markdown="1">
## Alumni*
*All alumni have been listed with prior consent, with the option of withdrawing this information at any point in time. (Please use the email address listed on the Contact page if you would like to be removed)

#### Former postdocs
{% for person in page.alumni_postdocs %}
* **{{ person.name }}**{% if person.comments %}: {{ person.comments }} {% endif %}
{% endfor %}

#### Former PhD students and research assistants
{% for person in page.alumni_phds_ras %}
* **{{ person.name }}**{% if person.comments %}: {{ person.comments }} {% endif %}
{% endfor %}


</div>