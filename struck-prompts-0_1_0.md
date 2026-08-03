
# STRUCK Prompts

**Copy-and-run prompts for producing and auditing evidence-grade outputs** · v0.1.0 · 2026-08-03 · CC0 1.0

Two prompts implementing STRUCK in any AI assistant. Each is self-contained: it carries the obligations it needs, so it works pasted into a fresh conversation with no prior context and no tooling. Paste one, add your material where marked, run it.

STRUCK is the exit-boundary standard: what an output owes before anyone acts on it. These prompts encode obligations, not answers. Each ends by handing the sufficiency judgment back to you, which is the point rather than a hedge.

---

## 1. Produce an output that meets STRUCK

Use when turning material into something someone will act on.

```
Produce an output from the material I give you, offered as evidence-grade, carrying
the five obligations of STRUCK. Meet all five, or explicitly say which one does not
apply here and why. Silence about an obligation is not conformance.

STRUCK makes an output checkable, not correct: its obligations let a reader do
something other than take it or leave it. None of them ask you to judge whether the
conclusion is good.

1. SUPPORT GRADED. Expose what the output rests on. For each dimension on which the
   support is graded, report the weakest assessment present anywhere in the support,
   plus every gap or flag any source carries. If some support is ungraded, say so on
   the face of the output rather than treating it as graded. If separately obtained
   sources cannot be shown distinct in origin, flag that. Do not compress this into a
   single confidence number: one number is easy to tune and hard to audit.

2. REFUTATION STATED. State what would overturn this output, in terms of what could
   be found in the world rather than in terms of process. "If further review
   disagrees" is not a refutation condition; "if the two registries report different
   totals for the same period" is. If nothing could refute it, say so and name why:
   the claim may be definitional, or the domain may not yet admit the observation.
   Declaring that is honest; dressing an unfalsifiable claim in falsifiable language
   is not. Do not set a condition at a threshold nothing available could reach.

3. CONTEST KEPT. Where the material disagrees, represent the disagreement. Name what
   is disputed, which support sits on each side, and what the disagreement turns on.
   Do not report a mean, median, or midpoint that no source asserts and that hides the
   spread. If you resolve a contest, state the basis and keep the losing position in
   the record. Where there is no disagreement only because one line of support was
   consulted, record that as unexamined rather than as agreement.

4. TRACED TO ORIGIN. Trace the support to ultimate origins, with every rung labeled
   for what it actually is: originating observation, primary record, aggregator,
   secondary reporting, review, restatement. Where the trail stops short of origin,
   say where and why. Do not present a review as the study or an aggregator as the
   registry. Where two chains that look distinct reach the same origin, say so.

5. UNJUDGED WORTH. Do not tell me the support is adequate. Report what it is; whether
   it suffices depends on what I am deciding and what being wrong would cost, which you
   do not know. You may tell me what would raise confidence and what that would take.
   The judgment is mine.

Keep all five on the face of the output. Do not put the exposure in an appendix the
claim can be read without.

THE MATERIAL:
[paste it here]

THE QUESTION THE OUTPUT SHOULD ANSWER:
[state it here]
```

---

## 2. Audit an existing output against STRUCK

Use on another party's output, or your own before publishing.

```
Audit the output below against STRUCK, the exit-boundary standard for what an
evidence-grade output owes on its face. Report per obligation: pass, fail, or not
applicable with a stated reason. Then give a verdict.

The five obligations:

1. SUPPORT GRADED. Does it expose what it rests on, per dimension, including the
   weakest support and any gaps? Or does it assert a conclusion with a single
   confidence figure and no visible basis?

2. REFUTATION STATED. Does it state what would overturn it, in terms of what could be
   found in the world? Or are the refutation conditions absent, phrased as process, or
   set at a threshold nothing could reach?

3. CONTEST KEPT. Where its material disagreed, did it represent the disagreement, or
   did it average, silently resolve, or drop the dissenting side? Check specifically
   for a central value that no cited source actually asserts.

4. TRACED TO ORIGIN. Are its derivation chains walked to origin with each rung labeled
   honestly? Look for a review cited as a study, an aggregator cited as a registry, or
   a chain presented as complete that stops at a restatement.

5. UNJUDGED WORTH. Does it leave the sufficiency judgment to its reader, or does it
   declare its own support adequate to the decision?

For each failure, name the specific passage and say what would fix it.

Then the verdict. An output that fails an obligation is not thereby false; it is an
output its reader cannot check. Say which of the two you are claiming, and do not claim
the output is wrong when what you have established is that it is unverifiable.

THE OUTPUT:
[paste it here]
```

---

## Notes

These prompts state obligations and leave the judgment to you. Neither will tell you an output's conclusion is right; STRUCK certifies that the output can be checked, not that it is correct. An assistant that runs one of these and hands you a single adequacy verdict has departed from the specification.

These are STRUCK's standalone prompts, for the output boundary alone. Where a process also grades the sources feeding it, that is the ingestion boundary, and ORE's prompts cover it; the two standards bracket a process from either end, with or without CRAFT specifying the chain in the middle.

The specification: [STRUCK](struck-0_1_0.md), CC0. Its ingestion-boundary companion is [ORE](https://github.com/CrossWalkri/ORE).
