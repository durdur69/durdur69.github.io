---
id: 132
title: Using Neuroimaging to Predict Recidivism and Identify Psychopaths
subtitle: A review of early empirical applications and their evidentiary use.
date: 2017-12-27T03:48:15-05:00
layout: default
permalink: /psychopathy/
keywords: fmri, neurolaw, neuroscience, psychiatry, psychopathy
---

<span style="font-size: 1rem;">The intersection of cognitive neuroscience and the law—called </span><em style="font-size: 1rem;">neurolaw</em><span style="font-size: 1rem;">—is a rapidly growing field of research. Many are excited by the potential of neuroscience to improve everything from criminal sentencing to rehabilitation of criminals (Jones et al., 2013). In this paper I will focus on the application of neuroimaging to psychopathy, and specifically on how it can be used to predict future recidivism—aptly named </span><em style="font-size: 1rem;">neuroprediction</em><span style="font-size: 1rem;">—and identify psychopaths. </span>

<span style="font-size: 1rem;">Psychopaths make up less than 1% of the U.S. population, yet commit 30% of all violent crime, costing us $250-400 billion dollars per year (Kiehl, 2010). Thus, if neuroimaging can improve our ability to diagnose psychopathy and predict recidivism, it will be quite the boon to society. However, as with other promising technologies, there are many methodological and ethical issues that arise from our growing neuropredictive powers. My thesis is that if we exercise sufficient caution and thoroughly vet these neuroprediction tools, then we ought to use them in our criminal justice system, for they are only going to give us better, more accurate information and improve upon our current forms of risk assessment. The real ethical issue is how we use this predictive information, but this issue isn’t unique to neuroimaging: it’s an issue all forms of predictive evidence face.</span>

In _Psychopathy Explained_, I will define psychopathy, explain how we measure it, and explain clinical and actuarial violence risk assessment. In _Neuroprediction Examples_, I will provide two examples in which neuroimaging is applied to psychopathy and one where it is applied to predicting recidivism is general. In _Methodological and Scientific Concerns_, I will discuss issues general to all three examples and to the practice of treating people differently on the basis of brain scans. Finally, in _Applications and Ethical Concerns_, I will discuss potential applications of neuroprediction and address the unique ethical issues they might give rise to.

<u>Psychopathy Explained</u>

Psychopathy is a psychiatric disorder composed of multiple traits. The Hare Psychopathy Checklist-Revised (PCL-R), a twenty item diagnostic exam, is currently the standard for measuring these traits and identifying psychopaths (Kiehl, 2010). Items in the PCL-R measure two factors of psychopathy. Factor 1 items measure traits related to “emotional and interpersonal relationships, such as superficial charm, egocentricity, grandiosity, deceitfulness and manipulativeness, and absence of remorse, guilt, or empathy”; Factor 2 items measure traits such as “impulsivity, poor behavioral controls, proneness to boredom, poor life planning, and irresponsibility” (Kiehl, 2010, 48). Thus, psychopathy is a complex disorder with distinct factors that can be measured via the PCL-R. However, because it is based on self-report, the PCL-R is not a perfect metric. For example, one of the Factor 1 items of the PCL-R measures pathological lying; one can imagine how difficult it would be to measure this trait via self-report (Hulbert, 2015).

The PCL-R is one part of a much broader violence risk assessment that is important to the legal process. Risk assessment factors into everything from sentencing to rehabilitation of criminals. An important distinction to note is that of “clinical assessment” vs. “actuarial assessment” of violence risk (Nadelhoffer, 2012a). Clinical assessment is based on a mental health professional’s interaction with a patient and what they believe the patient’s future behavior will be like. However, this type of assessment is prone to the biases of the mental health practitioner, and some claim that psychologists and psychiatrists’ predictions are no better than “flipping coins in the courtroom” (Nadelhoffer, 2012a; Ennis & Litwack, 1974). Conversely, actuarial assessment is a probabilistic approach to violence risk, which takes into account a host of factors such as age, gender, impulsivity, family and work history, history of violence, social networks and mental disorders (Nadelhoffer, 2012a, 77). The PCL-R often factors into these actuarial violence risk assessments. However, the PCL-R is not as robust as desired, so perhaps neuroimaging can improve our risk assessment models (81).

<u>Neuroprediction Examples</u>

_Machine learning_

Steele et al. trained machine learning algorithms to differentiate between psychopathic and non-psychopathic adolescents using structural MRI and other measures such as IQ and age. Psychopaths tend to exhibit “structural and cognitive deficits originating in paralimbic areas,” and therefore Steele et al. chose thirteen of these areas as their a priori regions of interest and measured grey matter volume in density in these ROIs (2). Their subject pool was composed of 71 “incarcerated youth with elevated psychopathic traits,” 72 “incarcerated youth with low-psychopathic traits,” and 21 “non-incarcerated youth as healthy controls” (1). These categorizations were based on the results of the PCL: YV, a youth version of the PCL-R (2).

Their machine learning algorithm based on grey matter density was able to differentiate between high-psychopathic individuals and healthy controls with an overall accuracy of 82.61%. However, their classifier which used only age and IQ was actually able to better differentiate between these individuals, with an overall accuracy of 83.10% (5). When the classifiers were used to differentiate between low-psychopathic individuals and healthy controls, a similar trend emerged, with the age and IQ-based classifier doing slightly better.

_rsfMRI_

Philippi et al. examined the resting state functional connectivity of 142 prison inmates, 46 of whom were psychopathic. They wanted to see how the functional connectivity of the default mode, frontoparietal, and cingulo-opercular networks (abbreviated DMN, FPN, and CON, respectively) related to PCL-R scores, and more specifically, scores on each factor of the PCL-R (6070). In their within-group analysis of psychopaths, they found that “higher PCL-R scores were associated significantly diminished connectivity between the right (R) IPS [intraparietal sulcus] and the bilateral dACC of the CON and the right precuneus of the FPN” (6071). Their between-group analysis resulted in similar findings, with only seed regions in the FPN showing significant differences in functional connectivity between the two groups. They conclude that “diminished parietal–dACC connectivity is a robust neurobiological correlate of psychopathy” (6075).

Interestingly, Philippi et al. actually found a dissociation in functional connectivity of the different factors of psychopathy. For example, “higher Factor 1 scores”—which measures interpersonal/affective traits— “were associated with significantly decreased connectivity between the medial and lateral regions of the DMN,” whereas “higher Factor 2 scores were associated with significantly increased functional connectivity between the medial prefrontal and parietal regions of the DMN” (6071). This apparent dissociation between the two factors of psychopathy is unintuitive and suggests that psychiatric disorders such as psychopathy aren’t as simple as we might make them out to be. Therefore, we ought to consider specific biomarkers for Factor 1 and Factor 2 of psychopathy when doing our risk assessment and designing our rehabilitation programs.

_Task-based fMRI_

Aharoni et al. did a longitudinal study looking at how anterior cingulate cortex (ACC) activity during the performance of an impulse control task correlated with recidivism. Their subject pool was composed of 96 adult offenders—those who had committed crimes in the past; however, only some, not all, of the participants were psychopaths. The task they performed was the go/no-go (GNG) task, which requires one to control their impulses. They chose this task because impulsivity is an important risk factor for recidivism (6223). They focused on ACC activity because this region of the brain has been associated with “error processing, conflict monitoring, response selection, and avoidance-learning,” so it would seem logical that its activity would correlate with performance on the GNG task (6223). Aharoni et al. found that lowered ACC activity on this task was indeed associated with increased probability of rearrest (6224). Interestingly enough, PCL-R Factor 2 score and the prison release age showed similar predictive power, though only for non-violent crimes (6224).

<u>Methodological and Scientific Concerns</u>

These three examples all provide interesting proofs of concept for how neuroimaging can be applied to identifying psychopaths and predicting recidivism. However, there are many issues with these examples. I will address the technical issues of each study in turn, and then address more general scientific issues with these types of studies.

In the machine learning study, the first thing to note is that the classifier based on grey matter density and volume was slightly _worse_ at discriminating between psychopathic and healthy individuals than the classifier based simply on age and IQ. This shows us how rudimentary our analysis techniques currently are. In the rsfMRI study, we must remember that functional connectivity doesn’t mean two brain regions are functionally connected; it simply means that there’s a correlation in the BOLD signal of the two areas, so we ought to be cautious in our interpretation of this study. Finally, in the ACC activity study, only 9 of the 96 participants later recidivated and were arrested, and therefore we can’t draw huge conclusions from this study because of the problem of false positives (Aharoni, 6224). Furthermore, just because ACC activity on the GNG task seemed to correlate with recidivism, this doesn’t necessarily mean it is causing recidivism, and we ought to keep this in mind when trying to intervene and rehabilitate criminals.

There are a couple issues common to all these studies. All of them were done with prison populations (and in the machine learning case, with incarcerated adolescents). Therefore, we can’t necessarily extend the findings to the general population. This relates to the problem of within-group analyses: just because we see certain levels of brain activity correlate with psychopathy or increased recidivism within a prison population, this doesn’t mean the same will be true for the general population. That said, the machine learning and rsfMRI studies actually did between group analyses, so this strengthens their findings.

Another concern with all these studies is how they categorize psychopathy. As mentioned before, psychopathy is a disorder composed of many traits, and treating it as one singular disorder is problematic. In the rsfMRI study, even among psychopaths there was a dissociation between Factor 1 and Factor 2 traits of psychopathy and their neural correlates. Therefore, future research ought to be aware that the etiology of each factor can vary, and this will affect how we try to treat different types of psychopathy.

A final concern relating to the actual application of this neuroimaging is the risk of false positives and the problem of extending these findings to individuals. Even if we do find some sort of correlation between ACC activity and recidivism in the ACC study, this doesn’t necessarily mean that a single individual with lower ACC activity on the GNG task is more likely to recidivate. Furthermore, in the case of identifying psychopaths, the potential for false positives—that is, identifying someone as a psychopath when they aren’t one—is high, even if the technique has a high overall accuracy. Therefore, we must be cautious in applying these techniques. That said, I see nothing wrong with applying neuroprediction to individuals if we have low p-values, do between-group comparisons, and replicate our results. Current actuarial risk assessment models take into account a host of probabilistic factors that are out of our control, so I don’t see what’s wrong with using neuroimaging in the same way if the technique is thoroughly vetted. In fact, I believe that while not there yet, these neuroimaging techniques will soon have greater construct validity than other measures we currently use in our violence risk assessment.

<u>Ethical Concerns </u>

The one ethical concern unique to neuroimages is that they might bias us, specifically in a legal setting where stakes are high. For example, Weisberg et al. (2008) showed that adding irrelevant neuroscientific information to a bad explanation made lay people find the explanation to be satisfying and logically sound. Furthermore, McCabe and Castel (2008) showed that explanations accompanied by neuroimages were judged as more credible than those not accompanied by neuroimages, suggesting that neuroimages have a special ability to cloud our judgement. One might think that given this biasing effect of neuroimages, we ought not use them in a legal setting. However, Schweitzer et al. (2013) had a significantly larger and more diverse subject pool (over 1000 participants vs. around 150 participants) and were unable to replicate McCabe and Castel’s findings (508). A recent review article by Roskies et al. (2013) also supports this claim, saying that “neuroimages have no special impact on juror decision-making beyond the neuroscientific testimony” (100). That is, the neuroimages themselves are no more biasing than the verbal testimony of a neuroscientist, which is an admissible form of evidence in court (Sinnott-Armstrong et al., 2008).

<u>Applications and Conclusion</u>

Other than the potential biasing effect of neuroimages, which seems to have been handled, with regards to predicting recidivism and diagnosing psychopathy, neuroimages don’t seem to bring any unique ethical concerns to the table. Nadelhoffer et al. (2012b) and others have argued that the real issue with neuroprediction is “the increased power of prediction, not the fact that neural information is being used to make the prediction” (636). Neuroimaging is simply refining our focus, allowing us to see more. We may not like what we see and may not want to act on that information, but we at least ought to know what is actually there.

Imagine that we had a perfect predictive tool that could tell you the probability of a criminal recidivating and within what time period. How would we use this information? Would we even want to know this information? The information itself isn’t bad; it simply has the potential to be applied in bad ways. That said, I’d argue that we’re ethically obligated to use this predictive information in our sentencing, for if we know that someone is likely to recidivate, we ought not to let them back into society until they have been treated and rehabilitated (which neuroimaging can help with). This makes sense within a restorative or consequentialist criminal justice framework—one which cares about rehabilitating criminals and maximizing collective well-being—but doesn’t make much sense in a retributive criminal justice framework—one which cares only about punishing wrongdoers (Greene & Cohen, 2004).

However, this consequentialist logic can lead us to some dark places. For example, in capital sentencing, if two people committed the same crime and we find out from the neuroimaging data that one is more likely to recidivate, ought we kill this person but keep the other on death row? Irrespective of one’s opinion about the death penalty, it makes sense to spend the resources on the person who is less likely to recidivate, for if they are eventually found innocent then they will cause less harm to society. However, one could imagine a case in which the person who is executed was actually innocent, yet we never found out because we executed them so soon.

All that said, these ethical issues are not unique to neuroimaging; they are issues we face with any sort of predictive evidence within a utilitarian framework. With the advent of new types of analyses and neuroimaging such as MVPA and rsfMRI, our neuropredictive powers are quickly improving, and if we scrutinize them thoroughly then I think they ought to be a part of our actuarial risk assessment models, which should factor into our criminal sentencing and rehabilitation processes.

<u>Citations:</u>

Aharoni, Eyal, Gina M. Vincent, Carla L. Harenski, Vince D. Calhoun, Walter Sinnott-Armstrong, Michael S. Gazzaniga, and Kent A. Kiehl. 2013. “Neuroprediction of Future Rearrest.” _Proceedings of the National Academy of Sciences_ 110(15): 6223-6228.

Ennis, Bruce J., and Thomas R. Litwack. 1974. “Psychiatry and the Presumption of Expertise: Flipping Coins in the Courtroom.” _California Law Review_ 62(3): 693-752.

Greene, Joshua, and Jonathan Cohen. 2004. “For the Law, Neuroscience Changes Nothing and Everything.” _Philisophical Transactions of the Royal Society of London B_ 359: 1775-1785.

Hulbert, Sarah, and Hojjat Adeli. 2015. “Spotting Psychopaths Using Technology.” _Review of Neuroscience_ 26(6): 721-732.

Jones, Owen D., René Marois, Martha J. Farah, and Henry T. Greely. 2013. “Law and Neuroscience.” _Journal of Neuroscience_ 33(45): 17624-17630.

Kiehl, Kent. 2010. “Can Neuroscience Identify Pscyhopaths?” _A Judge’s Guide to Neuroscience: A Concise Introduction_, ed. Michael Gazzaniga. Law and Neuroscience Project: Nashville, TN.

Koenigs, Michael, Arielle Baskin-Sommers, Joshua D. Zeier, and Joseph P. Newman. 2010. “Investigating the Neural Correlates of Psychopathy: A Critical Review.” _Molecular Psychiatry_ 16(8): 792-799.

McCabe, David P., and Alan D. Castel. 2008. “Seeing is Believing: The Effect of Brain Images on Judgements of Scientific Reasoning.” _Cognition_ 107(1): 343-352.

Nadelhoffer, Thomas, Stephanos Bibas, Scott Grafton, Kent A. Kiehl, Andrew Mansfield, Walter Sinnott-Armstrong, and Michael Gazzaniga. 2012a. “Neuroprediction, Violence, and the Law: Setting the Stage.” _Neuroethics_ 5: 67-99.

Nadelhoffer, Thomas, and Walter Sinnott-Armstrong. 2012b. “Neurolaw and Neuroprediction: Potential Promises and Perils.” _Philosophy Compass_ 7(9): 631-642.

Philippi, Carissa L., Maia S. Pujara, Julian C. Motzkin, Joseph Newman, Kent A. Kiehl, and Michael Koenigs. 2015. “Altered Resting-state Functional Connectivity in Cortical Networks in Psychopathy.” _Journal of Neuroscience_ 35(15): 6068–6078.

Roskies, Adina L., N. J. Schweitzer, and Michael J. Saks. 2013. “Neuroimages in Court: Less Biasing than Feared.” _Trends in Cognitive Science_ 17(3): 99-101.

Sato, João R., Ricardo de Oliveira-Souza, Carlos E. Thomaz, Rodrigo Basílio, Ivanei E. Bramati, Edson Amaro Jr., Fernanda Tovar-Moll, Robert D. Hare, and Jorge Moll. 2011. “Identification of Psychopathic Individuals Using Pattern Classification of MRI Images.” _Social Neuroscience_ 6(5-6): 627–639. ‘

Schweitzer, Nick J., Denise A. Baker, and Evan F. Risko. 2013. “Fooled by the Brain: Re-examining the Influence of Neuroimages.” _Cognition_ 129: 501-511.

Sinnott-Armstrong, Walter, Adina Roskies, Teneille Brown, and Emily Murphy. 2008. “Brain Images as Legal Evidence.” _Episteme_ 5(3): 359-372.

Steele, Vaughn R., Vikram Rao, Vince D. Calhoun, and Kent A. Kiehl. 2015. “Machine Learning of Structural Magnetic Resonance Imaging Predicts Psychopathic Traits in Adolescent Offenders.” _Neuroimage_, in press.

Tong, Frank, and Michael S. Pratte. 2012. “Decoding Patterns of Human Brain Activity.” _Annual Review of Psychology_ 63: 483-509.

Weisberg, Deena S., Frank C. Keil, Joshua Goodstein, Elizabeth Rawson, and Jeremy R. Gray. 2008. “The Seductive Allure of Neuroscience Explanations.” _Journal of Cognitive Neuroscience_ 20(3): 470-477.

_(Image credit: [PBS](http://www.pbs.org/wgbh/nova/next/body/theres-hope-for-fmri-despite-major-software-flaws/))_