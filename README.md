# vps price: What RackNerd's $21.99/Year KVM Plans Actually Get You, How Renewals Work, and Which Plan Fits Your Workload

Searching "vps price" usually means one of two things: you want a realistic monthly number before you commit, or you've been burned before by a cheap first term that doubled at renewal. Both are fair questions, and the honest answer is that VPS pricing splits into two very different markets — unmanaged plans starting around $2–5/month, and fully managed plans running $10–100/month depending on the provider. RackNerd sits firmly in the first camp: its current KVM VPS specials start at **$21.99/year**, which works out to about $1.83/month, with the same price locked in for every renewal.

That "locked in" part matters more than the sticker price, and it's the thing most price-comparison articles skip. More on that below.

> **Quick picks**
> - Just need a lightweight box — proxy, bot, monitoring node → **1 GB KVM VPS, $21.99/year** (1 vCPU, 20 GB SSD, 3 TB traffic)
> - Running a small site or a couple of Docker containers → **2 GB, $35.99/year** (2 vCPU, 35 GB SSD, 5 TB)
> - Heavier multi-service setups → **4 GB, $59.99/year** (3 vCPU, 60 GB SSD, 7 TB)
> - 👉 [Check RackNerd's current specials and prices](https://bit.ly/RacKnerd)

## What does a VPS actually cost?

For an unmanaged VPS — you get root access and you're responsible for everything on the server — entry-level pricing starts around $2/month, with most mainstream providers clustering between $3 and $6 for a basic 1–2 GB plan. Fully managed plans run $10 to $100 per month. That's the single biggest price gap in the market, and it's worth knowing which side of it you're shopping on before comparing any numbers.

Within the unmanaged bucket, prices vary more by billing structure than by quality. Some providers advertise a low monthly rate that only applies on longer terms or first orders. Others — RackNerd among them — sell annual specials at a flat price that recurs. A $21.99/year plan is $1.83/month; a "$2.99/month" plan billed annually is $35.88. Those two are nearly identical, so the number that actually decides value is the price times the billing cycle, not the monthly figure in the headline.

## RackNerd's current lineup at a glance

RackNerd's public VPS specials page currently lists five KVM plans, all annual, all with the same base spec: full root access, 1 Gbps port, 1 dedicated IPv4, SSD storage, and a KVM virtualization layer with a control panel for reboot, reinstall, and VNC console.

| Plan | CPU / RAM | SSD | Monthly traffic | Annual price | Order |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 vCPU / 1 GB | 20 GB | 3 TB | $21.99/yr | [Order the 1 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=952) |
| 2 GB KVM VPS | 2 vCPU / 2 GB | 35 GB | 5 TB | $35.99/yr | [Order the 2 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=953) |
| 4 GB KVM VPS | 3 vCPU / 4 GB | 60 GB | 7 TB | $59.99/yr | [Order the 4 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=954) |
| 6 GB KVM VPS | 6 vCPU / 6 GB | 100 GB | 12 TB | $89.99/yr | [Order the 6 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=955) |
| 8 GB KVM VPS | 7 vCPU / 8 GB | 150 GB | 20 TB | $119.99/yr | [Order the 8 GB plan](https://my.racknerd.com/aff.php?aff=11397&pid=956) |

Two things worth noticing in that table. The CPU allocation isn't linear — the 6 GB plan jumps from 3 to 6 vCores, so if your workload is CPU-bound rather than memory-bound, that's the sweet spot per core. And traffic allowances are generous relative to price: even the 1 GB plan includes 3 TB a month on a 1 Gbps port, which covers most self-hosted side projects many times over.

## The number nobody quotes: the renewal price

Most "cheap VPS" articles compare first-term prices and stop there. That's a problem, because the two cheapest-looking options in any comparison often have the most expensive second year. RackNerd's specials don't work that way — the company states in its own FAQ that these plans are "lifetime recurring": you renew at the same rate for as long as you keep the service. Buy the 1 GB plan at $21.99, and your renewal invoice three years from now says $21.99.

Not all of RackNerd's catalog works like this, though. The lifetime-renewal guarantee applies to the Special Promos lineup — the five plans above. RackNerd also sells regular KVM VPS products at standard monthly/annual rates, and those don't carry the same guarantee. If a renewal price matters to you (and if you're searching "vps price," it probably does), buy from the specials page specifically, not from the general product list.

One related misconception: RackNerd doesn't really run on coupon codes for VPS. The specials page *is* the discount — the prices above are already the promotional rate. Various sites circulate "RackNerd 30% off" codes, but the verifiable current codes apply to dedicated servers, not VPS plans, and older VPS codes from past New Year or Black Friday events have expired. If you see a coupon promising another cut off the prices above, treat it with suspicion.

> If the renewal math is what sold you, the cheapest way to lock it in is the entry plan: 👉 [Get the 1 GB KVM VPS at $21.99/year, recurring for life](https://my.racknerd.com/aff.php?aff=11397&pid=952)

## What's actually included at these prices

The headline prices are low enough that "what's the catch" is a reasonable question. Based on the current specials page, here's what every plan ships with:

- **KVM virtualization** with full root access — you can run your own kernel, Docker, custom ISOs on request via ticket
- **A control panel** covering reboot, OS reinstall, HTML5 VNC console (works even when the VM's network is down), root password reset, bandwidth graphs, and a network firewall that filters inbound traffic in front of the VPS
- **Choice of OS**: CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, Ubuntu
- **Multiple datacenter locations** — Los Angeles, New York, Dallas, Chicago, and others — selected at checkout
- **Instant provisioning** after payment
- **1 dedicated IPv4** and a 1 Gbps port

What you don't get is management. These are unmanaged plans: RackNerd keeps the host node and network healthy, but patching, securing, and backing up what runs inside your VM is on you. That's precisely why the price can sit at $1.83/month while managed hosts charge ten times that for the same RAM. If you want someone else to handle updates and breakage, the unmanaged price tag isn't the real comparison point — budget for managed pricing instead, or budget your own time.

## Which plan for which workload

The RAM number is the rough sorting key, but the one-click apps on RackNerd's panel make the decision more concrete, because each has a minimum memory requirement:

- **n8n, Coolify, CyberPanel/CloudPanel, Docker + Portainer** — run fine on 2 GB
- **Ollama, AnythingLLM, LibreChat, Hermes Agent** — want at least 4 GB
- **OpenClaw** — needs 8 GB

So the decision rules look like this:

1. **Lightweight background stuff** — an uptime monitor, a personal proxy, a small bot: the 1 GB plan at $21.99/year does this for about six cents a day. Paying more buys you idle RAM.
2. **A website, a game server for a few friends, Docker with one or two containers**: 2 GB at $35.99/year is the practical floor. 1 GB works for a static site but gets tight the moment a database and a PHP process share the box.
3. **Self-hosted AI tooling, multi-service homelab, several sites**: 4 GB at $59.99/year is the tier where Ollama-class apps become viable, and the 3 vCores help here too.
4. **Genuinely heavy, multi-user workloads**: 6 GB or 8 GB. If you can't name the workload, you probably don't need these yet — nothing in the lineup justifies doubling the price on speculation.

If you're not sure you'll still be using a VPS in six months, note that the specials are annual-only. The cautious move is to test your workload on the 1 GB plan — at $21.99 the downside of being wrong is small — rather than committing to a bigger plan and abandoning it mid-year.

## How RackNerd's prices compare

For context, here's what some well-known alternatives charge for comparable entry-level specs. These are information-only comparisons — check each provider's own site for current terms:

| Provider / type | Comparable plan | Advertised price | Billing notes |
| --- | --- | --- | --- |
| RackNerd | 1 vCPU / 1 GB / 20 GB SSD / 3 TB | $21.99/year (~$1.83/mo) | Annual specials, renews at the same price |
| OVHcloud | VPS Value tier | from ~€2.90/mo (intro) | EUR pricing; intro rates differ from renewal |
| Vultr | 1 vCPU / 1 GB shared | $5.00/mo | Monthly, billed as you go |
| Managed hosts (typical) | 1–2 GB managed plans | $10–100/mo | Includes maintenance and support |

The honest read: Vultr's $5/month is more flexible — no annual lock-in, hourly billing, a large location list — and if you spin servers up and down constantly, that flexibility is worth the premium. OVH's intro rate looks competitive until you check what it renews at. Where RackNerd wins is the combination of low annual cost and a renewal price that doesn't move: a 1 GB plan held for three years costs $65.97 total, versus $180 for three years of a $5/month plan at equivalent specs (with different network footprints, to be fair — Vultr has more locations).

## Buying checklist: things to know before you pay

A few practical details that affect the actual purchase, gathered from RackNerd's own pages and documentation:

1. **Payment**: PayPal, credit card, and Alipay are supported. Alipay support is a big part of why the brand is popular among users buying their first overseas VPS.
2. **Provisioning is instant** — login credentials arrive minutes after payment.
3. **Pick the datacenter deliberately.** Location is chosen during checkout and can't meaningfully be changed later. Los Angeles tends to be the default pick for Asia-Pacific latency; East Coast for European traffic.
4. **Renewal invoices generate 14 days before expiry** by default, with email reminders. You can also generate the next renewal invoice early from the client area (Services → My Services → Generate Renewal Invoice) — useful if you want to lock a year in early. Paying early extends the due date by a full cycle, so you don't lose remaining time.
5. **Miss a renewal and there's a grace period**, during which paying the invoice usually restores the server. Once the service is fully terminated and resources released, data recovery is essentially off the table. Whatever runs on this box, keep backups elsewhere.
6. **Custom ISOs are possible** but only via a support ticket — the panel's one-click list and standard OS images are what you get self-serve.

## FAQ

**Is the RackNerd renewal price the same as the first year?**
For the five plans on the specials page, yes — the company explicitly documents them as lifetime recurring, so your renewal invoice matches your original order price indefinitely. This applies to the Special Promos lineup; regular KVM products don't carry the same promise.

**Do I need a coupon code for the $21.99/year price?**
No. The specials page prices already reflect the current promotion. Widely circulated percentage-off codes either apply only to dedicated servers or have expired.

**Can I pay monthly instead of yearly?**
Not on the specials — those five plans are annual. RackNerd's regular KVM line offers monthly billing at standard rates if you need short-term flexibility, at a higher effective monthly cost.

**What happens if I outgrow my plan?**
Upgrades are handled through the control panel. If you expect to grow, starting at 2 GB costs $14 more per year than 1 GB — cheaper than migrating later, but only if you actually use the extra RAM.

**Is 3 TB of monthly traffic really enough?**
For a personal project, almost always. 3 TB on a 1 Gbps port sustains steady usage most hobby and small-business workloads never approach. Heavy media streaming or public file mirroring is where you'd start caring about the higher tiers' 7–20 TB allowances.

## The bottom line before you order

You already know the shape of the decision. Small always-on box you'll keep for a year or more → the 1 GB plan at $21.99 is hard to beat, and the renewal guarantee is what makes it cheap long-term. Running containers, a site with a database, or anything AI-adjacent → start at 2 GB or 4 GB depending on which one-click apps you're eyeing. Need hourly billing, many locations, or zero commitment → a monthly-billed provider fits better, at roughly triple the annual cost.

One last check before checkout: confirm you're ordering from the specials page (that's where the lifetime renewal price lives), and pick the datacenter closest to whoever actually uses the server. Both choices are permanent in practice. 👉 [Open RackNerd's current specials page and lock in a recurring price](https://bit.ly/RacKnerd)
