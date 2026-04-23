# Customer app QA guide

**App version: v1.2.0**

Quick checklist for testing the KhayrEats customer app. Work through each section and tick off items as you go.

---

## What's new in v1.2.0

Use this section to test only the new features in this release. Each item links to the relevant full section below.

### Sold out label (see [Browse KhayrBoxes](#3-browse-khayreats-boxes))

- [ ] Find a box with no remaining stock
- [ ] Confirm it shows **"Sold out"** — not "0 left"

### Ingredients & allergens on reserve page (see [Order / checkout](#4-order--checkout))

- [ ] Open a box detail page and tap reserve
- [ ] Confirm there is a collapsible **"Ingredients & allergens"** section
- [ ] Tap it — confirm it expands and shows relevant content
- [ ] Tap again — confirm it collapses

### Reserve page spacing (see [Order / checkout](#4-order--checkout))

- [ ] Open the reserve page and confirm there is visible space above the box description / main text

### Orders page — restaurant name display (see [Order tracking](#5-order-tracking))

- [ ] Go to the orders tab
- [ ] Confirm restaurant names are not cut off or overflowing their container on any order card

### Orders page — unified view (see [Order tracking](#5-order-tracking))

- [ ] Confirm past and active orders appear in a single unified list (no separate tabs or sections required to switch between them)

### Orders page — empty state (see [Order tracking](#5-order-tracking))

- [ ] Use an account with no orders
- [ ] Confirm the empty state on the orders page matches the updated design

### Customer mark as picked up (see [Order tracking](#5-order-tracking))

- [ ] Place a test order
- [ ] Go to the orders tab and open the active order
- [ ] Confirm a **"Mark as picked up"** button is present
- [ ] Tap it — confirm the order moves to past orders

### Past orders show date (see [Order tracking](#5-order-tracking))

- [ ] Open the orders tab and scroll to past orders
- [ ] Confirm each past order shows the **actual date** (e.g. "Apr 20") — not "Tomorrow" or a relative label

---

## 1. Sign up / login

- [ ] Open app and confirm entry screen appears
- [ ] Sign up with valid details
- [ ] Ensure email verification triggers
- [ ] Login with verified account
- [ ] Test invalid email / password cases
- [ ] Test forgot password flow

---

## 2. Location

- [ ] Grant location permissions
- [ ] Confirm map loads and current location is shown
- [ ] Search for a pickup location and save it
- [ ] Verify KhayrBoxes update for the selected location

---

## 3. Browse KhayrBoxes

- [ ] View available boxes for today and tomorrow
- [ ] Scroll through the feed
- [ ] Search for boxes
- [ ] Open a box detail page
- [ ] Confirm details, restaurant info, price, and images
- [ ] Find a box with no stock remaining — confirm it shows **"Sold out"** (not "0 left")

---

## 4. Order / checkout

- [ ] Start order from box detail page
- [ ] Confirm there is visible space above the main text on the reserve page
- [ ] Confirm the **"Ingredients & allergens"** collapsible section is present on the reserve page
- [ ] Tap it — confirm it expands and shows content; tap again — confirm it collapses
- [ ] Verify checkout summary and pickup time
- [ ] Complete payment with a valid method
- [ ] Confirm order success message
- [ ] Check the order appears in history

---

## 5. Order tracking

- [ ] Open the orders tab
- [ ] Confirm active and past orders appear in a single unified list
- [ ] Confirm restaurant names on order cards are not cut off or overflowing
- [ ] On an account with no orders, confirm the empty state looks correct
- [ ] Open an active order and confirm tracking details
- [ ] Confirm the **"Mark as picked up"** button is present on an active order
- [ ] Tap "Mark as picked up" — confirm the order moves to past orders
- [ ] Check past orders show the actual date (e.g. "Apr 20") rather than a relative label like "Tomorrow"
- [ ] Test cancellation flow if available

---

## 6. Profile & settings

- [ ] Open profile page
- [ ] Update profile info and save
- [ ] Change password successfully
- [ ] Test account deletion flow if present

---

## 7. Feedback

- [ ] Find the feedback screen
- [ ] Submit a rating / comment
- [ ] Confirm submission success

---

## 8. Navigation / UI

- [ ] Use bottom navigation tabs
- [ ] Confirm the active tab highlights correctly
- [ ] Check that back navigation works
- [ ] Verify UI looks good on both phone and tablet sizes

---

## Release checklist

- [ ] Sign up / login works
- [ ] Location and map work
- [ ] Browsing and details work — sold out label shows correctly
- [ ] Reserve page has ingredients & allergens section and correct spacing
- [ ] Checkout and payment work
- [ ] Orders page: unified view, correct date labels, no restaurant name overflow
- [ ] Customer can mark order as picked up
- [ ] Empty state on orders page looks correct
- [ ] Profile settings work
- [ ] Feedback submission works
- [ ] App is usable on different screen sizes
