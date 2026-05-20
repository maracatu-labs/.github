### Maracatu Labs

**Open source from Brazil: foundation models, civic AI, and network infrastructure.**

[maracatu.org](https://maracatu.org) · [Hugging Face](https://huggingface.co/maracatu-ai)

Maracatu Labs is an independent Brazilian open source effort building infrastructure and applications around three intertwined themes: foundation models native to Brazilian Portuguese, AI agents for civic transparency, and the systems software that runs them. We contribute to the [Brazilian AI Plan (PBIA 2024–2028)](https://www.gov.br/mcti/pt-br/acompanhe-o-mcti/transformacaodigital/plano-brasileiro-de-inteligencia-artificial).

## Projects

### [maracatu](https://github.com/maracatu-labs/maracatu)

Open-weight language models trained from scratch in Brazilian Portuguese. Llama-style decoder-only transformer, Apache 2.0 across code and weights. Released models so far: **Maracatu-20M** (17M params, val PP 23.81) and **Maracatu-80M** (87.8M params, val PP 21.34 on a 3.27M-token holdout — outperforming Tucano-160M with roughly half the parameters).

### [calunga](https://github.com/maracatu-labs/calunga)

A civic transparency platform: a conversational agent (LangGraph + Gemini, 15 tools) over Brazilian open data — federal expense records (CEAP), sanctions, contracts, public spending, parliamentary votes. Citizens ask questions in plain Portuguese and get answers with sources and anomaly flags from rule-based and statistical classifiers.

### [catraca](https://github.com/maracatu-labs/catraca)

A single-host TCP connection dispatcher in Rust. Uses `io_uring` `AcceptMulti` and hands file descriptors off to local workers via `SCM_RIGHTS`. Round-robin, zero byte copying, no HTTP parsing. ~300 lines, two dependencies, no async runtime — built for resource-constrained environments where every syscall counts.

## Naming

Our projects are named after elements of the *Maracatu*, an Afro-Brazilian cultural tradition from Pernambuco recognized as intangible cultural heritage by UNESCO. **Calunga** is the sacred doll carried at the front of the procession; **baque** is the constant drumbeat; **gonguê** is the bell that signals; **terreiro** is the sacred space where the *maracatu* gathers; **cortejo** is the public procession. **Catraca** (turnstile) is from a different lineage — pure systems engineering — but it shares the same theme: controlling who passes and where they go.

## Get involved

- Star a project that interests you.
- Read each repository's `CONTRIBUTING.md` for how to send patches.
- Found a security issue? See each repository's `SECURITY.md`.
- For general questions, open a discussion on the relevant repository.

## License

Each project is licensed independently — see the `LICENSE` file in each repository. Most are MIT; the `maracatu` repository (code and model weights) is Apache 2.0.
