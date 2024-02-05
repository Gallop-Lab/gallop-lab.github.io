---
layout: page
title:  "People"
people:

  - name: Jenny Gallop
    cv: |
      **2020 - present**: Associate Professor, Department of Biochemistry, University of Cambridge  
      **2011 - present**: Group Leader, Gurdon Institute, University of Cambridge  
      **2011 - 2020**: Affiliated Research Fellow, Department of Biochemistry  
      **2006 - 2011**: Postdoc and EMBO Fellow in laboratory of Marc Kirschner, Harvard Medical School, Boston, USA  
      **2001 - 2006**: PhD and short postdoc in Harvey McMahon's lab, MRC Laboratory of Molecular Biology, Cambridge, UK  
      **1997 - 2001**: Masters degree in Biochemistry, Trinity College, University of Oxford, UK  
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
    research: Examining how actin polymerisation is responsive to phosphoinositides and membrane curvature 
    picture: Jonathan-profile2.jpg
    
  - name: Thomas Blake
    cv: |
      **Position**: Wellcome Trust Research Associate, joined the lab in January 2021  
      **Previous positions**: BA Natural Sciences and MSci Biochemistry, University of Cambridge; MRes and PhD Imperial College, London, and short postdoc in Jake Baum's lab studying myosin motors in malaria parasites
    research: Superresolution and rapid timelapse microscopy in studying filopodial initiation and extension
    picture: Tom_portrait.jpg

  - name: Mary-Pia Jeyarajasingham
    cv: |
      **Position**: AstraZeneca PhD Student, joined the lab in October 2022  
      **Previous positions**: MSci in Biomedical Sciences at St Georges, University of London
    research: Using phage display antibody technology to find new filopodial proteins
    picture: Pia.png
    
  - name: Pankti Vaishnav
    cv: |
      **Position**: Wellcome Trust Research Assistant/PhD student, joined the lab in July 2020  
      **Previous positions**: BSc in Biochemistry, University of Birmingham and MRes in Molecular and Cellular Biosciences, Imperial College, London
    research: Molecular mechanisms of SNX9-mediated actin polymerisation
    picture: Pankti-tn2.jpg  

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
