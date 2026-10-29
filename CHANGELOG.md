# Changelog

Tutte le modifiche rilevanti a questo plugin sono documentate in questo file.

Il formato è basato su [Keep a Changelog](https://keepachangelog.com/it/1.1.0/)
e questo progetto aderisce al [Semantic Versioning](https://semver.org/lang/it/).

## [1.1.0] - 2026-10-22

### Added
- Testi per lingua: titolo, riassunto, introduzione e link aggiuntivi si possono sovrascrivere per ogni lingua
  attiva (WPML o Polylang) da *Impostazioni → LLMs.txt → Testi per lingua*. Un campo vuoto usa il valore generale,
  quindi `/en/llms.txt` non deve più mostrare il riassunto in italiano. Senza plugin multilingua il pannello non cambia.

### Changed
- Le impostazioni della 1.0.0 restano valide e valgono come valori generali per tutte le lingue.

## [1.0.0] - 2026-10-21

### Added
- `/llms.txt` e `/llms-full.txt` generati al volo, per lingua (WPML e Polylang), con cache invalidata al
  cambiare di contenuti, categorie e impostazioni.
- Pannello *Impostazioni → LLMs.txt*: contenuti e categorie da includere, limite per tipo, ID esclusi, titolo,
  riassunto, introduzione e link aggiuntivi.
- Politica per i crawler AI (GPTBot, ClaudeBot, PerplexityBot e altri) nel `robots.txt` di WordPress.
- Filtri `wp_llmstxt_query_args`, `wp_llmstxt_post_html` e `wp_llmstxt_full_max_bytes`.
