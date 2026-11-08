# A Website Hosting Server, Explained: Shared vs VPS vs Dedicated, When You Need a Whole Machine, and What $79 a Month Buys (Plan Table + Pre-Order Checklist)

A website hosting server is the always-on computer that stores your site's files, runs its code, and answers every request that arrives through your domain. How much of that machine belongs to you alone is the biggest decision in buying hosting, and it's usually the one buried deepest in plan comparison pages.

Three levels cover most of it. Shared hosting puts your files on a server you split with hundreds of other sites. A VPS reserves a slice of one physical machine and hands you root access. A dedicated server gives you the whole box and the whole bill with it. Nearly every first website belongs in the first group. The question worth answering is where the line sits between the second and third, and what crossing it costs.

Below: what each type actually gives you, the thresholds that justify bare metal, verified pricing on both sides of that line, and the terms to read before you pay.

> **Short version:** a blog, brochure site or small store runs fine on shared hosting or a small VPS, and buying bare metal at that stage wastes money. Once you need root access plus hardware no other tenant can slow down, SpinServers' entry config, an Intel Xeon E3-1280 v5 with 4 cores, 32 GB RAM, 1 TB NVMe and 30 TB of transfer, is **$79/month** on month-to-month billing with no setup fee. 👉 [See the current dedicated server plans](https://bit.ly/Spinservers)

## SpinServers dedicated plans at a glance

| Plan | Core specs | Price and term | Best for | Order |
| --- | --- | --- | --- | --- |
| Intel Xeon E3-1280 v5 (Dallas) | 4 cores, 32 GB RAM, 1 TB NVMe, 30 TB transfer, dual 10 Gbps ports | $79/mo, month-to-month | A first dedicated box; sites that have outgrown a VPS | [View this plan](https://bit.ly/Spinservers) |
| Intel Xeon E3-1280 v5 (San Jose) | Same hardware, West Coast location | $79/mo, month-to-month | Same workload with US Pacific latency | [View this plan](https://bit.ly/Spinservers) |
| Dual Intel Xeon Gold 6148 (Dallas) | 40 cores, 256 GB RAM, 3.8 TB SSD, 30 TB transfer | $235/mo, month-to-month | Multi-site stacks, busy stores, heavy database work | [View this plan](https://bit.ly/Spinservers) |
| Dual Intel Xeon Platinum 8173M (Dallas) | 56 cores, 512 GB RAM, 7.7 TB SSD, 30 TB transfer | $390/mo, month-to-month | Running your own VMs, CI runners, large client fleets | [View this plan](https://bit.ly/Spinservers) |

Prices are USD, read from SpinServers' instant-dedicated store pages in September 2026. None of the four carries a promotional first-term rate, so there's no renewal jump waiting at month thirteen. Pre-built inventory rotates, which means the exact CPU, RAM and disk combination available on a given day can shift, so confirm the spec sheet in the cart before checkout.

## What a hosting server actually does

The server is a physical computer in a data center with a fixed IP address. Your domain is a pointer that resolves to that address. The two are separate purchases: a domain is registered with a registrar and renewed annually, and hosting does not include it unless a provider bundles it as a promotion. Budget for it as its own line item.

When you open a hosting account, the provider allocates space on one of its machines along with CPU, RAM and bandwidth quotas. How large that allocation is depends entirely on the plan type. On shared hosting you get a folder and a control panel. On a dedicated server you get an operating system of your choosing, root access and the ability to install anything the hardware supports.

Speed belongs in this section too, because it has a commercial edge. Search engines favor faster, more reliable pages, and every extra second of load time shows up as abandoned carts and lower ad revenue. The host you pick sets the floor on how fast your site can possibly be.

## Shared, VPS, cloud, dedicated: what changes between them

| Type | What is yours alone | Fits |
| --- | --- | --- |
| Shared | Nothing. Storage, bandwidth and processing are pooled with other sites | Blogs, brochure sites, first online store |
| VPS | A guaranteed share of CPU, RAM and disk on a shared physical machine, plus root | Sites outgrowing shared, custom software stacks |
| Cloud | Your site replicated across several machines, scaling with demand | Spiky traffic, ecommerce, international audiences |
| Dedicated | The entire physical machine | High traffic, compliance isolation, custom hardware needs |
| Reseller | A block of someone else's server that you sublet | Agencies reselling hosting |
| Managed | The same hardware, with the provider handling updates, security and backups | Teams with no sysadmin |
| Colocation | Your own hardware, sitting in someone else's rack | Companies that already own servers |

Shared hosting's weakness is structural. Another site on the same machine can spike and consume the CPU your checkout page needed, and you can't install software the host hasn't approved. AWS describes the tradeoff as leasing a coworking desk versus leasing the whole building: cheap and instant at the low end, constrained as you grow.

A VPS fixes the isolation problem without the full hardware bill. You get reserved resources and root access on a machine you still share, which puts server configuration, security patching and backups on your desk unless you pay for a managed layer.

Dedicated hosting removes the noisy neighbour entirely and introduces a different risk. One machine means one point of failure: if a component dies, your site is down until it's replaced, where a cloud setup routes around the failed node. Redundancy on bare metal is something you architect, not something the plan includes.

## When a whole server starts paying for itself

Answer yes to two or more of these and the $79 tier is a reasonable spend rather than an expensive toy:

- You need root and the freedom to install software the host doesn't support, such as a specific runtime, kernel module or daemon.
- Your traffic is steady enough that shared vCPU steal is visible in your own latency graphs, not just in theory.
- You move more than a few terabytes a month, where 30 TB of included transfer changes the economics.
- You need single-tenant hardware for a compliance scope or a client contract that forbids shared infrastructure.
- You run several sites, containers or virtual machines and want to consolidate them onto one bill.
- You need 10 Gbps ports for backups, media delivery or replication between machines.

The other direction matters more, because most readers searching for a hosting server are on the wrong side of this line. A WordPress blog with a few thousand monthly visits does not need 32 GB of RAM. A five-page business site does not need 30 TB of transfer. A developer who has never restored a broken bootloader should not start with bare metal unless they're prepared to learn on a production box. If any of that describes you, a $4 to $25 a month shared or cloud plan will serve you better, and you can revisit this in a year.

## What the money buys on either side of the line

Two reference points from the shared and cloud side, for scale.

Scaleway's hosting page lists a Mini plan at €3.99/month with one website, 1 GB SSD, 1 vCPU and 1 GB RAM, and an Advanced plan at €24.99/month covering up to 50 websites, 1,000 GB SSD, 16 vCPU, 64 GB RAM, a dedicated IP and automated backups. Both include SSL and support, run on cPanel, and come with a library of 420+ one-click application installs. Backups are an add-on at €2.99/month on the lower tiers.

GoDaddy's entry web hosting plan covers one website with 10 GB NVMe storage, a free domain, free email and a free SSL certificate with no renewal fee, plus daily backups, automated DDoS protection and a 30-day money-back guarantee. The company advertises up to twice the performance with its CDN and a 99.9% uptime guarantee; those are vendor claims rather than independent measurements.

SpinServers' entry Xeon sits at $79/month, which is $948 a year. Compared with a €3.99/month shared plan, that difference buys 4 dedicated cores, 32 GB of RAM, 1 TB of NVMe, 30 TB of monthly transfer and dual 10 Gbps ports. If your site can't use those resources, the gap is pure waste. If it can, the same money spent on a bigger shared plan buys you a bigger slice of a machine that still has neighbours.

The uptime commitment on these servers is published as a 99.99% SLA with a public status page, and the machines sit in Dallas and the Santa Clara area.

## Read this before you order

SpinServers' own knowledgebase is blunt about refunds: month-to-month services are not refundable, apart from SLA credits on a cancelled service. A refund may be granted at their discretion, and when one is approved the payment reversal can take up to 48 hours. There is no free trial and no free plan listed. If you're uncertain about network performance from your region, that uncertainty is worth resolving before you commit rather than after. 👉 [Check the entry dedicated server and its terms](https://bit.ly/Spinservers)

The rest of the pre-order checklist applies to any host, and the answers change what a plan really costs:

1. **SSL.** Included, or a paid certificate on top?
2. **Backups.** How often, how long are they retained, and is the service extra? Don't assume bare metal includes managed backups; on a dedicated server you usually own that process.
3. **Renewal pricing.** Compare the first-term rate with what you pay in year two. A cheap first year with an unlisted renewal is the most common hidden cost in hosting.
4. **Bandwidth overage.** What happens past 30 TB, and what does the extra terabyte cost?
5. **IP addresses.** How many are included, and what does an additional one cost per month?
6. **DDoS protection.** Standard on every plan, or a paid add-on?
7. **Location and latency.** Dallas and Santa Clara suit North American audiences. Visitors in Asia or Europe will see higher round-trip times.
8. **Support scope.** Who handles a failed disk at 3 a.m., and who handles a broken application config? Those are different tickets with different response times.
9. **Control panel.** cPanel or Plesk licensing is normally a separate cost on a dedicated machine. Confirm before you assume it's bundled.
10. **Upgrade path.** Can you move to the next tier without a rebuild and a migration?
11. **Domain.** Registered and renewed separately, at whatever the registrar charges.

## FAQ

**Is a domain the same thing as hosting?**
No. The domain is your address; hosting is the server that holds your files. You need both, they're bought from different places, and they're renewed on separate schedules.

**Do I need Linux skills to run a dedicated server?**
You need enough to install an OS, secure it, configure a web stack and recover it when something breaks. Managed hosting exists precisely because most site owners don't want that job.

**How do I know when shared hosting has to go?**
Watch three signals: page load times that climb as your traffic grows, resource-limit errors in your control panel, and plugins or services your host won't let you install. Two of the three showing up at once means it's time to move.

**How hard is migration?**
Easier than most people expect. Files, databases and DNS records are the whole job, and DNS propagation is the slow part at 24 to 48 hours. Plan the move for a low-traffic window and keep the old account active until the new one resolves cleanly.

## Choosing

Running a blog, a portfolio or a small store with no custom server software: stay on shared hosting, or move up to a small VPS when load times start slipping. You'll spend somewhere between €4 and €25 a month and get everything the site can use.

Running a site that needs root, single-tenant hardware, tens of terabytes of transfer, or a machine you can carve into several environments: the entry Xeon at $79/month is the cheapest sensible starting point, and the $235 and $390 tiers only make sense once you can name the workload that needs 40 or 56 cores.

Two last things to confirm before paying: the exact spec sheet in the cart, since pre-built stock rotates, and whether you're handling backups and server administration yourself or paying someone to do it. That second cost is the one people forget, and it's often larger than the hosting bill. 👉 [Compare the SpinServers dedicated configurations](https://bit.ly/Spinservers)
