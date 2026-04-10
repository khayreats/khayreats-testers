# Customer app QA guide

Quick checklist for testing the KhayrEats customer app. Work through each section and tick off items as you go.

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

---

## 4. Order / checkout

- [ ] Start order from box detail page
- [ ] Verify checkout summary and pickup time
- [ ] Complete payment with a valid method
- [ ] Confirm order success message
- [ ] Check the order appears in history

---

## 5. Order tracking

- [ ] Open the orders tab
- [ ] View current and past orders
- [ ] Open an active order and confirm tracking details
- [ ] Check order status updates
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
- [ ] Browsing and details work
- [ ] Checkout and payment work
- [ ] Order history and tracking work
- [ ] Profile settings work
- [ ] Feedback submission works
- [ ] App is usable on different screen sizes
