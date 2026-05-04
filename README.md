# rotmeter-prompts

AI prompts for the ROT Meter fact-checking application.

## Usage

Set these environment variables in your ROT Meter instance:

```bash
PROMPT_REPO=RotFinger/rotmeter-prompts
PROMPT_BRANCH=master
```

## Prompts

- `verification_fact_check_system.yml` - Fact verification and ROT detection
- `similarity_claim_comparison.yml` - Claim similarity analysis
- `source_analysis_system.yml`, `profile_description_system.yml`, `verified_claims_system.yml`, `entity_extraction_system.yml`

## Multilingual output

`system_prompt` YAML files contain **task and style instructions only**. The app always appends a standardized multilingual JSON schema block at runtime (`PromptManager`), so you do not duplicate it here. Re-run this script after changing embedded cores in `prompt_manager.ex` to refresh the repo.

