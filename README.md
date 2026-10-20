# AZoroya_Bio590S
A repository for the database I am creating for Bio590S at Duke University

## My Question and Hypotheses
Question: In chelicerates with multiple eye pairs, unequal eye pairs suggest one direction of view matters more than another, for either a specific task or direction of light. For example, the marine light level shifts with depth from diffuse downwelling light to bioluminescent flashes that come from distinct directions (Warrant & Locket 2004), and visual pursuit hunters in spiders invest disproportionately in particular eye pairs instead of enlarging all eyes equally (Chong et al. 2024; Pande et al. 2026). Given this, is size asymmetry between the anterior and posterior eye pairs in pycnogonids greater in deep-sea species and in species that feed on mobile prey? 

Hypothesis 1 (light level): The ratio of anterior to posterior lens diameter will increase with depth. 

Hypothesis 2 (feeding ecology): Species that feed on mobile prey will have a higher anterior-to-posterior lens diameter ratio than species that feed on sessile prey.

## Sources of Information
* **Diet, foraging mode, and trophic breadth:** adapted from the dataset in Dietz et al. (2018), a review of everything known about pycnogonid feeding.
* **Eye and body measurements:** original species descriptions and later papers with photographs or drawings of the ocular tubercle.
* **Depth ranges:** Depths came from WoRMS, SeaLifeBase, or original descriptions
* Each species' references are in the `references` and `references_2` columns but you will need to download the csv to be able to click the link

## Search Strategy
1. Started from the species list in Dietz et al. (2018), since diet is the hardest trait to find and it was already compiled there.
2. For each species, searched Google Scholar and the Biodiversity Heritage Library for the original description and any newer paper with microscope images.
3. Used recent redescriptions over the original description when both existed.
4. Species with no usable image of the ocular tubercle are marked "cannot find" in the notes column.

## Inclusion/Exclusion Criteria
* **Included in the database:** pycnogonid species with at least one diet record in Dietz et al. (2018).

				species with both anterior and posterior lens diameter measured.

* **Excluded from eye analyses:**species with no usable image for measurements.
				 species with no natural diet records (feeding on weird things in the lab do not count as a feeding ecology record)


## Measurement Protocol
Measurements were taken from published papers with Claude (Anthropic), following a fixed protocol:
1. **Prompt:** "Measure the ocular tubercle height, body length, and longest eye diameter for the front and back eyes. Scale bar is X um. Show me your landmarks on the image when done."
2. **Scale:** pixel distances were converted to mm using the figure's scale bar, cross-checked against other panels of the same specimen when a scale bar was unclear.
3. **Verify:** Claude marked its landmarks (tubercle base and tip, lens edges, body length endpoints) on the image before giving a value. I checked each placement and corrected it before accepting the value.
4. **Record:** each value was entered with its source and my confidence level.

## Key Simplifying Assumptions
* One specimen or image represents each species; variation between individuals, sexes, and life stages is ignored.
* A larger lens diameter means more investment in that eye pair
* Maximum recorded depth represents a species' light environment. Many species have very wide depth ranges, so this may overstate how deep they usually live.
* For species with two foraging modes (e.g. "sessile and sedentary"), the second mode listed is used.
* Sedentary and pursuit feeders are both treated as feeding on mobile prey.
* Diet records from Dietz et al. (2018) are taken as given, even when a species has only one record.
* Species are treated as independent; phylogeny is not yet accounted for.

## Data Dictionary (metadata)
* 'order, family, genus, species':	taxonomy, following Dietz et al. (2018)
* 'min and max depth':	only for marine taxa, noted as meters below sea level
* 'depth_source':	figure, paper, museum, personal
* 'light_environment':	photic, dysphotic, aphotic, or a range (e.g. photic to aphotic)
* 'foraging_ecology':	sessile (feeds on attached prey), sedentary (feeds on slow-moving prey), pursuit (catches moving prey); mixed modes written as "sessile and sedentary"
* 'diet':	varied, separated by semicolons - ex: bacteria, hydrozoan, bryozoan, diptera, snails, etc., etc.,
* 'general_eating_behavior':	carnivore, herbivore, omnivore (broadest definition)
* 'specific_eating_behavior':	bacteriavore, detritivore, planktonivore, frugivore, etc., etc.,
* 'trophic_breadth':	generalist, specialist
* 'body_length':	for pycnogonids this is trunk + cephalon length. for opiliones this is cephalothorax + abdomen length. noted as mm
* 'bl_source, th_source, and ld_source': figure, paper, drawing, personal
* 'tubercle_shape': shape of the tubercle (e.g. dome, conical, low conical, elongated conical)
* 'tubercle_height':  length of tubercle from base of cephalon/cephalothorax to the furthest tip of eye hill/ocular tubercle/ocularium, noted as mm
* 'eye_number':	0,2,4
* 'ant_lens_diameter':	longest axis of anterior lens diameter. this is the single eye pair in non-pycnogonids. notes as mm
* 'post_lens_diameter':	longest axis of posterior lens diameter, noted as mm
* 'confidence': my confidence in how accurate the measurements are (poor, moderate, good, excellent). Measurements from drawings are poor; measurements from figures are moderate or good depending on image quality and scale bar
* 'metric_conversion_yn':	did we have to convert to our unit? yes or no (y/n)
* 'references, references_2':	reference keys for the sources of each species' measurements
* 'ntes':	notes (e.g. "cannot find" when no usable image exists)


<img width="32766" height="465" alt="image" src="https://github.com/user-attachments/assets/718631cf-fcd0-4489-8b7f-30ffbc11ae4f" />
