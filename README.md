# STRUCK

The exit-boundary standard: what an output owes before anyone acts on it. STRUCK is the last legible commitment a chain makes about an output before it travels.

Every system that turns records into decisions eventually hands an output to someone who acts on it. Everything before that point is process; everything after it is consequence. STRUCK specifies what an output must carry on its face so that the party receiving it can do something other than take it or leave it: check it, and if it is wrong, show it wrong. It specifies obligations, not implementations, and binds no one to any tool, format, or vocabulary. An output produced entirely by hand can satisfy it as fully as one produced by a pipeline.

STRUCK expands as **S**upport graded, **T**raced to origin, **R**efutation stated, **U**njudged worth, **C**ontest kept, **K**nown on its face: the five obligations any evidence-grade output must carry, plus the conformance principle that makes them checkable.

<p align="center">
<img alt="CRAFT is the meta-standard for an evaluation chain, drawn as a room whose six conditions (decision context, ontology, instruments, criteria set, decision logic, feedback) run its length from world to decision. ORE is the door in and STRUCK the door out, the two boundary standards CRAFT requires; WALKRI stands at the intake fields." src="images/standards-family-0_1_0.svg" width="880">
</p>

<p align="center">
<img alt="ORE and STRUCK on their own: the two ends of any chain, independently adoptable, bracketing any process with or without CRAFT in the middle." src="images/ore-struck-pair-0_1_0.svg" width="820">
</p>

**[Read the specification](struck-0_1_0.md)** (v0.1.2)

## What it specifies

An output conforms when it carries all five obligations, or explicitly declares and justifies the absence of any that does not apply. Conformance is assessable from the output alone, with no access to the process that produced it.

- **Support graded.** The output exposes the grade profile of its material support per dimension, and never collapses it into a single combined confidence figure.
- **Refutation stated.** The output states, in terms of what could be found in the world, what would overturn it.
- **Contest kept.** Where the support disagrees, the output represents the disagreement rather than resolving it into an average that no source asserts.
- **Traced to origin.** Every rung of support is walked to ultimate origin and labeled for what it is, with stopping points declared where the walk cannot continue.
- **Unjudged worth.** The output leaves the judgment of sufficiency to the party consuming it, and carries what that party needs to make it.

The line STRUCK holds is between certifying the material and judging the use: it certifies that an output met its prestated intended use, and says nothing about whether that use was the right one. Certify the material, never judge the art.

## How STRUCK carries CRAFT's six conditions

CRAFT disciplines its six conditions inside the chain; STRUCK is where each one reaches the face of the output. What CRAFT gets from STRUCK, condition by condition:

1. **Decision Context.** The output carries what it was built and tested for, and leaves the worth-call to whoever acts on it.
2. **Technical Ontology.** The weakest supporting dimension and every flag are exposed; an obligation that does not apply is declared, not dropped.
3. **Measurement Instruments.** The instrument's uncertainty travels on the face of the output, never collapsed into one figure.
4. **Pre-Specified Criteria.** The output states, in advance and in world terms, what would show it wrong.
5. **Explicit Decision Logic.** The judgment of sufficiency is left to the consumer, and kept readable for automated ones.
6. **Feedback with Propagation.** Every rung is labeled, so an error in a released output can be traced back; a losing position is kept, so a resolution can be revisited.

The full worked account is in [`struck-craft-condition-map-0_1_0.md`](struck-craft-condition-map-0_1_0.md).

## Relations

STRUCK is independently adoptable: taking STRUCK requires taking nothing else, and STRUCK does not require CRAFT. The dependency runs the other way. CRAFT depends on ORE and STRUCK to account for what enters and leaves its chain, and a CRAFT certification is not complete without them. STRUCK draws its legibility principle from [CRAFT](https://github.com/CrossWalkri/craft-meta-standard), and its floors from the Precision-First Design Standard and the Adverse-Signal Engagement Principle, but nothing it inherits makes it need CRAFT to stand. *(See the round-room figure in the [CRAFT](https://github.com/CrossWalkri/craft-meta-standard) repository for how the three sit together.)*

The through line, stated once: every system that turns records into decisions has the same anatomy. Sources feed in material the system did not create, fields capture that material as data, and a chain of evaluation carries it to a claim someone acts on. Knowing begins honestly, or begins broken, in three places, and one standard stands at each: [ORE](https://github.com/CrossWalkri/ORE) at the source boundary, [WALKRI](https://github.com/CrossWalkri/WALKRI) at the field, [CRAFT](https://github.com/CrossWalkri/craft-meta-standard) over the whole path. STRUCK stands at the fourth place, the exit: the claim on its way out. One commitment runs through all of them: no silent trust anywhere, and the worth-judgment left visible in the hands, human or automated, that make it.

STRUCK and ORE are one handoff seen from two sides. STRUCK is what an upstream chain owes on the way out; ORE is what a downstream chain may assume on the way in. A STRUCK-conformant output is exactly the thing ORE grades well, because it arrives already carrying its grade profile, its refutation conditions, and its derivation walked to origin.

ORE and STRUCK were also designed to work as a pair, the two ends of a chain: ORE accounts for what enters, STRUCK for what leaves. They bracket the process between them regardless of how well that process is specified, so a chain with no formal specification at all still gains honest boundaries at both ends.

They are the same discipline at two boundaries, but not one posture set mirrored. ORE declares an intake posture (Screened, Graded, or Open) for how and when sources are admitted. The exit boundary has its own modes, because it varies by what an output is for and who bears its consequences, not by how sources were admitted. Same shape, different content: each boundary's postures answer that boundary's question, and the two questions differ. (The general term for what leaves is the output; "finding" is one register of output, native to evidentiary work, not the umbrella.)

## License

CC0 1.0 Universal. No permission or fee, no attribution required. See [LICENSE](LICENSE).
