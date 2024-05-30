---
title: "Artificial Larynx"
layout: single-portfolio
excerpt: "<img src='/images/research/artificial-larynx.png' alt=''>"
category: Past Projects
collection: research
order_number: 1
header: 
  og_image: 
---

This project constitutes the research I conducted during my Ph.D, which you can download a copy of the manuscript [here (FR)](/files/pdf/research/Adrien-Mialland-Thesis-FR.pdf){:target="_blank"}, and the defence presentation [here (EN)](/files/pdf/research/Adrien-Mialland-Thesis-Defense-20231106-FR.pptx){:target="_blank"} or [here (FR)](/files/pdf/research/Adrien-Mialland-Thesis-Defense-20231106-FR.pptx){:target="_blank"}.

<iframe src="/files/pdf/research/Adrien-Mialland-Thesis-Defense-20231106-FR.pdf" width="100%" height="500" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>

<br />
# Context

Located in the throat, above the trachea, and sharing a common passage with the esophagus, the larynx is a multifunctional organ primarily involved in phonation, respiration, and swallowing. It contains the vocal cords, is capable of regulating the flow of air entering and exiting the lungs, and offers a complex airway protection mechanism during swallowing, to prevent any misdirection of the food bolus. In cases of advanced cancer, the standard treatment involves the complete removal of the larynx, called a total laryngectomy. Consequently, the functions of the larynx are lost, and then partially and suboptimally restored through surgery by creating a tracheostomy. This involves suturing the trachea to the front of the neck, effectively addressing the loss of the laryngeal airway protection mechanism but also permanently separating the airway from the digestive tract. 

![](/images/research/swallowing-artificial-larynx.png)

After the surgery, the patients no longer breathe through their nose and mouth, resulting in the loss of smell, air warming, filtration, and speech. Therefore, repositioning the trachea to its original position would be a first step towards better restoration of laryngeal functions and improving patients' quality of life. However, this first requires replicating the airway protection mechanism, and in this regard, the first implantation of an artificial larynx in humans took place in 2012. The prosthesis was <u>entirely passive</u>, made of titanium in a tubular shape, and reproduced the airway protection mechanism through a concentric valve mechanism. The patients could breathe and swallow, but only under medical supervision, and food residues were found in the trachea because of imperfect sealing. This partial success opens up new possibilities, and the addition of an <u>active mechanism</u> would allow to forcibly and temporarily close and protect the trachea during swallowing, through the design of an *active implantable artificial larynx*. However, this requires the development of a real-time and implantable swallowing detection system by measuring physiological signals, which has been the subject of my research.

*Also, let us specify that all of this work was carried out in close collaboration with an otorhinolaryngologist surgeon, within the framework of a [clinical research protocol](https://clinicaltrials.gov/study/NCT05452018){: target="_blank"} for validation of our research carried out on humans, and conducted at the Grenoble hospital center in France.*

# Results

The apparent ease of swallowing hides the considerable complexity of the process, involving more than 25 pairs of muscles that contract in a sequential and coordinated manner over the course of a second. Therefore, a precise understanding of the swallowing process was first required. Besides, no research was conducted on an implantable active artificial larynx, which led to my first contribution with a comprehensive survey containing the current knowledge on the swallowing physiology, total laryngectomy consequences, the current swallowing detection methods, and the establishment of four main criteria for the feasibility of such a prosthesis.

> A. Mialland, I. Atallah, and A. Bonvilain - "Toward a robust swallowing detection for an implantable active artificial larynx: a survey." - *Medical & Biological Engineering & Computing*

[Article](https://doi.org/10.1007/s11517-023-02772-8){: .btn--research target="_blank"} [Preprint](/files/pdf/research/swallowing-detection-survey.pdf){: .btn--research target="_blank"}

The main and decisive criteria is the **earliness** of the detection, as no implantable active artificial larynx can be considered safe if the swallowing is detected when the airway is already at risks of food aspiration. Besides, the current detection methods are not meant to be implanted and are essentially developed for the improvement of swallowing assessment tools, for a clinical practice. They also use external sensors that only give access to the superficial anatomical structures, which therefore limit the detection performances. However, an implantable swallowing detection system should not allow for detection errors, to avoid food aspiration. 

To address these limitations, we aimed at the measurement of deep anatomical structures within the neck, on the hypothesis that they would provide more qualitative data in terms of earliness and performances. In that regard, my survey suggests the stylohyoid (SH) and the posterior digastric (PD) neck muscles to be great candidates, but little data were available about them so far. Only indirect measurements via imaging methods were available, because of the difficulty to get precise and direct measurements of each of them independently. So, my following contribution was on the development of a new measurement method to record the *SH and PD muscles activity*. We used two needles containing microsensors that allow to record their electrical activity, which is called intramuscular electromyography (iEMG) measurement. The challenge was to precisely locate each muscle to insert the needles, which was performed by the otorhinolaryngologist surgeon. Then, two other sensors were used for later comparison with the SH and PD muscle activities. First, the sound of swallowing was recorded to extract precise swallowing events and especially define a *temporal detection limit*, after which the airway would be at risk of aspiration. Second, other superficial muscles, called submental muscles, can easily be accessed using surface electromyographic (sEMG) electrodes, placed on the skin. The beginning of their activity has been shown to mark the *beginning of swallowing*. 

> A. Mialland, I. Atallah, and A. Bonvilain - "Stylohyoid and posterior digastric measurement with intramuscular EMG, submental EMG and swallowing sound." - *Bio-Inspired Systems and Signal Processing.*

[Article](https://doi.org/10.5220/0011628100003414){: .btn--research target="_blank"} [Preprint](/files/pdf/research/SH-PD-measurement.pdf){: .btn--research target="_blank"}

However, this approach is actually the results of a primary evaluation of the swallowing process, that used external sensors only to record the beginning of swallowing to the temporal limit. It was meant to get a first estimation of the available timings, as no further analysis would be justify, especially with the use of needles inserted into the neck, if the timings are too short. A relatively comfortable timings of **324 milliseconds** on average was found, which is comparable to the timings available in other health devices application, such as arm prosthesis.

> A. Mialland, B. Kinsiklounon, G. Tian, C. Noûs et A. Bonvilain - "Submental MechanoMyoGraphy (MMG) to Characterize
the Swallowing Signature" - *Innovation and Research in BioMedical engineering*

[Article](https://doi.org/10.1016/j.irbm.2021.05.001){: .btn--research target="_blank"} [Preprint](/files/pdf/research/MMG-evaluation.pdf){: .btn--research target="_blank"}

So, once the needle-based approach was validated by an ethical committee, we recorded the signals on 17 people, that each performed 4 swallowing tasks (liquid, solid, ...) and 13 non-swallowing tasks (head movements, jaw movements, ...), that I later compared with statistical analysis. The results first show that both SH and PD muscles activate at the *beginning of swallowing*, which would give the maximum amount of time up to the temporal limit, to run a detection algorithm and close a protective mechanism of the airway. It also allowed to refine the available time up to the temporal limit, which is now of **427 milliseconds** on average. Second, the SH muscle showed a net predisposition for swallowing, only closely followed by mastication, and the PD muscle had the large majority of its activities located *before the temporal limit*. Therefore, these elements could allow to improve both detection performances and earliness. These statistical analyses were conducted separately and can be found in the following papers.

> A. Mialland, I. Atallah, and A. Bonvilain - "Stylohyoid and posterior digastric timing evaluation" - *Body Sensor Networks*

[Article](https://doi.org/10.1109/BSN58485.2023.10331308){: .btn--research target="_blank"} [Preprint](/files/pdf/research/SH-PD-timings.pdf){: .btn--research target="_blank"}

> A. Mialland, I. Atallah, and A. Bonvilain - "Stylohyoid and posterior digastric recruitment pattern evaluation in swallowing and non-swallowing tasks" - *Innovation and Research in BioMedical engineering*

[Article](https://doi.org/10.1016/j.irbm.2024.100823){: .btn--research target="_blank"} [Preprint](/files/pdf/research/SH-PD-amplitude.pdf){: .btn--research target="_blank"}

The statistical analysis allowed to formally establish the viability of the SH and PD muscles and better understand their behavior. Then, I assessed them within a real time swallowing detection strategy. I used the signals to build machine learning algorithms and evaluate both their detection performances and earliness. The results show that, as suggested by the statistical analyses, the SH muscles allowed for a net improvement in detection performances in comparison the common approaches, and the PD muscles consistently allowed for the earliest detection, before the temporal limit. In addition, the difficulty to differentiate swallowing from each non-swallowing tasks were evaluated and most of them were easy to differentiate. However, the tasks closely related to swallowing, such as mastication or jaw movements, were the hardest to discriminate, which gives important clues on what tasks or family of tasks to focus on for further improvement. This analysis can be found in the following paper.

> A. Mialland, I. Atallah, and A. Bonvilain - "Stylohyoid and posterior digastric potential evaluation for a real-time swallowing detection, with intramuscular EMG" - *IEEE Transactions on Medical Robotics and Bionics*

[Article](https://doi.org/10.1109/TMRB.2023.3336960){: .btn--research target="_blank"} [Preprint](/files/pdf/research/SH-PD-real-time-detection.pdf){: .btn--research target="_blank"}


So far, these results show that an implantable swallowing detection system, meant to be part of an implantable active artificial larynx, is a viable perspective in terms of the capabilities that the anatomy provides for a detection. I showed that carefully chosen anatomical structure can provide qualitative and improved signals in terms of earliness and performances of detection. So, further improvement should seek to incorporate more varied types of data to get a clear view of the neck activity as a whole, and not just swallowing. Also, different type of sensor would give access to different types of neck activity. For instance, new sensors are being developed by researchers, that are able to record sensory inputs directly on the nerve. Coupled with the measurement of the SH and PD muscles, it could provide a finer grained view of swallowing, by the association the sensory inputs with the motor outputs generated in the muscles.

One final aspect though, is the time it would take for an implantable active artificial larynx to actuate a swallowing detection and airway protective systems. Indeed, whatever the ability of the anatomy to provide qualitative data, the system itself should be able to temporarily close the airway as fast as possible. So, to formally and practically establish the viability of an implantable active artificial, the following paper constitute the last contribution of my thesis and gathers what I discussed so far to develop a laboratory prototype, as a proof of concept of such a prosthesis. I first established the requirements and the basis of it and its practical implementation was then conducted by engineering students in electronics and mechanics, that I supervised within internships. So, given that it constitutes a specific sub project within my thesis, the detailed can be found in the [Laboratory Prototype](/research/laboratory-prototype){: target="_blank"} page I dedicated to it. In short, it reproduces the requirement of an implanted system by, first, implementing real time detection algorithms on microcontrollers and, second, developing a protective mechanism that reproduces the mechanism of the larynx. The full prototype could be actuated in less than 30 miliseconds, from the moment it starts to process incoming data, to the full closure of the protective mechanism, **which easily fits within the timings** defined by the SH and PD muscle activities, with regard to the temporal limit.

> A. Mialland, E. Bouchet, A. Diallo, and A. Bonvilain - "Implantable active artificial larynx: timing evaluation of a laboratory prototype" - *IEEE International Conference on Advanced Robotics and Mechatronics*

[Article](http://www.ieee-arm.org/){: .btn--research target="_blank"} [Preprint](/files/pdf/research/artificial_larynx_prototype.pdf){: .btn--research target="_blank"}








