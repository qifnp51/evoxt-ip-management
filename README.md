# Evoxt IP Management Complete Guide: How to Assign, Swap, and Add Floating IPs on Your VPS — Plus All Plans, Pricing, and Promo Codes Compared

Running multiple VPS servers is one of those things that sounds straightforward until you actually have to manage IP addresses across them. Which server is which? What happens when you need to move production traffic to a standby box? Can you migrate without your users noticing downtime?

These are real questions, and Evoxt built an IP management system specifically to deal with them. If you've been hunting for a VPS provider that gives you proper IP control without buried settings or support tickets for every small task, this is worth reading.

---

## What Is Evoxt IP Management?

Evoxt is a Malaysia-based VPS hosting provider founded in 2020. Beyond the high-frequency CPUs they're known for, Evoxt includes a built-in IP address management toolset with every account — no extra subscription, no tier lock. The system handles four core operations directly from the VM control panel:

- **Assign IPv4** — attach an extra IP to a specific virtual machine
- **Reassign IPv4** — move an IP currently on one server to another
- **Set as Primary IP** — promote a secondary IP address to become the server's main address
- **Remove IPv4** — detach an IP from a server so it can be reassigned elsewhere
- **Swap IPv4 between VMs** — exchange IP addresses between two of your virtual machines

The Swap IP feature is the one most users end up caring about. It lets you exchange the IP addresses between a development server and a live production server in a few clicks — which means you can test a full environment migration before flipping the switch, and then flip it with minimal downtime.

👉 [Get started with Evoxt and access IP management tools free](https://bit.ly/Evoxt)

---

## How to Access the IP Management Panel

Everything lives inside the VM control panel. Once you're logged in:

1. Navigate to your VM's control panel
2. Click **IP Management** in the top navigation bar
3. You'll land on the Assign IP tool by default

From there you can toggle between Assign IPv4 Tools and Swap IPv4 Tools. The interface is clean — each option is labeled and there are GIF demos on the IP management feature page walking you through the motions.

One thing to note: **IP assignments trigger an automatic server reboot.** Evoxt's system handles the configuration side automatically after reboot (no manual network config changes needed), but you'll want to save any temporary work on the server before initiating any IP action.

Also, IPs can only be assigned from the same region. If you need to move a server to a different region entirely, that requires a support ticket.

---

## Floating IPs and Extra IP Addresses

Beyond the IP swapping tools, Evoxt lets you order additional IP addresses for each VM. The pricing is straightforward: **$3/month per extra IP address**, and you can order up to **5 extra IPs per virtual machine**.

This is useful when you're running multiple services on a single server and want to separate them at the network layer — different IPs for a web server and a mail server on the same VM, for example, or running multiple SSL certificates without SNI complications.

The extra IP ordering process is automated, so there's no wait time for provisioning. Once ordered, the IP shows up in your control panel and can be assigned, swapped, or set as primary just like any other address.

> **Practical use case:** You're running a live production website on VM-A. You've set up VM-B as an upgraded replacement. With Evoxt's Swap IP feature, you can point the production IP to VM-B in a few clicks, test that everything's working, and if something goes wrong, swap back just as fast. No DNS propagation delays, no extended downtime window.

---

## Why IP Management Matters for VPS Users

A lot of budget VPS providers treat IP management as an afterthought — you get one IP, it's tied to the server, and moving it requires opening a ticket and waiting. Evoxt made it a panel feature from early on because the use cases are common:

**Development-to-production transitions** — swap the live IP to a freshly configured server without reconfiguring DNS or waiting for propagation.

**Failover setups** — if a primary server has an issue, point the IP to a standby in seconds.

**Multi-site setups** — assign multiple IPs to a single server, each handling different domains or services.

**Infrastructure reorganization** — reassign IPs as you scale up or consolidate servers without disrupting the addresses your users or services depend on.

The fact that all of this is included at no extra charge (aside from the $3/month per additional IP) puts Evoxt ahead of a lot of providers who either don't offer it or make you email support every time.

---

## All Evoxt VPS Plans and Pricing

Evoxt runs three regional tiers with different bandwidth allocations. The CPU, RAM, and storage specs are identical across tiers — what changes is how much monthly transfer you get, reflecting the higher transit costs in premium network regions.

### Standard Network (US, UK, Canada, Germany, Poland, Amsterdam, Japan Tokyo, Malaysia, Australia)

| Plan | CPU | RAM | Storage | Monthly Transfer | Price | Deploy |
|------|-----|-----|---------|-----------------|-------|--------|
| VM-0.5 | 1 core (up to 6.0 GHz) | 512 MB | 5 GB NVMe | 500 GB | $2.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-0.75 | 1 core (up to 6.0 GHz) | 1 GB | 10 GB NVMe | 750 GB | $4.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-1 | 1 core (up to 6.0 GHz) | 2 GB | 20 GB NVMe | 1000 GB | $5.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-1.5 | 2 cores (up to 6.0 GHz) | 2 GB | 20 GB NVMe | 1500 GB | $6.95/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-2 | 2 cores (up to 6.0 GHz) | 4 GB | 30 GB NVMe | 2000 GB | $11.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-3 | 4 cores (up to 6.0 GHz) | 4 GB | 30 GB NVMe | 3000 GB | $14.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-4 | 4 cores (up to 6.0 GHz) | 8 GB | 60 GB NVMe | 4000 GB | $23.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-6 | 8 cores (up to 6.0 GHz) | 8 GB | 60 GB NVMe | 5000 GB | $29.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-8 | 8 cores (up to 6.0 GHz) | 16 GB | 80 GB NVMe | 6000 GB | $47.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-12 | 16 cores (up to 6.0 GHz) | 16 GB | 80 GB NVMe | 8000 GB | $60.95/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-16 | 16 cores (up to 6.0 GHz) | 32 GB | 100 GB NVMe | 10 TB | $95.99/mo |  [Deploy](https://bit.ly/Evoxt) |

### Premium Network (Hong Kong, Japan Osaka)

Same specs as Standard, with reduced bandwidth allocations (250 GB on VM-0.5, scaling up to 5 TB on VM-16). Hong Kong includes CN2 network optimization for better mainland China connectivity.

| Plan | Monthly Transfer | Price | Deploy |
|------|-----------------|-------|--------|
| VM-0.5 | 250 GB | $2.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-1 | 500 GB | $5.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-2 | 1000 GB | $11.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-4 | 2000 GB | $23.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-8 | 3000 GB | $47.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-16 | 5000 GB | $95.99/mo |  [Deploy](https://bit.ly/Evoxt) |

### Premium Plus Network (Malaysia Premium)

Higher-tier network infrastructure, slightly tighter bandwidth allocations than Standard.

| Plan | Monthly Transfer | Price | Deploy |
|------|-----------------|-------|--------|
| VM-0.5 | 150 GB | $3.49/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-1 | 300 GB | $5.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-2 | 600 GB | $11.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-4 | 1000 GB | $23.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-8 | 2000 GB | $47.99/mo |  [Deploy](https://bit.ly/Evoxt) |
| VM-16 | 4000 GB | $95.99/mo |  [Deploy](https://bit.ly/Evoxt) |

All plans run on a 1 Gbps port. All plans include weekly automatic offsite backups at no extra charge.

---

## Add-On Pricing

Beyond the base plans, Evoxt lets you add individual resources without upgrading your whole plan:

| Add-On | Cost |
|--------|------|
| Extra IP address | $3/month per IP (max 5 per VM) |
| Extra vCPU core | $3/month per core |
| Extra RAM | $2/month per GB |
| Extra bandwidth (Standard) | $3/TB |
| Extra bandwidth (Premium) | $12/TB |
| Extra bandwidth (Premium Plus) | $24/TB |

This a la carte approach is genuinely useful if you're close to a bandwidth limit but don't need more CPU or RAM. Instead of jumping to a bigger plan, you just buy the extra transfer.

---

## Promo Codes and Current Discounts

The most widely reported recurring discount code right now is **EVOXT595**, which applies a **40% recurring discount** to VM-1 plans and above. That means the $5.99/month VM-1 effectively drops to around $3.59/month — and that discount stays every billing cycle, not just the first month.

Another code circulating across coupon sites is **BHW595**, reported to work similarly. The VM-0.5 entry plan at $2.99 is not eligible for percentage-based promo codes but is already the lowest entry price in Evoxt's lineup.

To apply a code: choose your plan → configure the server → proceed to checkout → enter the promo code in the "Promotional Code" field → hit Apply. The discount reflects immediately before payment.

Evoxt also supports billing cycles from monthly up to 3 years, with longer commitments offering further savings. If you're confident in the product, locking in for a year with the recurring promo code stacked on top makes the math look pretty good.

👉 [Browse Evoxt plans and apply your promo code at checkout](https://bit.ly/Evoxt)

---

## What Else Is Included With Every Plan

The IP management system doesn't sit in isolation — it's part of a broader control panel that Evoxt has built out over the years:

- **VNC browser access** — manage your server even if SSH is down
- **Layer 3 firewall** — set rules before traffic reaches your VM, handled at the network level
- **VM cloning** — duplicate a configured server without reinstalling from scratch
- **API access** — automate server management through Evoxt's documented API
- **One-click app installs** — WordPress, Docker, GitLab, Nextcloud, cPanel, Minecraft, and more
- **Weekly offsite automatic backups** — included in every plan, no upsell
- **Sub-accounts** — manage users and access permissions within your account

On the network side, Evoxt owns its own ASN (AS149440), which gives them direct control over routing. For Asian-market traffic in particular, this tends to translate into better peering and lower latency than providers routing through resellers.

---

## Who Should Use Evoxt

The IP management features and overall platform make the most sense for:

**Developers managing multiple environments** — staging, development, and production servers where IP swapping saves time during deploys.

**Small businesses running several services** — assign different IPs to different services on the same or separate VMs, keep things organized without complexity.

**Users targeting Asian markets** — the Hong Kong and Japan Osaka Premium Network locations with CN2 optimization serve this case well.

**Anyone running WordPress, game servers, or self-hosted tools** — Evoxt's high single-core CPU frequency (up to 6.0 GHz turbo) benefits these workloads more than extra cores at slower speeds.

**Budget-conscious users who want actual features** — the included backups, firewall, IP management, VNC, API, and clone tools would cost extra at a lot of comparable providers.

---

## Final Thoughts

Evoxt's IP management isn't flashy. It's a practical set of tools — assign, swap, set primary, remove — that covers the situations where you'd otherwise be opening a support ticket and waiting. The fact that it's included at no extra cost and works without any server-side configuration changes (just a reboot) makes it a genuinely useful feature rather than a marketing checkbox.

The extra IP pricing at $3/month per address is fair. The ability to swap IPs between VMs for failover or migration scenarios is the kind of thing that saves real time when you actually need it.

If you're comparing VPS providers and IP flexibility is on your list, it's worth factoring in that Evoxt has this built in from the start.

👉 [Start with Evoxt — plans from $2.99/month, IP management included](https://bit.ly/Evoxt)
