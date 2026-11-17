# Benic Global website: free hosting and connecting benicglobal.com

**What's free and what isn't.** The hosting below (Netlify, free plan) is free with no time limit. Renewing the domain is not: whoever registers benicglobal.com charges a yearly fee, usually about USD 10–20 a year. Cancelling Wix Premium does not cancel the domain itself. If Wix registered it, it stays at Wix until it expires.

---

## Step 0. Check where the domain is registered (1 minute)

1. Open https://lookup.icann.org and search for `benicglobal.com`.
2. Look at **Registrar** and **Expiration date**.
   - If it says **Wix.com Ltd.**, the domain is still with Wix. Log in to Wix, go to **Domains**, and check that it renews (or move it, see Step 4).
   - If it says GoDaddy, Namecheap or another company, log in there instead.
3. **Important about email:** operations@benicglobal.com must keep working. Before changing anything, find out who hosts that mailbox (Google Workspace, Microsoft 365, Zoho, or Wix mail). Write down its **MX records** from the domain's DNS settings, so they can be copied across.

## Step 1. Put the site online (5 minutes, free)

1. Open https://app.netlify.com/drop
2. Drag the whole **benicglobal** folder onto the page. You get a live link within seconds.
3. Click **Sign up / claim site** and register with **operations@benicglobal.com** (unclaimed sites are deleted after about an hour).
4. **Site configuration → Change site name** → `benicglobal`, so the address becomes benicglobal.netlify.app.

To update the site later: open the site in Netlify → **Deploys** → drag the folder in again.

## Step 2. Connect benicglobal.com

1. In Netlify: **Domain management → Add a domain** → enter `benicglobal.com` → confirm you own it.
2. Netlify shows the DNS records to add. Usually:
   - `A` record, host `@`, value `75.2.60.5`
   - `CNAME` record, host `www`, value `benicglobal.netlify.app`
   (Use the values Netlify shows you if they differ.)
3. Log in where the domain is registered (see Step 0; Wix: **Domains → ⋯ → Manage DNS records**). Delete the old Wix website records (the old `A` record for `@` and the `www` CNAME), then add the two records above. **Do not touch the MX records**, because they deliver your email.
4. Wait up to a few hours. Netlify then switches on HTTPS (the padlock) automatically.

## Step 3 (optional). Stop paying Wix markups for the domain

If the domain is registered with Wix, you can transfer it to a cheaper registrar such as Cloudflare Registrar or Namecheap when it's close to renewal. You'll need the transfer (EPP) code from Wix. A transfer includes one year of renewal.

## Step 4. Switch on the enquiry form

The form sends enquiries to hanna@benicglobal.com through FormSubmit, a free service that needs no account.

1. Once the site is live, send one test enquiry from the website.
2. FormSubmit emails hanna@benicglobal.com asking you to **Activate** the form. Click it.
3. Every enquiry after that arrives in that inbox as a neat table.

## Changing your details later

Open `index.html` in any text editor and search for `EDIT YOUR DETAILS HERE`. You can change the email, WhatsApp number, phone, address, Instagram handle and your trade licence number there. Leave the quote marks in place.

## Adding photos

The destination photos are free Unsplash photos, loaded straight from Unsplash, so there is nothing to upload. To swap one for your own photo, see `images/README.txt`.
