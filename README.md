# references
Citations for .bib files for a wide range of topics, loosely classified.  

References repository is set to be a centralized location for all .bib files. Then, where ever tex documents are created, there is no need to import .bib files to multiple directories. Just keep the .bib files in this repository. 

.tex files in this repository are set up to render a list of references for the specific topic.

Add references to .bib files only.

In .bashrc set something like the following -


export BIBREF="$HOME/path/to/references-repository"

export BIBINPUTS="$BIBREF/cybersecurity/cyberattacks:$BIBREF/cybersecurity/nonproliferation:$BIBREF/cybersecurity/cybersecurity:$BIBREF/cybersecurity/general:$BIBREF/government-agencies/doe:$BIBREF/government-agencies/epa:$BIBREF/government-agencies/federal:$BIBREF/government-agencies/nrc:$BIBREF/government-agencies/nsf:$BIBREF/government-agencies/nwtrb:$BIBREF/nuclear-fuel-cycle/back-end/disposal:$BIBREF/nuclear-fuel-cycle/back-end/nuclear-waste:$BIBREF/nuclear-fuel-cycle/back-end/wipp:$BIBREF/nuclear-fuel-cycle/back-end/yucca-mountain:$BIBREF/nuclear-fuel-cycle/front-end/nuclear-power:$BIBREF/nuclear-fuel-cycle/general:$BIBREF/nuclear-fuel-cycle/storage:$BIBREF/nuclear-fuel-cycle/transport:$BIBREF/people/araujo:$BIBREF/people/borrelli:$BIBREF/people/jenkins-smith:$BIBREF/people/malin:$BIBREF/resilience:$BIBREF/risk/dynamic:$BIBREF/risk/ethics:$BIBREF/risk/general:$BIBREF/risk/perception:$BIBREF/social-science/consent/siting:$BIBREF/social-science/consent/states/utah:$BIBREF/social-science/consent/tribal:$BIBREF/social-science/environmental-justice:$BIBREF/social-science/learning:$BIBREF/social-science/participation-inclusion:$BIBREF/social-science/public-opinion:$BIBREF/social-science/socio-tech-economics:$BIBREF/risk/techniques/delphi:$BIBREF/risk/techniques/fuzzy-logic:$BIBREF/risk/techniques/ahp:"

BIBINPUTS is the path to each .bib file in the repository. Add to BIBINPUTS as new directories are created. 
