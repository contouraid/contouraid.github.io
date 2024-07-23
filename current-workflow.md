---
layout: default
---

## Current Radiation Oncology workflow for Glioblastoma Patients

This page describes the current workflow, highlighting potential venues for improvement of the process. The TL;DR version is:

1. This is a multi-step process: initial diagnosis; resection surgery; imaging; contouring; treatment planning and then quality assurance.
2. Various clinical specialists handle each step - wait durations depends on scheduling, coordination, experience, and difficulty.
3. insta-RT can semi-automate contouring, treatment planning and quality assurance by moving away from the waterfall-like strategy to an agile workflow with shorter iteration loops to eventually lead to better treatment plans.

---

### The patient journey through a typical radiation oncology clinic

THis page walks through what could be considered as the typical steps undertaken in a radiation oncology clinic when a patient goes through the process of getting treated using radiation therapy for brain tumors like glioblastoma. There could certainly be variations to these steps depending on individual circumstances, while this is meant to describe 80% of the scenarios.

#### Initial diagnosis and tests

Most patients who enter this treatment are already symptomatic - where they enter the hospital in general with issues like (TBD: are there any specific lists of symptoms that are commonly associated with glioblastoma?) and so on. The general physician can who looks at them initially can then refer them to specialists like neurologists, who can then order an MR scan or a CT, depending on their assessment of what could be causing these symptoms.

These scans are then interpreted by a neuro-radiologist, who can then indicate that there could be a tumor or a similar pathology that can explain these symptoms. Typically, a next step then is to conduct a biopsy - where a sample of the affected tissue is excised through surgery so that a histopathological examination can be done to confirm or deny the hypothesis of the tumor being of a certain known variety of cancer, and to understand what grade it is (TBD: when is this grading done?). 

Depending on the spread and extent of the tumor, a surgical resection could be proposed. This is done typically in cases where the tumor mass is localized and can be reasonably easily reached surgically, so that it can be removed physically to the maximum extent possible. If the tumor is diffuse and has already spread to large parts of the brain, resection is not usually possible and this step of treatment is skipped to proceed directly to a combination of chemotherapy and radiotherapy, described later on.

##### Resection surgery and related procedures

The initial MR or CT scan conducted to make the diagnosis is used to plan the surgery (TBD: why is another scan not done prior to surgery here, to decide the plan for reaching the tumor?), and the goal of this procedure is to maximally remove the tumorous parts. 

##### Post-surgical imaging and evaluations

MR and CT scans are taken again (this is the second time), when the amount of resection will be known, and, how much other damage (edema, bleeding, ...) is currently present is evaluated.

Waiting for 3 weeks for the edema to heal sufficiently for radiation and subsequent treatment. 

---

#### Decision to treat with radiation therapy

This can vary depending on the prognosis: some patients reject this step (even after deciding to go ahead initially). How is the decision to do chemotherapy and radiation therapy concurrently, or sequentially done (TBD: need to get more clarity here).

#### Imaging and related considerations

MR and CT scans are taken again (this is the third time), to check if the edema has healed, and, to actually make the treatment planning with as recent a scan as possible. This happens typically 3 weeks after the surgery.

*How can insta-RT help in this step?*

---

#### Contouring and delineation

The radiation oncologist does this using current treatment planning systems. Already, many of the organs at risk (OARs) are delineated automatically (interestingly some like the eye are based on the CT image; others could be in the future based on MR), and they focus on correcting any errors, while also manually drawing the GTV (Gross Tumor Volume), then 1.5 cm dilation for the CTV (clinical TV) - which has to be corrected and edited subjectively based on other anatomical regions around (not passing through the skull to avoid skin scarring and hair loss; not passing through the dura or the cerebellum-cerebrum boundary and so on). Then, a 3 mm extension of this becomes the PTV (Planning TV), which is finally used to plan the dose next. The goal is for the 95% of the PTV to get the prescribed radiation dose, while also having as much flatness (variance of dose within the PTV minimized) in the dose profile as possible. This has to be traded off against toxic doses to the organs at risk, which have a recipe varying between hospitals. 

*How can insta-RT help in this step?*

---

#### Dosimetry and treatment planning 

This is possibly the most technically complex step. What arc angles to use? How many arcs to use (2, 3, or 4?: larger is more time consuming, but can be more conformal); what kind of treatment plan and machine to use (Trubeam IMRT, VMAT; cyberknife; ETHOS? and others); what are the priorities to apply to each organ at risk while optimizing the plan? What subjective limits on the DVH curve is applied to each organ and tumor itself to align with the clinical goals? If clinical goals cannot be met, where do we first go to trade off choices? 

*How can insta-RT help in this step?*

---

#### Quality assurance and clinical evaluations

Here is where insta-RT can help!

*How can insta-RT help in this step?*

---

#### Treatment delivery 

This is what all the previous steps culminate in - where the dose is finally delivered, typically in 30 fractions of 2 Gray each, across six weeks (M to F, Saturday and Sunday off - while also being used to conduct blood tests to ensure compliance).

[back](./)
