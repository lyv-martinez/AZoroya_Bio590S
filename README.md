# AZoroya_Bio590S
A repository for the database I will be creating for Bio590S at Duke University

## My Question and Hypotheses
Question: In chelicerates with multiple eye pairs, unequal eye pairs suggest one direction of view matters more than another, for either a specific task or direction of light. For example, the marine light level shifts with depth from diffuse downwelling light to bioluminescent flashes that come from distinct directions (Warrant & Locket 2004), and visual pursuit hunters in spiders invest disproportionately in particular eye pairs instead of enlarging all eyes equally (Chong et al. 2024; Pande et al. 2026). Given this, is size asymmetry between the anterior and posterior eye pairs in pycnogonids greater in deep-sea species and in species that feed on mobile prey? 

Hypothesis 1 (light level): The ratio of anterior to posterior lens diameter will increase with depth. 

Hypothesis 2 (feeding ecology): Species that feed on mobile prey will have a higher anterior-to-posterior lens diameter ratio than species that feed on sessile prey.
## Data Dictionary (metadata)
* 'depth':	only for marine taxa, noted as meters below sea level
* 'depth_source':	figure, paper, museum, personal
* 'light_environment':	photopic, scotopic
* 'foraging_ecology':	pursuit, sessile
* 'diet':	varied, separated by commas - ex: bacteria, hydrozoan, bryozoan, diptera, snails, etc., etc.,
* 'general_eating_behavior':	carnivore, herbivore, omnivore (broadest definition)
* 'specific_eating_behavior':	bacteriavore, detritivore, planktonivore, frugivore, etc., etc.,
* 'trophic_breadth':	generalist, specialist
* 'body_length':	for pycnogonids this is trunk + cephalon length. for opiliones this is cephalothorax + abdomen length. noted as mm
* 'bl_source, th_source, and ld_source': figure, paper, personal
* 'tubercle_height':	length of tubercle from base of cephalon/cephalothorax to the furthest tip of eye hill/ocular tubercle/ocularium, noted as mm
* 'eye_number':	0,2,4
* 'ant_lens_diameter':	longest axis of anterior lens diameter. this is the single eye pair in non-pycnogonids. notes as mm
* 'post_lens_diameter':	longest axis of posterior lens diameter, noted as mm
* 'metric_conversion_yn':	did we have to convert to our unit? yes or no (y/n)
	
<img width="32766" height="465" alt="image" src="https://github.com/user-attachments/assets/718631cf-fcd0-4489-8b7f-30ffbc11ae4f" />
