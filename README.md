DNS: The Part of Your Internet Connection You Probably Never Think About

You use DNS every time you use the internet, whether you realize it or not.

Before your device can connect to example.com, something has to figure out where that domain actually lives. That job falls to a DNS resolver. Most people simply use whatever resolver their ISP, router, operating system, browser, or network happens to provide.

And for a lot of people, that's completely fine.

But DNS can be much more than just "the thing that turns a website name into an IP address."

The resolver you choose can affect privacy, security, filtering, reliability, performance, and how much control you have over your network. DNS can also be used as an additional security layer to block known malicious domains, phishing infrastructure, trackers, unwanted content, or other categories of traffic before your device even attempts to connect. {"fallbackMarkdown":"(RFC Editor
)","reference":{"matched_text":"","prefix":null,"start_idx":1223,"end_idx":1255,"safe_urls":["https://www.cloudflare.com/learning/access-management/what-is-dns-filtering/","https://www.cloudflare.com/learning/access-management/what-is-dns-filtering/?utm_source=chatgpt.com","https://www.rfc-editor.org/info/rfc8932/","https://www.rfc-editor.org/info/rfc8932/?utm_source=chatgpt.com"],"refs":[],"alt":"(RFC Editor
)","prompt_text":null,"type":"grouped_webpages","error":null,"style":null,"items":[{"title":"RFC 8932: Recommendations for DNS Privacy Service Operators | RFC Editor","url":"https://www.rfc-editor.org/info/rfc8932/?utm_source=chatgpt.com","attribution":"RFC Editor","pub_date":1601510400,"snippet":"","attribution_segments":null,"supporting_websites":[{"title":"What is DNS filtering? | Secure DNS servers | Cloudflare","url":"https://www.cloudflare.com/learning/access-management/what-is-dns-filtering/?utm_source=chatgpt.com","pub_date":null,"snippet":"","attribution":"Cloudflare"}],"refs":[{"turn_index":0,"ref_type":"search","ref_index":0},{"turn_index":0,"ref_type":"search","ref_index":3}],"hue":null,"attributions":null}],"fallback_items":null,"status":"done"},"showLoginRequiredCard":false}

That makes choosing a DNS provider less trivial than simply picking the address with the lowest ping.

Why should you care?

Think of DNS as one of the first stops your traffic makes when you ask the internet for something.

The resolver you use can potentially see the DNS queries being sent to it, which means the provider's privacy practices, logging policies, security practices, and business model actually matter. Encryption such as DNS-over-HTTPS (DoH) or DNS-over-TLS (DoT) can protect DNS traffic while it travels between you and the resolver, but it doesn't remove the need to trust the resolver itself. {"fallbackMarkdown":"(RFC Editor
)","reference":{"matched_text":"","prefix":null,"start_idx":1874,"end_idx":1906,"safe_urls":["https://www.rfc-editor.org/info/rfc8932/","https://www.rfc-editor.org/info/rfc8932/?utm_source=chatgpt.com","https://www.rfc-editor.org/info/rfc9076/","https://www.rfc-editor.org/info/rfc9076/?utm_source=chatgpt.com"],"refs":[],"alt":"(RFC Editor
)","prompt_text":null,"type":"grouped_webpages","error":null,"style":null,"items":[{"title":"RFC 8932: Recommendations for DNS Privacy Service Operators | RFC Editor","url":"https://www.rfc-editor.org/info/rfc8932/?utm_source=chatgpt.com","attribution":"RFC Editor","pub_date":1601510400,"snippet":"","attribution_segments":null,"supporting_websites":[{"title":"RFC 9076: DNS Privacy Considerations | RFC Editor","url":"https://www.rfc-editor.org/info/rfc9076/?utm_source=chatgpt.com","pub_date":null,"snippet":"","attribution":"RFC Editor"}],"refs":[{"turn_index":0,"ref_type":"search","ref_index":0},{"turn_index":0,"ref_type":"search","ref_index":8}],"hue":null,"attributions":null}],"fallback_items":null,"status":"done"},"showLoginRequiredCard":false}

At the same time, different DNS services can make very different tradeoffs.

Some focus heavily on privacy.
Some focus on security.
Some offer extensive filtering and customization.
Some prioritize simplicity and reliability.
Some combine several of these approaches.

There isn't necessarily one configuration that makes sense for everyone.

So... which one should you use?

That's where this wiki comes in.

The goal isn't to tell you "use this DNS provider because it's the best."

Instead, the wiki breaks down the things that actually matter when comparing providers, so you can understand what you're choosing.

You'll find explanations and comparisons covering things such as:

Privacy & logging — What information can a resolver see, what might be retained, and what the provider says it does with that information.

Security — Malware, phishing, malicious-domain blocking, threat intelligence, and other security features.

Filtering — How DNS-level blocking works and what you can actually control.

Encryption — DoH, DoT, and what encrypting DNS does — and importantly, what it doesn't do.

Performance & reliability — Why a resolver being fast isn't the only thing that matters.

Customization — Blocklists, allowlists, policies, categories, and per-device or per-network rules.

Transparency & trust — Who operates the service, what they disclose, and why the provider's policies matter.

Censorship & network restrictions — How DNS choices can interact with networks that interfere with or restrict DNS traffic.

Technical differences — The stuff that becomes important once you go beyond the basic setup.

Real-world tradeoffs — Because every additional feature can come with its own compromises.

DNS is infrastructure. Infrastructure deserves a little more thought than simply copying an IP address from a random forum post.

You don't need to be a networking expert

If you don't know what a recursive resolver is, what DoH means, or why a DNS provider can see your queries, start with the beginner sections.

They're written to build the concepts from the ground up without assuming you already know networking.

If you already understand DNS, the later sections go deeper into the technical and operational differences that can actually matter when you're deciding between services.

The wiki is meant to work at both levels:

Beginner: "What does changing my DNS actually do?"

Advanced user: "What are this provider's transport options, logging practices, filtering architecture, and operational tradeoffs?"

Both questions are worth answering.

Before you choose, understand what you're choosing

Changing DNS is easy.

Understanding who you're handing your DNS queries to, what that provider does with them, what protections they actually provide, and what tradeoffs you're accepting is the part that deserves attention. {"fallbackMarkdown":"(RFC Editor
)","reference":{"matched_text":"","prefix":null,"start_idx":4845,"end_idx":4877,"safe_urls":["https://www.internetsociety.org/resources/doc/2023/fact-sheet-encrypted-dns/","https://www.internetsociety.org/resources/doc/2023/fact-sheet-encrypted-dns/?utm_source=chatgpt.com","https://www.rfc-editor.org/info/rfc8932/","https://www.rfc-editor.org/info/rfc8932/?utm_source=chatgpt.com"],"refs":[],"alt":"(RFC Editor
)","prompt_text":null,"type":"grouped_webpages","error":null,"style":null,"items":[{"title":"RFC 8932: Recommendations for DNS Privacy Service Operators | RFC Editor","url":"https://www.rfc-editor.org/info/rfc8932/?utm_source=chatgpt.com","attribution":"RFC Editor","pub_date":1601510400,"snippet":"","attribution_segments":null,"supporting_websites":[{"title":"Encrypted DNS Factsheet - Internet Society","url":"https://www.internetsociety.org/resources/doc/2023/fact-sheet-encrypted-dns/?utm_source=chatgpt.com","pub_date":null,"snippet":"","attribution":"Internet Society"}],"refs":[{"turn_index":0,"ref_type":"search","ref_index":0},{"turn_index":0,"ref_type":"search","ref_index":9}],"hue":null,"attributions":null}],"fallback_items":null,"status":"done"},"showLoginRequiredCard":false}

So if you're considering changing your DNS, don't just jump to a provider because someone said it's "fast," "private," or "secure."

Read the wiki first.

Then make the choice based on what actually matters to you.
