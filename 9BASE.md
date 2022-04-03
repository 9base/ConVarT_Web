# Historical 9base ConVarT Web development

**Status: Historical Downstream; retained as an archive of meaningful local development.** Documentation reconstructed from repository history on 8 October 2026.

[Kaplan Lab](https://github.com/thekaplanlab/ConVarT_Web) developed the ConVarT scientific visualization resource. This fork records subsequent 9base-specific web/service work. Local development does not confer authorship of the ConVarT research, upstream implementation, underlying databases or collaborators' work.

## Verified historical scope

The all-branch audit identified 33 unique GitHub-linked `Zaryob` commits ahead of the relevant upstream comparison baselines across `master` and `zdev`, with overlap between branches. The counts include merges and must not be added together as 45 independent contributions. The visible change sequence largely runs from December 2021 through April 2022; two reachable changes carry January/February 2021 dates. Those literal commit dates do not establish when the repository entered 9base.

Verified local changes include configurable paths ([babce1f4](https://github.com/9base/ConVarT_Web/commit/babce1f435654283a9a89c1e5070cf1ec52c5d51)), development Docker Compose setup ([7462f9c3](https://github.com/9base/ConVarT_Web/commit/7462f9c3)), SQL/search structure changes ([7277cfe1](https://github.com/9base/ConVarT_Web/commit/7277cfe1)), submission/result UI work and dbSNP/API corrections ([fed1d0ad](https://github.com/9base/ConVarT_Web/commit/fed1d0ad)). These support Historical Downstream rather than a plain preserved-reference classification.

Süleyman Poyraz (`Zaryob`) is the verified local author identity used in the audit. One other ahead commit, `00427230`, is by `asayici`; its author's organizational affiliation is unverified, so it is not assigned to 9base.

## Branch record before documentation curation

| Branch | Comparison | Result |
| --- | --- | --- |
| `master` (default) | Kaplan Lab `master` | 12 ahead, 0 behind; 11 GitHub-linked Poyraz commits. |
| `zdev` | Kaplan Lab `master` fallback; no same-named upstream branch | 33 ahead, 0 behind; 32 GitHub-linked Poyraz commits. |
| `dev` | Kaplan Lab `dev` | Identical. |
| `msa_viewer` | Kaplan Lab `msa_viewer` | Identical. |

All branches remain part of the archive. See the existing [development instructions](docs/HowToRun.md) and [dependencies](docs/Dependencies.md). They document a historical Docker/MySQL/phpMyAdmin setup; curation did not execute the stack or verify a live scientific service. The [`zdev` schema](https://github.com/9base/ConVarT_Web/blob/zdev/sql/structure.sql) includes `convart_gene` and `convart_gene_to_db`, also constructed by the companion R tooling.

## ConVarT repository family

| Repository | Role and attribution |
| --- | --- |
| [ConVarT_Web](https://github.com/9base/ConVarT_Web) | Kaplan Lab web/service project with historical 9base configuration, search and UI development. |
| [ConVarT_pipeline](https://github.com/9base/ConVarT_pipeline) | Kaplan Lab analysis pipeline, retained without verified 9base branch divergence. |
| [ConvartDataGenerate](https://github.com/9base/ConvartDataGenerate) | Original Süleyman Poyraz R scripts for FASTA/metadata preparation and SQL generation. |

The family links describe related roles; they do not establish deployment of every component or assign Kaplan Lab scientific authorship to 9base.

The existing [README scientific overview](README.md) and upstream notices are preserved. This reconstruction does not add a license, infer a transfer date, or claim ongoing maintenance.
