---
layout: feature
title: "Who Owns the Chart?"
dek: "Global surgery partnerships will run in both directions only when the hospitals doing the work hold their own outcome data. CESIS was built around that premise, and it is looking for collaborators."
kicker: "Global Surgery"
description: "CESIS, the Center for Equitable Surgical Information Systems: its mission, five domains, and principles, and an invitation to collaborate."
read_time: 7
image: /assets/img/posts/koidu-records-desk.jpg
---

Last week I argued that global surgery often runs in one direction. Visiting teams bring equipment and expertise, and when they leave, the data and most of the decisions leave with them. Host surgeons manage the follow-up and the complications but rarely receive anything they can use to improve their own program.<sup>1</sup>

Saying that a partnership should run both ways is easy. Specifying what has to exist for that to happen is harder, and my answer starts with records. A hospital cannot direct its own improvement if it cannot see its own results. Shared authorship and local governance both depend on a record of what happened to each patient, held by the people who cared for them, in a form they can analyze.

That premise is the basis of CESIS, the Center for Equitable Surgical Information Systems. CESIS has a founding charter, an active recovery project at Kabala Government Hospital in Sierra Leone, and a second site in Ghana. Much of it is still under construction, and this post describes what it is meant to do in the hope of drawing in collaborators and criticism.

<figure class="span">
<img src="{{ '/assets/img/posts/koidu-records-desk.jpg' | relative_url }}" alt="Two health workers sitting at a desk in a ward at Koidu Government Hospital, with paperwork and charts posted on the window behind them.">
<figcaption><b>Koidu Government Hospital, Kono District, Sierra Leone.</b> Much of the documentation in district hospitals like this one is still done by hand. Photo: John Green, <a href="https://commons.wikimedia.org/wiki/File:Koidu_Government_Hospital_Sierra_Leone_2020_04.png">Wikimedia Commons</a>, CC BY 3.0.</figcaption>
</figure>

## The leaking loop

Each operation should inform the next. In a well-resourced hospital this happens routinely: the operation is documented, the outcome is recorded, someone reviews the data, and practice changes when a complication rate rises. Surgeons in the United States spent decades building that machinery, from risk-adjusted outcome registries to the risk calculators derived from them.<sup>2</sup>

In many low-resource settings the loop breaks at nearly every step. The operation is recorded on a handwritten form, and the form is filed in a box. A wound infection two weeks later is never linked to the operation that caused it. My colleagues and I described this pattern in a recent paper as a leaky pipe, because information escapes at each transition between the operating room and the next patient, and no single loss is large enough to draw attention.<sup>3</sup>

These losses are difficult to see from inside the system. When we recovered twelve years of handwritten records from Kabala Government Hospital, we identified 99 postoperative complications that were documented in patient charts but absent from the mission case logs.

<div class="mission span">
<p class="mission-label">Our mission</p>
<p class="mission-text">To make sure that every surgical program, wherever it is and whatever it can afford, can capture, keep, and learn from its own patients’ outcomes, and to study what it takes to make that last.</p>
</div>

CESIS is an academic research program. It studies the information infrastructure on which surgical learning depends: how clinical information is captured, recovered, validated, integrated, and applied. Ayekta and the recovery pipeline are working implementations that give the research something to test against.

The condition CESIS aims for is what I call *information equity*: every surgical program, regardless of geography or budget, has a meaningful opportunity to generate, preserve, and learn from its own clinical information. The term is proposed rather than established, and I would welcome arguments against it.

## Five domains

The research is organized into five domains. Each depends on those before it, and the fifth cannot be reached without the first four.

<div class="domains span">
<div class="domain"><span class="dnum">01</span><h3>Information capture</h3><p>Prospective, point-of-care recording of surgical data, including offline-first systems with synchronization and conflict resolution for low-connectivity settings.</p><p class="dmeth"><b>Methods:</b> workflow and human factors evaluation, time-motion study. Implementation: Ayekta.</p></div>
<div class="domain"><span class="dnum">02</span><h3>Information recovery</h3><p>Structured extraction from legacy paper and scanned records, with linkage and validation to a stated level of confidence.</p><p class="dmeth"><b>Methods:</b> deterministic and model-assisted extraction, error taxonomy, reference-standard validation sampling.</p></div>
<div class="domain"><span class="dnum">03</span><h3>Information integration</h3><p>Assembly of captured and recovered data into longitudinal, interoperable datasets built on existing standards such as FHIR.</p><p class="dmeth"><b>Methods:</b> standards mapping, minimum dataset specification, identity resolution, provenance modeling.</p></div>
<div class="domain"><span class="dnum">04</span><h3>Learning systems</h3><p>Registries, audit and feedback, and benchmarking, rebuilt at a cost low-resource programs can sustain.</p><p class="dmeth"><b>Methods:</b> registry design, implementation science, prospective cohorts.</p></div>
<div class="domain"><span class="dnum">05</span><h3>Computational surgical intelligence</h3><p>Natural language processing, prediction, and decision support, developed only on data with characterized provenance and completeness.</p><p class="dmeth"><b>Methods:</b> predictive modeling, decision support, external validation.</p></div>
</div>

The FAIR principles for scientific data stewardship are a useful benchmark for integration, particularly their emphasis on explicit provenance, since a dataset built from both prospective and recovered sources may vary in reliability within a single record.<sup>4</sup> For learning systems, the WHO Surgical Safety Checklist showed that a structured information intervention could reduce deaths and complications across eight hospitals in very different settings.<sup>5</sup>

The ordering of the fifth domain is deliberate. Computational tools are attractive in global surgery, but they depend entirely on the data they are trained on. The surgical risk calculators used in the United States became possible only after a large, standardized, prospectively validated dataset existed,<sup>2</sup> and the field of surgical data science has made a similar argument about the infrastructure its own methods require.<sup>6</sup> Applied to fragmented or unvalidated surgical records, predictive models produce outputs that are plausible and incorrect.

<figure class="span">
<img src="{{ '/assets/img/posts/koidu-corridor.jpg' | relative_url }}" alt="A covered outdoor corridor at Koidu Government Hospital, with staff and visitors walking along blue-painted walls.">
<figcaption><b>An outdoor corridor at Koidu Government Hospital.</b> Photo: John Green, <a href="https://commons.wikimedia.org/wiki/File:Koidu_Government_Hospital_Sierra_Leone_2020_05.png">Wikimedia Commons</a>, CC BY 3.0.</figcaption>
</figure>

## Principles

The charter sets out seven principles, written as constraints on what CESIS will do.

<div class="principles" markdown="1">

**Equity.** The capacity to learn from clinical information should not depend on institutional wealth. Methods must be usable in the settings that need them most, beyond being demonstrated there.

**Openness.** Standards, tools, and evaluation methods are published. A program's data remain available to that program in a portable format, without exception.

**Interoperability.** Open standards are the default, and dependence on a single vendor is treated as a defect.

**Scientific rigor.** A tool that has been deployed without proper evaluation has not been studied, and CESIS will not report it as though it had.

**Clinical primacy.** Technology adapts to the surgical workflow. A system that increases documentation burden without a demonstrated learning benefit is at fault.

**Longitudinal learning.** Information systems are judged by what they allow a program to learn over years, rather than by the completeness of a single encounter.

**Technology neutrality.** CESIS holds no commitment to any product, vendor, or method, including its own, and abandons approaches the evidence does not support.

</div>

## Partnership terms

The principles above govern information. The terms that respond to last week's argument govern people. Partnerships with institutions in low- and middle-income countries carry a documented risk of extraction: data collected locally, analyzed elsewhere, published without local authors, and returned in a form the site cannot use. Each CESIS collaboration agreement states four commitments in writing:

1. Partner sites receive co-authorship on work derived from their data.
2. Analyses are returned in a form the site can use directly.
3. Each project leaves a functioning system and the local capacity to operate it.
4. The partner retains the primary data in a portable format.

The fourth commitment carries the most weight. A hospital that holds its own surgical data can set its own research questions, choose its collaborators, and measure its own progress, and a visiting team becomes a partner the hospital has chosen.

## Collaborators and feedback

CESIS is looking for collaborators, including surgeons and staff at partner hospitals, researchers in informatics and quality improvement, and students looking for a project. Critical feedback is equally useful, particularly from people who think parts of this framework are wrong. You can reach me through the <a href="{{ '/#contact' | relative_url }}">contact section</a> of this site.

The measure of success is whether surgical programs that could not previously study their own results are able to do so, and whether that capacity persists after the initiating collaboration ends.

*Next week: why surgery in low-resource settings has no equivalent of NSQIP or TQIP, and what a practical first step would be.*

<div class="refs-block">
<h2>References</h2>
<ol>
<li>Faizullabhoy E. <a href="{{ '/writing/2026/11/nurturing-the-neglected-stepchild/' | relative_url }}">Nurturing the neglected stepchild</a>. November 14, 2026.</li>
<li>Bilimoria KY, Liu Y, Paruch JL, et al. Development and evaluation of the universal ACS NSQIP surgical risk calculator: a decision aid and informed consent tool for patients and surgeons. <em>J Am Coll Surg.</em> 2013;217(5):833–842. <a href="https://doi.org/10.1016/j.jamcollsurg.2013.07.385">doi:10.1016/j.jamcollsurg.2013.07.385</a></li>
<li>Faizullabhoy E, Bocian T, Hirani F, Grotheer K, Sifri ZC. The leaky pipe: closing the surgical data-learning loop in low- and middle-income countries. <em>World J Surg.</em> 2026. <a href="https://doi.org/10.1002/wjs.70593">doi:10.1002/wjs.70593</a></li>
<li>Wilkinson MD, Dumontier M, Aalbersberg IJ, et al. The FAIR Guiding Principles for scientific data management and stewardship. <em>Sci Data.</em> 2016;3:160018. <a href="https://doi.org/10.1038/sdata.2016.18">doi:10.1038/sdata.2016.18</a></li>
<li>Haynes AB, Weiser TG, Berry WR, et al. A surgical safety checklist to reduce morbidity and mortality in a global population. <em>N Engl J Med.</em> 2009;360(5):491–499. <a href="https://doi.org/10.1056/NEJMsa0810119">doi:10.1056/NEJMsa0810119</a></li>
<li>Maier-Hein L, Vedula SS, Speidel S, et al. Surgical data science for next-generation interventions. <em>Nat Biomed Eng.</em> 2017;1(9):691–696. <a href="https://doi.org/10.1038/s41551-017-0132-7">doi:10.1038/s41551-017-0132-7</a></li>
</ol>
</div>
