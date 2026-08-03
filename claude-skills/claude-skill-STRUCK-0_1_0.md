---
title: STRUCK Skill
version: 0.1.0
date: 2026-08-03
status: Procedural encoding of STRUCK v0.1.2 for AI-assisted production and audit of evidence-grade outputs. Structured so a partial task can be received and completed correctly.
related_documents:
  - struck-0_1_0.md (v0.1.2)
  - ORE v0.1.2 (ore-specification-0_1_2.md; github.com/CrossWalkri/ORE)
  - CRAFT (github.com/CrossWalkri/craft-meta-standard)
  - struck-prompts-0_1_0.md (v0.1.0)
license: CC0 1.0
---

# STRUCK Skill

Invoke this skill before producing any output offered as evidence-grade, and before auditing such an output, whether your own or another party's. This is a procedural encoding of STRUCK (Support graded, Traced to origin, Refutation stated, Unjudged worth, Contest kept, Known on its face) v0.1.2, the exit-boundary standard: what an output owes before anyone acts on it.

STRUCK sits at one of the two boundaries of any evidence-using process. ORE, its companion, covers what a system may assume about what enters it; STRUCK covers what an output owes on the way out. A system operating both has an account of its material at entry and an account of what rests on it at exit. This skill is the exit half. Where an output rests on graded material, STRUCK's grade-profile obligation (Part I) is ORE's exposure obligation applied at the output boundary; STRUCK requires that the profile be exposed, not that ORE be the thing that produced it. STRUCK is independently adoptable, and this skill does not re-encode ORE's grading procedure.

## The commitment that holds through every operation below

STRUCK makes an output checkable, not correct. Every obligation here answers one question: can the party who receives this output do something other than take it or leave it? None of them answers "is the conclusion right." An output that satisfies all five and reaches a wrong conclusion has still conformed, because a reader can now see that it is wrong; an output that reaches a right conclusion no reader can check has not. The corpus carries the distinction in its own words: certify the material, never judge the art.

The failure STRUCK exists to catch is not fabrication. It is the output that is entirely accurate and structurally unusable: it states a conclusion without stating what would overturn it, averages away the disagreement its sources contained, cites a secondary source as though it were an origin, and arrives with a confidence the reader cannot audit. Such an output can only be accepted or rejected, both of them uninformed.

Two consequences hold throughout and are not negotiable per task:

- **Never combine the support into a single confidence figure.** A per-dimension profile is hard to tune silently and cheap to audit; one number is the reverse. This refusal is inherited from ORE for the same adversarial reason.
- **Keep every obligation on the face of the output.** Exposure carried in an appendix the claim can be read without is not on the face. A claim severed from what qualifies it travels alone into every downstream use.

## Runtime Sequence

Identify what is requested and run it in full.

1. **Output production.** Producing an output offered as evidence-grade. Run all five obligations, Parts I through V, then confirm conformance, Part VI. The assembled procedure is Part VII.
2. **Output audit.** Assessing an existing output against STRUCK. See Part VIII.
3. **Single-obligation work.** A task touching one obligation, such as stating refutation conditions, representing a contest, or labeling a derivation chain. Run the corresponding Part.

The five obligations are Parts I through V; conformance is Part VI. Each stands on its own so a partial task lands correctly.

---

## Part I: Graded evidence (Support graded)

Expose the grade profile of everything the output rests on. For each dimension of source quality, report the weakest assessment present anywhere in the support, plus every flag any source in it carries. The profile is per dimension; imply no ordering across dimensions, and never compress it into one number.

STRUCK's obligation is the exposure, not the production of the grades: it requires that whatever grade profile the support carries appears on the output's face, per dimension. Producing that profile is the ingestion boundary's work, which ORE specifies where ORE is adopted; STRUCK is independently adoptable and conforms with any grading scheme that yields a per-dimension profile. Three rules bind how the profile appears:

- Where the output rests on ungraded material admitted under an Open posture, say so on the face, and never cite quarantined material as support.
- Where separately admitted sources cannot be shown distinct in effective origin, carry the joint-support flag. Separately admitted is not independently originated.
- Never present a single combined confidence figure in place of the per-dimension profile.

An output whose support is thin is not thereby weak. It is one whose reader can see what is being trusted. That is the whole of what the obligation buys, and it is enough.

---

## Part II: Refutation conditions (Refutation stated)

State what would overturn the output: the observation, measurement, disclosure, or counter-evidence whose appearance would require it to be withdrawn or revised, in terms concrete enough that a reader could recognize the refuting thing on meeting it.

- State the conditions in terms of what could be found in the world, not in terms of internal process. "If further review disagrees" is not a refutation condition; "if the two registries report different totals for the same period" is.
- Where no condition can be stated, say so and name why: the claim may be definitional, the domain may not yet admit the observation, or the output may be impressionistic in CRAFT's sense. Declaring unfalsifiability is conformant; presenting an unfalsifiable claim in falsifiable dress is not.
- Never set a condition at a threshold known to be unreachable. A condition no available instrument could satisfy is a refusal to be checked, written as an invitation.

The obligation is not that the output be refutable by someone with unlimited resources. It is that the reader be told, in advance and in the producer's own words, what the producer would accept as being wrong.

---

## Part III: Contested regions rather than averages (Contest kept)

Where the material supporting the output disagrees, represent the disagreement rather than resolving it into a central value.

- Name the region of contest: what is disputed, which support sits on each side, and what the disagreement turns on where that is visible.
- Never report a mean, median, midpoint, or consensus figure that no source asserts and that conceals the spread it was computed from. Where a central value is genuinely informative it may sit alongside the contest, never in place of it.
- Where you resolve a contest, state the basis and retain the losing position in the record. A resolution whose reasoning is not stated is a preference; a losing position silently dropped cannot be revisited when new evidence arrives.
- Where disagreement is absent because only one line of support was consulted, record the absence of contest as unexamined rather than as agreement. Uncontested and confirmed are different states.

An average across a genuine disagreement is precise, defensible, and about nothing, and its precision is what makes it durable: it survives into every downstream use carrying none of the doubt that produced it.

---

## Part IV: Derivation chains to ultimate origin (Traced to origin)

Trace the support to ultimate origins, with every intermediate rung labeled for what it actually is.

- Identify each rung by its own role: originating observation, primary record, aggregator, secondary reporting, review, restatement. A source that restates another is labeled as restating it, with the restated source named.
- Where a chain cannot be walked to origin, record where the walk stopped and why: the origin is unpublished, the aggregator does not disclose its inputs, the trail ends in an unattributed claim. A truncated chain honestly labeled is conformant; a chain presented as reaching origin when it stops at an aggregator is not.
- Never present a rung at a standing higher than it holds. Citing a review as though it were the study, or an aggregator as though it were the registry, is the ordinary form of this failure and it is usually inadvertent.
- Where two apparently distinct chains converge on the same origin, record the convergence. This is the derivation-side form of the joint-support flag, and it is the specific failure that makes corroboration counts untrustworthy: chains that share an origin agree because they must.

---

## Part V: The worth-judgment stays with the consumer (Unjudged worth)

Leave the judgment of sufficiency to the party consuming the output, and carry on the output's face what that party needs to make it.

- Never assert that the support is adequate to any particular decision. Report what the support is; whether it suffices depends on what is being decided and what being wrong would cost, neither of which the producer generally knows.
- Where the output is addressed to a decision whose stakes the producer does know, it may state what it would take to raise confidence and what that would cost, which aids the judgment rather than substituting for it.
- Where the consumer is automated, the obligation is unchanged: the decision logic that composes outputs into an action must itself be readable and challengeable, so the judgment is made from the readings rather than in silence.
- Never structure the output so that the exposure required by Parts I through IV is separated from the claim. Material in an appendix the claim can be read without is not on the face.

This obligation carries the whole standard's line inside itself: the producer certifies the material and does not judge the art. Worth is the reader's to weigh.

---

## Part VI: Conformance (Known on its face)

An output conforms when it carries all five obligations, or explicitly declares and justifies the absence of any that does not apply. The declaration is itself conformant; silence is not.

Conformance is assessable from the output alone. No obligation requires access to the producing process, the tools used, or any implementation. The assessment answers five questions:

1. Is the support graded and exposed per dimension?
2. Are refutation conditions stated in world terms?
3. Is disagreement represented rather than averaged?
4. Is every rung labeled for what it is, with stopping points declared?
5. Is the sufficiency judgment left to the consumer, with what they need to make it present on the face?

An output that fails any of the five is not thereby false. It is one whose reader cannot check it, which is a different and more durable problem.

---

## Part VII: Output production, assembled

When producing an output offered as evidence-grade, meet all five obligations or declare which does not apply and why:

1. Graded evidence (Part I): expose the support per dimension, weakest assessment and every flag, no combined figure.
2. Refutation conditions (Part II): state what would overturn it, in world terms.
3. Contested regions (Part III): represent disagreement rather than averaging.
4. Derivation to origin (Part IV): labeled chains carried onto the face, stopping points declared.
5. Unjudged worth (Part V): leave sufficiency to the consumer.

Then confirm conformance (Part VI) and keep all five on the face. An output not offered as evidence-grade is out of scope: an opinion, a summary presented as a summary, or an exploratory note is not bound here, and labeling such an output evidence-grade to borrow the standing while avoiding the obligations is the failure the scope boundary names.

---

## Part VIII: Output audit

Assess an existing output against the five obligations. Report pass, fail, or not-applicable-with-reason for each, name the specific passage for every failure, and say what would fix it.

Look specifically for the four failures that are common and quiet: a central value no cited source asserts; a review or aggregator cited at the standing of a primary record; refutation conditions phrased as process rather than observation; and a dissenting source dropped rather than represented.

Close with a verdict that distinguishes the two possible claims. An output failing an obligation is not thereby false; it is an output its reader cannot check. Say which you are asserting, and never claim an output is wrong when what has been established is that it is unverifiable.

---

## Relations to the rest of the corpus

**ORE (Origin, Reliability, Exposure)** is the companion at the ingestion boundary. Part I of this skill is ORE's exposure obligation (its Section 5) applied at the output boundary, and the refusal to combine grades is ORE's (its Section 2), adopted for the same adversarial reason. ORE covers the material at entry; STRUCK covers what rests on it at exit; a system operating both has both accounts. STRUCK shares this exposure obligation by reference and is independently adoptable: it requires the exposure, not a particular grading procedure, so it does not depend on ORE to run. Where ORE is the ingestion companion, the grades exposed are ORE's; where it is not, they are whatever the support carries.

**CRAFT (Chains Reveal Attested Falsifiable Truth)** is the meta-standard for evaluation chain legibility. The legibility principle and the notion of an impressionistic claim are CRAFT's. Part II's refutation obligation is the output-level realization of what CRAFT requires of an evaluation chain, and Part IV's labeled rungs serve CRAFT Condition 6's requirement that detected errors propagate back to every prior stage, which is only possible where the stages are named. STRUCK inherits CRAFT by reference and is independently adoptable.

**WALKRI** is the instrument-level standard at the intake fields. Where an output reports values collected through defined fields, the reproducibility of those fields is WALKRI's obligation and is not discharged by anything here. An output built on labels rather than instruments can satisfy STRUCK and remain unreliable; neither standard substitutes for the other.

**Precision-First Design Standard.** Every obligation here is held to operational definability. A refutation condition that two independent readers cannot assess the same way from its wording is a precision deficit in the output, not a matter of taste.

**Adverse-Signal Engagement Principle Core Standard.** Part III's requirement that a losing position be retained rather than dropped is the no-silent-discard obligation, applied to the internal disagreements of an output rather than to signals about a source.

## The expansion

STRUCK names its own obligations: **S**upport graded (Part I), **T**raced to origin (Part IV), **R**efutation stated (Part II), **U**njudged worth (Part V), **C**ontest kept (Part III), **K**nown on its face (Part VI). The expansion is posture-neutral: it holds wherever an output is offered as evidence-grade, whatever the exit posture, and Unjudged worth carries the certify-the-material-never-judge-the-art line inside it.
