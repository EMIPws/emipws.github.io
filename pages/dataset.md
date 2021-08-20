---
layout: single
permalink: /dataset/
header:
title: "Distributed Collection of Eye Movement Data in Programming - Dataset"
sidebar:
  nav: "main"
---

The EMIP dataset contains eye movement data during program comprehension.

The dataset consists of:

1. date.txt – file specifying when the dataset was uploaded
2. emip_metadata.csv – file with participants’ background information, order in which the stimulus programs were shown, and information about the comprehension questions
3. rawdata – folder with raw eye movement data
4. stimuli – folder with screenshots of the experiment slides and AOI coordinates for the stimulus programs. For more details on stimulus see [stimulus material](/stimulus-material/).

[Link to the dataset](http://emipws.org/wp-content/uploads/emip_dataset.zip)

**Apparatus:**

The stimuli were presented to participants using a laptop PC. The screen resolution was 1920×1080 px. The data was recorded with an *SMI RED250* mobile eye tracker (sampling rate 250 Hz). The experiment was built with SMI Experimental Suite Scientific Premium.

**Participants:**

The experiment involved 269 participants, of which 15 had to be excluded due to different reasons (e.g. terminating the experiment prematurely). All subjects filled a questionnaire with the following items:

- Age
- Gender (female | male | other)
- Mother tongue
- English level (none | low | medium | high)
- Overall programming expertise (none | low | medium | high)
- Expertise in Java / Python / Scala (none | low | medium | high)
- How long they have been programming (years)
- How long they have been programming in Java / Python / Scala (years)
- How often they use any programming language other than Java / Python / Scala
  (not at all | less than 1 hour / month | less than 1 hour / week | less than 1 hour / day | more than 1 hour / day)
- How often they program in Java / Python / Scala
  (not at all | less than 1 hour / month | less than 1 hour / week | less than 1 hour / day | more than 1 hour / day)
- Which other programming languages they know (Language – Level of expertise: low | medium | high)
- Whether they are wearing glasses or contact lenses (no | glasses | contact lenses)
- Whether they are wearing mascara or other eye-makeup (yes | no)
The answers are compiled in emip_metadata.csv.

**Dataset**

For each participant, the dataset contains a tsv-file with raw eye movement data. The file header provides information like version of the IDF Converter used, number of samples, and coordinates of the calibration points. All header lines start with “#”.

The data columns are separated by  a tab, they include among others:

- Time: timestamp of the sample
- Type: Sample (SMP) | Message (MSG)
- L Raw X [px]: horizontal pupil position – left eye
- L Raw Y [px]: vertical pupil position – left eye
- R Raw X [px]: horizontal pupil position – right eye
- R Raw Y [px]: vertical pupil position – right eye
- L Dia X [px]: pupil diameter on the X axis in pixels – left eye
- L Dia Y [px]: pupil diameter on the Y axis in pixels – left eye
- L Pupil Diameter [mm]: pupil diameter in mm – left eye
- R Dia X [px]: pupil diameter X axis in pixels – right eye
- R Dia Y [px]: pupil diameter Y axis in pixels – right eye
- R Pupil Diameter [mm]: pupil diameter in mm – right eye
- L CR1 X [px]: horizontal corneal reflex position. One or two CRs can be present – left eye
- L CR1 Y [px]: vertical corneal reflex position. One or two CRs can be present – left eye
- L CR2 X [px]: left eye horizontal corneal reflex position. One or two CRs can be present
- L CR2 Y [px]: left eye vertical corneal reflex position. One or two CRs can be present
- R CR1 X [px]: horizontal corneal reflex position. One or two CRs can be present – right eye
- R CR1 Y [px]: vertical corneal reflex position. One or two CRs can be present – right eye
- R CR2 X [px] : horizontal corneal reflex position. One or two CRs can be present – right eye
- R CR2 Y [px] : vertical corneal reflex position. One or two CRs can be present – right eye
- L POR X [px]: point-of regard in the X axis in pixels – left eye
- L POR Y [px]: point-of regard in the Y axis in pixels – left eye
- R POR X [px]: point-of regard in the X axis in pixels – right eye
- R POR Y [px]: point-of regard in the Y axis in pixels – right eye
- Timing: Quality values
- L Validity: validity – left eye
- R Validity: validity – right eye
- Pupil Confidence
- L Plane: plane number – left eye
- R Plane: plane number – right eye
- L EPOS X: left pupil position from the perspective of the subjective camera, in the X axis in pixels
- L EPOS Y: left pupil position from the perspective of the subjective camera, in the Y axis in pixels
- L EPOS Z: left pupil position from the perspective of the subjective camera, in the Z axis in pixels
- R EPOS X: right pupil position from the perspective of the subjective camera, in the X axis in pixels
- R EPOS Y: right pupil position from the perspective of the subjective camera, in the Y axis in pixels
- R EPOS Z: right pupil position from the perspective of the subjective camera, in the Z axis in pixels
- L GVEC X: left eye gaze vector, from the perspective of the left eye camera, X axis component
- L GVEC Y: left eye gaze vector, from the perspective of the left eye camera, Y axis component
- L GVEC Z: left eye gaze vector, from the perspective of the left eye camera, Z axis component
- R GVEC X: right eye gaze vector, from the perspective of the left eye camera, X axis component
- R GVEC Y: right eye gaze vector, from the perspective of the left eye camera, Y axis component
- R GVEC Z: right eye gaze vector, from the perspective of the left eye camera, Z axis component

Each trial includes messages naming the stimulus screenshot, which can be found in the stimuli-folder, and giving the coordinates of mouse clicks.

All data is anonymous. 15% of the data is not published.

The EMIP Distributed Dataset can be used under the CC 4.0 license ([https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/))

When using the dataset, refer to: Bednarik, R., Busjahn, T., Gibaldi, A., Ahadi, A., Bielikova, M., Crosby, M., … & van der Linde, I. (2020). EMIP: The eye movements in programming dataset. *Science of Computer Programming*, 198, 102520. [https://doi.org/10.1016/j.scico.2020.102520](https://doi.org/10.1016/j.scico.2020.102520)