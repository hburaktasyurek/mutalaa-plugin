# Mütalaa: Hukuk, Vergi, İçtihat

Research Turkish law (hukuk), tax and fiscal legislation (vergi ve mali
mevzuat), and case law (içtihat) through primary sources. Find legislation,
article texts, legislative rationales, Yargıtay and Danıştay judgments,
Constitutional Court (AYM) decisions, and Turkish Revenue Administration
(GİB) private tax rulings. Read and compare source texts, legal concepts,
provisions, judicial reasoning and administrative interpretations with citations.

Mütalaa supports legal interpretation, academic and professional research,
regulatory compliance research, rights and obligations, disputes, and legal
remedies across Turkish public and private law. Coverage includes civil,
commercial, obligations, property, family, inheritance, employment, consumer,
criminal, administrative, constitutional and tax law, subject to the sources
available. Turkish search terms include mevzuat, kanun, yasa, yönetmelik,
gerekçe, içtihat, emsal karar, özelge and hak arama.

## Connect and research

In Claude Code, add this repository's marketplace and install Mütalaa:

```text
/plugin marketplace add hburaktasyurek/mutalaa-plugin
/plugin install mutalaa@mutalaa
```

Open `/mcp`, select the Mütalaa connection, and authenticate with your Mütalaa
account through OAuth. Start a new session and ask your legal research question.
The plugin uses the existing remote server at https://mutalaa.tr/mcp.
No local Python service, API key or additional runtime is required by this
plugin. A direct repository install does not establish Anthropic directory
approval.

Four Turkish workflow skills and four Turkish reference files are bundled.
They load through the host's skill mechanism without MCP resource reads or
private user files. Explanations follow the user's language;
Turkish source terms, tool names and official identifiers retain their spelling.

The workflows route a question to legislation, case law or tax ruling research,
read the relevant text before drawing conclusions, and explain source errors
and quotas. They do not file applications, access private case files or perform
financial transactions.

## Data and authentication

Tool calls send the required search terms, filters and public document
identifiers to the declared Mütalaa server using the authenticated account.
The server retrieves legal material from the public sources supported by
Mütalaa. Account and usage processing is described in the
[privacy policy and terms](https://mutalaa.tr/legal).

Remove identifying or confidential case details before making a request.
The skills instruct the model to anonymize tool arguments; this is a model
instruction, not a guarantee that a server-side sanitizer removes personal data.
The package contains no credentials, local server, lifecycle hooks or install
scripts.

## Sources and limits

Supported public court sources include Yargıtay, Danıştay, regional appellate
civil courts, first-instance civil courts, the kanun yararına bozma collection,
and the Constitutional Court (AYM), including constitutional review and
individual applications. A GİB private ruling is an administrative view, not a
court judgment. Criminal appellate and regional administrative court searches,
private UYAP files and foreign-law-only research are outside this release.

Mütalaa is a legal research aid, not a lawyer or a guarantee of complete,
historical or immediately updated coverage. Read relevant source texts before
relying on search results. Do not send identifying or confidential case details.
OAuth, quotas and source availability still apply.

## Publisher and support

The individual publisher and service provider is Hasan Burak Taşyürek. HB Global
is the brand he uses.

- [Website](https://mutalaa.tr)
- [Support](https://mutalaa.tr/legal): admin@hbglobal.dev
- [Privacy policy](https://mutalaa.tr/legal)
- [Terms](https://mutalaa.tr/legal)

## License

The MIT grant in `LICENSE` covers the skill/reference Markdown and plugin/MCP
manifest JSON. Mütalaa names, logos and `assets/` are excluded; no trademark or
branding rights are granted. The private backend is not included. This README
is installation documentation.
