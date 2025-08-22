
# **MbendeStay Real Estate Platform – Application Outline**

## 1. **Overview**

MbendeStay is a real estate platform based in Cameroon that connects **property seekers (tenants)** with **property owners (landlords/agents)**. It covers **all regions of Cameroon**, with advanced filtering by **region → division → subdivision → city**, as well as **price range, duration of stay, and property type**.
Access to property details and communication features is **subscription-based** for both tenants and landlords.

---

## 2. **Core User Roles**

1. **Guest User (unregistered)**

   * Can browse limited listings with blurred/hidden details.
   * Cannot view full property information or contact landlords.
   * Prompted to **subscribe** or **register**.

2. **Tenant (Subscriber)**

   * Registers and subscribes to access property details.
   * Can view landlord info, property details, amenities, reviews.
   * Can **chat directly with landlords**.
   * Can leave **reviews & ratings**.
   * Can **report landlords** for misconduct (e.g., charging visitation fees).

3. **Landlord / Property Owner (Subscriber)**

   * Must **verify identity** (KYC: ID, phone number, email, utility bill, etc.).
   * Pays a **subscription fee** to list properties for a set duration.
   * Can manage property details (price, location, amenities, images, videos).
   * Must upload **video walkthroughs** for contract signing.
   * Can communicate with tenants via chat.

4. **Admin (Platform Management)**

   * Manages users, subscriptions, and payments.
   * Approves property listings based on **strict rules**.
   * Moderates chats and reviews.
   * Manages reports (fraud, fake listings, illegal activities).
   * Generates analytics and revenue reports.

---

## 3. **Platform Features**

### 3.1 Property Search & Filtering

* Search by **Region → Division → Subdivision → City**.
* Filters: **price range, duration of stay (daily, weekly, monthly, yearly), property type (apartment, studio, villa, hostel, shared room, etc.), amenities (Wi-Fi, parking, AC, furnished, etc.)**.
* Search results for non-subscribers show only:

  * Basic description
  * Blurred images
  * Hidden landlord contacts

### 3.2 Subscriptions & Access Control

* **Tenant Subscription**: Required to view full property details and contact landlords.
* **Landlord Subscription**: Required to list properties (packages by duration & number of listings).
* Subscription packages may include:

  * **Tenant Plans**:

    * *Daily Access* – 1,000 XAF
    * *Monthly* – 5,000 XAF
    * *3 Months* – 12,000 XAF
    * *6 Months* – 20,000 XAF
  * **Landlord Plans**:

    * *Single Property – 1 Month* – 5,000 XAF
    * *Up to 5 Properties – 3 Months* – 20,000 XAF
    * *Unlimited Listings – 6 Months* – 50,000 XAF

(Pricing adjustable by Admin)

### 3.3 Property Listing (Landlords)

* **Required Fields:**

  * Property title
  * Region → Division → Subdivision → City
  * Exact location (hidden from unsubscribed users)
  * Price (daily, weekly, monthly, yearly)
  * Amenities (multi-select)
  * Images (min. 3 high-quality photos)
  * Video walkthrough (mandatory before signing contract)
  * Availability status

* **Identity Verification (KYC):**

  * ID card / Passport upload
  * Phone verification (OTP)
  * Email verification

### 3.4 Tenant Features

* **Chat with Landlords** (in-app messaging).
* **Reviews & Ratings** after staying at a property.
* **Report Landlords** (e.g., for charging visitation fees, fraud, fake property).
* **Save Favorites** for quick access.
* **Guide to Visit Property**: Free visits must be allowed. If fees are requested, tenants can report.

### 3.5 Chat & Communication

* **One-to-one chat** between tenant and landlord.
* Tenants can only initiate chat **after subscription**.
* **Admin moderation tools** to review suspicious chats.

### 3.6 Video Confirmation Before Contract

* For every rental contract, the landlord must upload a **video walkthrough** showing the exact condition of the property.
* Tenants confirm the property matches the listing before signing.

### 3.7 Rules & Moderation

* No duplicate listings.
* No fake images or misleading pricing.
* No visitation fees allowed.
* Only verified landlords can post.
* Properties must fall under approved categories (no illegal buildings or unsafe housing).
* Repeated offenders get banned.

---

## 4. **Technical Modules**

### 4.1 Authentication & Security

* Email & phone OTP verification.
* Two-factor authentication (optional).
* Role-based access control (tenant, landlord, admin).
* Encrypted chats.
* Secure payments (MTN Mobile Money, Orange Money, PayPal, Credit/Debit Card).

### 4.2 Payment & Billing

* Integrated payment gateway supporting:

  * **Mobile Money (MTN, Orange)**
  * Bank cards
* Auto-renew subscription option.
* Admin dashboard for revenue tracking.

### 4.3 Admin Panel

* User management (block, verify, delete).
* Subscription management.
* Property approval workflow.
* Fraud detection and reports management.
* Analytics (active tenants, landlords, revenue, most searched areas).

### 4.4 Notifications

* Email & SMS alerts for subscription expiry.
* Push notifications for:

  * New property matches.
  * Chat messages.
  * Tenant reviews.
  * Expiring subscriptions.

---

## 5. **Scalability & Future Enhancements**

* Multi-language support (**English, French**).
* AI-powered property recommendations.
* Virtual tours with 360° images.
* Integration with legal e-signature for rental agreements.
* Referral program for tenants and landlords.

---

## 6. **System Flow (Summary)**

1. **Tenant Flow:**
   Register → Subscribe → Browse & Filter → View Property → Chat with Landlord → Visit Property (free) → Confirm via Video → Sign Contract → Leave Review

2. **Landlord Flow:**
   Register → Verify Identity → Subscribe → List Property → Admin Approval → Tenants Contact via Chat → Video Walkthrough for Contract → Rental Completed

3. **Admin Flow:**
   Approve Listings → Verify Landlords → Manage Subscriptions → Handle Reports → Generate Reports
