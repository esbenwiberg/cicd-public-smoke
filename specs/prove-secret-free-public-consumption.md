# Prove secret-free public consumption

This fork is a neutral qualification fixture, not a deployment or release target.
Its manual-only public-consumption workflow fetches the released source and
installer action by the existing v5.1.5 content identity, then runs the quality
module against the source repository's own Go fixture.

The job has read-only contents permission, uses no repository secrets, configures
no source credential and refuses an unexpected authentication token or SSH agent.
It checks witnessed test counts, measured coverage, commit identity and native
errors rather than equating a successful export with a passing test gate.

This proves one public module/action execution route on a fresh hosted runner.
It does not certify other applications, every module, scanner coverage, delivery
protocols or deployment safety. Coverage-ratchet skips and other native warnings
remain evidence, not claims of complete enforcement. Inherited automation remains
disabled; only the explicit qualification workflow is run.
