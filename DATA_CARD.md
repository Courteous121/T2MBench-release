# T2MBench Data Card

## Overview

T2MBench is a text-to-motion benchmark designed to evaluate generated human
motion under diverse natural-language instructions. The benchmark organizes
prompts by category and subcategory, and provides prompt metadata and
representative qualitative examples.

This repository is a review-stage release. It contains benchmark prompts,
metadata, representative examples, and the LLM evaluator prompt template needed
to inspect the benchmark structure. Due to the large scale of the generated data
and related intellectual property considerations, the complete data package will
be released after paper acceptance.

## Released Contents

This review-stage repository includes:

- Standardized benchmark prompts and metadata in `instructions/`.
- The LLM-based evaluation prompt template in `llm_evaluation/`.
- Representative prompt-level qualitative examples in `examples/`.

The repository does not include quantitative evaluation results, processing
scripts, or the complete generated output archive at this stage.

## Prompt Data

Each prompt is assigned a stable prompt identifier, such as `T2MB_0276`.
Prompt metadata includes category, subcategory, length type, source split, source
folder, source file, and local prompt index. The canonical prompt table is:

`instructions/t2mbench_prompts.csv`

## Generated Outputs

Representative generated outputs are included only as lightweight qualitative
examples. They are intended to help reviewers inspect prompt-level behavior
across models. The full set of generated outputs will be released after paper
acceptance.

## Intended Use

The released materials are intended for:

- Academic review and reproducibility inspection.
- Benchmark structure inspection and prompt-level comparison.
- Non-commercial research on text-to-motion evaluation.
- Development of evaluation tools for generated human motion.

## Out-of-Scope Use

The released materials are not intended for:

- Commercial use without explicit permission.
- Re-identification or attribution of anonymous review materials.
- Training systems that violate the terms of any underlying third-party models,
  datasets, or generated outputs.
- Redistribution of representative or full generated outputs outside the
  applicable license terms.

## Ethical and Privacy Considerations

The benchmark prompts describe human motion at the text level. The representative
motion outputs are generated samples and are not intended to identify real
people. The repository has been prepared for anonymous review and should not
contain personal author information.

Users should still review any downstream use for privacy, safety, and licensing
risks, especially when combining these materials with third-party datasets,
models, or generated outputs.

## Licensing

This repository is provided under the review-stage terms in `LICENSE`. Third-party
models, datasets, code, and generated outputs may have their own licenses. Users
are responsible for complying with all applicable third-party terms.

## Maintenance and Future Release

The current release is intended for review. After paper acceptance, the authors
plan to release the complete benchmark package, including quantitative evaluation
results, processing scripts, and the full generated outputs, with final
documentation and license terms.
