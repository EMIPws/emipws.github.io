---
layout: single
permalink: /workshop/emip-2022-program/
header:
title: "EMIP 2022 Workshop - Program"
sidebar:
  nav: "emip-2022"
---

The Tenth International Workshop on Eye Movements in Programming 2022 will be held on **May 18, 2022 virtually**. It is co-located with the [44th International Conference on Software Engineering (ICSE 2022)](https://conf.researchr.org/home/icse-2022/).

**EMIP 2022 Schedule (May 18 2022):**

| Central Time | Eastern Time | Pacific Time | UTC | Event | Duration |
| --- | --- | --- | --- | --- | --- |
| 10:00AM | 11:00AM | 8:00AM | 3:00PM | Welcome from Organizers | 5 minutes |
| 10:05AM | 11:05AM | 8:05AM | 3:05PM | **[Keynote by Felienne Hermans](https://www.felienne.com/)**<br />[Hedy: Creating a Graduate Programming Language](#hedy-creating-a-gradual-programming-language) | 45 mins + 15 Q/A|
| 11:05AM | 12:05PM | 9:05AM | 4:05PM | Mingle and Introduction Breakout Sessions (optional) | 10 minutes |
| 11:15AM | 12:15PM | 9:15AM | 4:15PM | Paper Presentations | 45 minutes |
| | | | | Raymond Lister: *Some Thoughts on Designing Eye Movement Studies for Novice Programmers* | 10 mins + 5 Q/A |
| | | | | Tanya Beelders: *Eye-tracking analysis of source code reading on a line-by-line basis* | 10 mins + 5 Q/A |
| | | | | Krzysztof Krejtz, Andrew T. Duchowski, Katarzyna Wisiecka, Izabela Krejtz: *Entropy of Eye Movements While Reading Code or Text* | 10 mins + 5 Q/A |
| Noon | 1:00PM | 10:00AM | 5:00PM | Break and Small Group Breakout Discussion (optional) | 15 minutes
| 12:15PM | 1:15PM | 10:15AM | 5:15PM | **Panel discussion:** [Practical Implications of EMIP Research on Software Engineering and CS Education](#panel-practical-implications-of-emip-research-on-software-engineering-and-cs-education)<br /><br />Andrew Begel - Microsoft Research, USA<br />Ian McChesney - Ulster University, Northern Ireland<br />Janet Siegmund - Technical University of Chemnitz, Germany<br />Martha Crosby - University of Hawaiʻi, USA<br />Norman Peitek - Saarland University, Germany<br />Roman Bednarik - University of Eastern Finland, Finland<br />Sarah Fakhoury - Washington State University, USA | 45 mins + 15 Q/A |
| 1:15PM | 2:15PM | 11:15AM | 6:15PM | Closing | 5 minutes |

  
  
# Hedy: Creating a gradual programming language
**Felienne Hermans**  

Hedy is a gradual programming language to make learning programming easier. The core idea of Hedy is that it uses different language levels. In level 1, there is hardly any syntax at all, for example printing is done with:

print hello EMIP!

In every level, new syntax and concepts are added, until kids are doing a subset of Python in level 20 with conditions, loops, variables and lists. The leveled approach means that learners do not have to learn all syntax rules at once. Hedy is aimed at children that want to get started with textual programming languages, but for whom starting with Python might still be too complex.

Hedy is open source, runs in the browser, is free to use, and available in 22 different languages (Including English, Spanish, Arabic and Hindi). Hedy was launched in early 2020 and since then almost 2 million Hedy programs have been created by children worldwide. Try Hedy at www.hedycode.com.

In this talk, Felienne will dive into the pedagogy behind Hedy, but also expand on the technical aspects of Hedy. For example, a set of increasingly complex grammars, rather than one grammar, poses new challenges for language design.


# Panel: Practical Implications of EMIP Research on Software Engineering and CS Education

**Andrew Begel:**  
Eye tracking technologies offer lots of promise to enhance both computing education and practice. As the study of eye movements in programming progresses, we should consider studies in basic science to support the theoretical foundation of our work and applications to have impact on software engineers. We all use fixation algorithms derived from studies of people reading natural language text. However, code is not text --- reading code induces different eye gaze patterns than reading text. We need to develop algorithms to accurately classify fixations in gaze paths when reading source code in text and block forms. On the application end, we have begun to make progress in identifying program comprehension and task-specific eye gaze patterns. If we leverage this understanding in live user interface visualizations, we could guide novice as well as expert software developers to complete their tasks more efficiently. 

**Janet Siegmund:**  
Eye tracking has proved successful to shed more details on how programmers work with source code. Now it is time to use the potential of eye tracking to improve programming education. Despite many years of research, the failure rates in introductory programming courses are still rather high. Eye tracking would allow us to observe novice programmers from a new angle. Do they read algorithms different than programming experts? What would that tell us? And can we nudge novice programmers to look at source code the way programming experts do? Eye tracking can help us answer these and similar questions, which may be one missing link to move programming education forward. 

**Martha Crosby:**  
Physiological sensors could be used by teachers to view students’ cognitive load in real time allowing the teacher to enhance or adjust their presentation to optimize the student-computer interaction. This ability could be particularly helpful for distance educational multimedia presentations. Research in the Hawaii Interdisciplinary Neurobehavioral and Technology (HINT) Laboratory in the Department of Information and Computer Sciences (ICS) at the University of Hawai'i at Mānoa (UHM) target extracting real-time cognitive load from physiological sensors to collect: eye fixation times, number of fixations, eye saccades, blink rates, pupil dilation, hand/finger pressures on a mouse, relative blood flow, pulse, temperature, general somatic activity and electrodermal activity change. The goal is to obtain a reliable suite of cognitive load indicators which use passive physiological sensors. The development of real-time cognitive load indicators involves different types of cognitive activities, establishing the transform from sensor to cognitive load and controlling the cognitive impact of various multimedia features.


**Norman Peitek:**  
Eye tracking has shown its merits for a wide range of research and practical applications in software engineering, because it enables researchers to observe visual attention in high detail. However, it is limited regarding obtaining insights into the underlying cognitive processes. Recently, neuroimaging methods, such as functional magnetic resonance imaging (fMRI) or electroencephalography (EEG), have emerged as a suitable method to comprehensively study programmers’ cognition. However, neuroimaging may suffer from lower temporal resolution and limited insights into programmers’ strategies. Thus, a combination of eye tracking, with its high temporal view of visual attention, and neuroimaging, with its profound perspective into programmers’ cognition, will be a powerful method for researchers in the future. 

