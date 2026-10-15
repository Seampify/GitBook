---
description: >-
  When you're inside Meta Commerce Manager (after logging in), you'll see three
  options under "Add Items". These determine how you upload products to your
  catalog:
---

# Catalog Item Upload Options

## 1. ✅ **Add Manually** _(Recommended for most users)_

**What it is**:\
You enter product details one-by-one via a form.

**Use when**:

* You have a small number of products.
* You want full control over each item.
* You’re testing or starting out.

**What you’ll enter**:

* Product name
* Description
* Image URL or upload
* Price
* Inventory
* Product condition
* Product link (optional)

🟢 _Best for Seampify users with under 50–100 products._

***

## 2. 📥 **Use Data Feed**

**What it is**:\
Upload a bulk file (CSV, TSV, or XML) that contains all your product details.

**Use when**:

* You have many products (hundreds or thousands).
* You want to manage the catalog from a spreadsheet.
* Your data comes from an eCommerce platform (e.g., Shopify, WooCommerce).

**Common fields in the file**:

* `id`, `title`, `description`, `price`, `availability`, `image_link`, `link`, etc.

📌 You can also set up scheduled fetches from a hosted file (e.g., Google Sheets or Dropbox).

***

## 3. 🧠 **Use Meta Pixel** _(Advanced / Developers only)_

**What it is**:\
Automatically pulls product info from your website using the Meta Pixel + microdata on your product pages.

**Use when**:

* You run an eCommerce site with many dynamic product pages.
* You want the catalog to update in real time based on site changes.

**Requires**:

* Facebook Pixel installed on your website.
* Proper metadata setup using [Open Graph](https://ogp.me/) or [Schema.org](https://schema.org/).

🟡 _Useful for developers or advanced setups, not necessary for Seampify-only use._

***

### 🔍 Which Should You Use for Seampify?

> 💡 **Choose “Add Manually”** unless:

* You manage your products in a spreadsheet (then use **Data Feed**).
* You run a complex online store (then explore **Meta Pixel**).
