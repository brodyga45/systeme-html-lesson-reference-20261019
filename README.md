# H5P in a systeme.io lesson: a reproducible HTML check

A minimal embed and lesson-comment procedure for course creators who want an interactive item followed by a reflection prompt. Checked on 19 October 2026 in one inactive course through the owner/admin lesson View.

**Affiliate disclosure:** brodyga45 participates in the systeme.io affiliate programme and may receive a commission from eligible purchases through the optional referral link below. This material and the synthetic check were prepared with AI assistance. No teaching history or customer results are claimed. This is an independent reference; neither vendor has endorsed it.

## What this answers

Can the public H5P documentation demo render inside a saved systeme.io lesson HTML block, accept an answer, and be followed by a lesson comment? In the tested administrative view, yes. That is narrower than validating a learner-facing LMS integration.

| Check | Observed result | Boundary |
| --- | --- | --- |
| Official H5P demo iframe | Rendered after saving the lesson | One demo, one authenticated admin View |
| Select an answer and press Check | Demo displayed 1 out of 1 points | No score transfer into course records established |
| Enable comments and submit a reflection | Owner-only synthetic comment persisted below the lesson | No independent student accounts or cohort isolation tested |

## Reproduce without importing a course package

1. Create a clearly labelled test course, module and lesson. Keep them inactive while preparing the check. A free account was sufficient for this single-course admin check; a paid purchase is unnecessary for reproducing it.
2. Open the lesson editor. Drag a **Raw HTML** block into the lesson, open **Edit code**, and replace the default block with [lesson-embed.html](lesson-embed.html). Save both the block and the lesson, then exit the editor.
3. Use the lesson's **View** action. In this check the direct admin View rendered the iframe even though the course-level preview omitted the inactive lesson. The vendor's general HTML help says HTML is not displayed in its Preview mode; do not assume all preview surfaces behave identically.
4. Interact with the official demo and press **Check**. A visible score inside the iframe is only the embedded activity's result.
5. In the lesson's settings, enable **Comments** and save. Reload the lesson View, type a clearly synthetic reflection, and submit it. Confirm the saved text appears below the lesson.

The snippet uses a fixed height of 637 pixels and the official public documentation demo. It contains no API key, learner identifier, camera permission, microphone permission or analytics code. For real content, use only a provider-approved embed URL for material you are authorised to share. Permission to view a private H5P item is not permission to make it publicly embeddable.

## Decide whether this is enough

This check may help a creator evaluating a simple lesson with an external interactive activity and reflection. **Do not use it as evidence of** independent-student access, keyboard/screen-reader accessibility, grade passback, LTI/SCORM/xAPI support, retained progress, video performance, checkout, migration, or separate cohort privacy. Those were not tested.

If your course requires two isolated cohorts, exportable discussions or recorded H5P grades, this result is insufficient to choose a platform. Test that complete learner workflow and obtain vendor confirmation before paying or migrating. No plan recommendation is made here.

## Official sources

- [systeme.io: insert HTML/CSS/JS](https://help.systeme.io/article/306-is-it-possible-to-insert-html-css-or-js-code)
- [systeme.io: add comments to a course](https://help.systeme.io/article/1718-add-comments-to-course)
- [H5P: sharing and embedding](https://help.h5p.com/hc/en-us/articles/10004208804893-How-to-share-an-H5P)
- [Public H5P documentation demo used by the snippet](https://documentation.h5p.com/content/1291910063569938878/embed)

The original wrapper and instructions are MIT licensed. The embedded H5P demo remains third-party content under its provider's terms; it is linked, not copied into this repository. See [verification.json](verification.json) for the scope of the actual check.

## Optional systeme.io account link

If the limited workflow above matches your needs, you can start with a free account and verify it yourself. **The following is an affiliate link; eligible purchases may earn the publisher a commission:** [systeme.io referral link](https://systeme.io/?sa=sa02842922474ab87f02de4e433ef1d6a3007e42d9&tk=github-html-lesson-20261019).

You can also visit [systeme.io without the referral parameter](https://systeme.io/). Check current plans and terms there. This reference does not promise attribution, commission approval or any financial outcome.
