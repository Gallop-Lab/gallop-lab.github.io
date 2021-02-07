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
    research: actin polymerisation, membranes, filopodia formation, cell shape, cell movement, signalling to actin, the membrane-cytosol interface
    picture: jenny2014.jpg

  - name: Julia Mason
    cv: |
      **Position**: Lab Manager since the lab started in 2011  
      **Previous positions**: At the Gurdon Institute for many years supporting the research of a number of labs  
    research: Molecular biology, cell culture and Xenopus in vivo studies
    picture: julia_profile.jpg

  - name: Jonathan Gadsby
    cv: |
      **Position**: Wellcome Trust Research Associate, joined the lab in January 2015.    
      **Previous positions**: BSc Molecular Biology & Biochemistry, Durham University; MRes Newcastle University; PhD and short postdoc in Mette Mogensen's lab at UEA, Norwich, studying microtubule +TIPs in epithelial differentiation and cancer 
    research: Examining how actin polymerisation is responsive to phosphoinositides and membrane curvature. 
    picture: Jonathan-profile2.jpg
    
  - name: Thomas Blake
    cv: |
      **Position**: Wellcome Trust Research Associate, joined the lab in January 2021 
      **Previous positions**: BA Natural Sciences and MSci Biochemistry, University of Cambridge; MRes and PhD Imperial College, London, and short postdoc in Jake Baum's lab studying myosin motors in malaria parasites
    research: Superresolution and rapid timelapse microscopy in studying filopodial initation and extension
    picture: 

  - name: Pantelis Savvas Ioannou
    cv: |
      **Position**: MedImmune PhD Student, joined the lab in October 2018  
      **Previous positions**: BSc in Biological Sciences and MSc in Biomedical Sciences at the University of Cyprus
    research: Using phage display antibody technology to find new filopodial proteins
    picture: pantelis.jpg
    
    
  - name: Pankti Vaishnav
    cv: |
      **Position**: Wellcome Trust Research Assistant, joined the lab in July 2020 
      **Previous positions**: BSc in Biochemistry, University of Birmingham and MRes in Molecular and Cellular Biosciences, Imperial College, London
    research: Molecular mechanisms of SNX9-mediated actin polymerisation
    picture: 

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
  
  - name: Benjamin Richier
    comments: |
      Moved back to family in france where he pursues new career opportunities. Joined the lab as drosophila specialist from the Crick institute. Developed live imaging in fly embryos and worked at elucidating the role of integrins in muscle attachments (JCS, 2018).

  - name: Iris Jarsch
    comments: |
      Moved back to Germany to pursue new career opportunities. Worked on FLS tip complex protein composition and developed the FLS Ace image analysis pipeline (bioRxiv preprint 2019).

  - name: Bishara Marzook
    comments: |
      Now a postdoc in Barry Thompson's Lab at the Crick Institute. Investigated the role of filopodial tip complex proteins during Chlamydia cell invasion.
            
  - name: Ulrich Dobramysl
    cv: |
      **Position**: Herchel Smith Postdoctoral Fellow, joined the lab in October 2015.  
      **Previous positions**: Postdoctoral Researcher at the Mathematical Institute, University of Oxford; PhD in Theoretical Physics at Virginia Tech; Diploma in Engineering Physics at Johannes Kepler University Linz, Austria.
    research: Data-driven modeling of actin dynamics inside filopodia, stochastic modeling of biological processes. [[personal website](http://ulido.github.io)]
    picture: uli-profile.jpg

alumni_phds_ras:
  - name: Daniel Saxton
    comments: |
      former research assistant, now PhD student at University of Berkeley, USA.
      Developed methods for looking at filopodia-like structure elongation (Methods in Cell Biology, 2015)

  - name: Helen Fox
    comments: |
      former PhD student, now a Project Manager at Eurofins.
      Looked at roles of Toca-1 interactions in actin polymerization (CSH protocols, 2019; JBC, 2016)

  - name: Hanae Shimo
    comments: |
      former PhD student, now a PostDoc at the Salk Institute.
      Studied the nanoscale structure of filopodial tip complexes (bioRxiv preprint 2019).

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

<div style="clear: both;"></div>
</div>
{% endfor %}

{% comment %}
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
{% endcomment %}
