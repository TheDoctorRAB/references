# References  
Citations for .bib files for a wide range of topics, loosely classified.  

References repository is set to be a centralized location for all .bib files. Then, where ever tex documents are created, there is no need to import .bib files to multiple directories. Just keep the .bib files in this repository. 

.tex files in this repository are set up to render a list of references for the specific topic.

Add references to .bib files only.

In .bashrc set something like the following -

export BIBREF="$HOME/path/to/references-repository"

export BIBINPUTS="$BIBREF/cybersecurity/cyberattacks:$BIBREF/cybersecurity/nonproliferation:$BIBREF/cybersecurity/cybersecurity:$BIBREF/cybersecurity/general:$BIBREF/government-agencies/doe:$BIBREF/government-agencies/epa:$BIBREF/government-agencies/federal:$BIBREF/government-agencies/nrc:$BIBREF/government-agencies/nsf:$BIBREF/government-agencies/neup:$BIBREF/government-agencies/nwtrb:$BIBREF/nuclear-fuel-cycle/back-end/disposal:$BIBREF/nuclear-fuel-cycle/back-end/nuclear-waste:$BIBREF/nuclear-fuel-cycle/back-end/wipp:$BIBREF/nuclear-fuel-cycle/back-end/yucca-mountain:$BIBREF/nuclear-fuel-cycle/front-end/nuclear-power:$BIBREF/nuclear-fuel-cycle/general:$BIBREF/nuclear-fuel-cycle/storage:$BIBREF/nuclear-fuel-cycle/transport:$BIBREF/people/araujo:$BIBREF/people/borrelli:$BIBREF/people/jenkins-smith:$BIBREF/people/malin:$BIBREF/resilience:$BIBREF/risk/dynamic:$BIBREF/risk/ethics:$BIBREF/risk/general:$BIBREF/risk/perception:$BIBREF/social-science/consent/siting:$BIBREF/social-science/consent/states/utah:$BIBREF/social-science/consent/tribal:$BIBREF/social-science/environmental-justice:$BIBREF/social-science/learning:$BIBREF/social-science/participation-inclusion:$BIBREF/social-science/public-opinion:$BIBREF/social-science/socio-tech-economics:$BIBREF/risk/techniques/delphi:$BIBREF/risk/techniques/fuzzy-logic:$BIBREF/risk/techniques/ahp:$BIBREF/nuclear-fuel-cycle/instrumentation:$BIBREF/social-science/education/rural:$BIBREF/social-science/education/states/idaho:$BIBREF/social-science/education/general:$BIBREF/climate:$BIBREF/people/koerner:$BIBREF/nuclear-fuel-cycle/integrated-energy-systems:$BIBREF/modeling-simulation:$BIBREF/risk/bayes/:$BIBREF/risk/energy-water/:$BIBREF/risk/energy/:$BIBREF/risk/finance/:$BIBREF/risk/food/:$BIBREF/risk/governance/:$BIBREF/risk/water/:$BIBREF/risk/climate/:$BIBREF/risk/drought/:$BIBREF/social-science/workforce/rural:$BIBREF/social-science/workforce/states/idaho:$BIBREF/social-science/workforce/general:$BIBREF/risk/index:"

BIBINPUTS is the path to each .bib file in the repository. Add to BIBINPUTS as new directories are created. 


## Formatting   
The 'bib code' is the first author three letters of the surname + publication year + a,b,c. The letters are for when the XXXNN are the same for multiple resources. 


@article{  
    red22a,  
    author = {Redfoot, Emma K. and Verner, Kelley M. and Borrelli, R. A.},  
    journal = {Progress in Nuclear Energy},  
    pages = {104083},  
    title = {Applying analytic hierarchy process to industrial process design in a nuclear renewable hybrid energy system},  
    volume = {145},  
    year = {2022}  
}  
@article{  
    lee19a,  
    author = {Lee, Jieun and Borrelli, R. A.},  
    title = {{Use of discrete event simulation for material throughput}},  
    journal = {Nuclear Engineering and Design},  
    volume = {345},  
    pages = {183},   
    year = {2019}  
}  
@article{  
    lee19b,  
    author = {Lee, Jieun and Shigrekar, Amey and Borrelli, R. A.},  
    journal = {Nuclear Engineering and Design},  
    pages = {131},  
    title = {Hazard and operability analysis of a pyroprocessing facility},  
    volume = {348},  
    year = {2019}   
}  


Don't use weird @fields; see the bib files and stick to the usual ones. When in doubt use @misc. Do not add URLs or 'date accessed' for web pages. Use @misc with the regular fields and use the date of the web page. Do not use number = {N} for journal articles. See the above examples. Do not use a page range; just put the page number where the resource starts. For no page numbers and just a DOI, only put in the numerical code of the DOI. No 'http://doi.org/10.XXXXXX'. 

@article{  
    ram18a,  
    author = {Ramana, M. V.},  
    title = {Technical and social problems of nuclear waste},  
    journal = {WIREs Energy and Environment},  
    volume = {7},  
    pages = {10.1002/wene.289},  
    year = {2018}  
}

Do not use @techreport because it add 'Tech Rep' and it looks ridiculous. Use @misc and put the report number in the note = {{}}.


@misc{  
    aum21a,  
    author = {Aumeier, Steven E. and Shropshire, David E. and Allen, Todd and Ara{\'u}jo, Kathleen and Bell, Christi and Craig, Michael and Parsons, John and Righetti, Tara},  
    title = {{Emerging Energy Market Analysis Initiative, Methodological Framework}},  
    year = {2021},  
    note = {{INL/EXT-21-65347}}  
}

For an agency as an author - author = {{Department of Energy}}

Input the FULL AUTHOR LIST. Even if there's 27 of them. No exceptions. The journals will use their own bst file to truncate.   

To find if the bib code is duplicated, execute grep -Rnw -e 'bibcode' on the command line.   

