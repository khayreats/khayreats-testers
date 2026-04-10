# Restaurant app QA guide

Testing guide for the KhayrEats restaurant app. Work through each section in order for a full sign-up to order flow test.

---

## 1. New restaurant sign-up

### Step 1: account creation

- [ ] Enter restaurant name, email, phone, password
- [ ] Password confirmation matches
- [ ] "Next" button works → goes to step 2

### Step 2: business details

- [ ] Enter IBAN (bank account)
- [ ] Enter commercial registration number
- [ ] Select food category from dropdown
- [ ] "Next" button works → goes to step 3

### Step 3: logo & terms

- [ ] Upload restaurant logo (image picker works)
- [ ] Check "I agree to terms" checkbox
- [ ] "Create Account" button works → goes to location setup

### Step 4: location setup

- [ ] Google Maps loads
- [ ] Search for address or select on map
- [ ] Confirm location → goes to waiting page

### Step 5: waiting for approval

- [ ] Shows "pending approval" message
- [ ] Can't access dashboard until admin approves

---

## 2. Login & authentication

- [ ] Valid email / password → goes to dashboard
- [ ] Wrong credentials → shows error
- [ ] Customer account → redirected to customer app
- [ ] Pending restaurant → stays on waiting page
- [ ] Suspended restaurant → shows suspension message

---

## 3. Dashboard

- [ ] Loads for approved restaurants only
- [ ] Shows restaurant name and logo
- [ ] Bottom navigation: Dashboard | Orders | Profile
- [ ] Quick links to manage orders and boxes

---

## 4. Order management

### Active orders

- [ ] Shows list of pending orders
- [ ] Each order shows: customer name, phone, box name, price, pickup time
- [ ] Tap order → goes to details page
- [ ] "Mark as Picked Up" button works
- [ ] After marking → order moves to past orders

### Past orders

- [ ] Shows completed orders
- [ ] Same info as active orders
- [ ] Historical data loads correctly

### Order details page

- [ ] Shows full order info
- [ ] Customer phone number is clickable to call
- [ ] "Mark as Picked Up" → confirmation dialog appears
- [ ] Confirm → status changes to completed

---

## 5. KhayrBox management

### View all boxes

- [ ] Shows list of restaurant's boxes
- [ ] Each box shows: title, description, image, pickup times, status, price
- [ ] "Create New Box" button → starts creation flow

### Create new box

**Step 1: size**

- [ ] Choose Small / Medium / Large
- [ ] "Next" → goes to step 2

**Step 2: description**

- [ ] Enter title and description
- [ ] Upload image
- [ ] "Next" → goes to step 3

**Step 3: schedule**

- [ ] Select days of week (Sun–Sat)
- [ ] Set pickup start / end times
- [ ] Set max daily boxes
- [ ] "Next" → goes to step 4

**Step 4: review**

- [ ] Shows all entered info
- [ ] "Publish" → creates box
- [ ] Box appears in list as "Active"

### Edit box

- [ ] "Edit" button on box card
- [ ] Same 4-step flow with pre-filled data
- [ ] Save changes → updates box

### Deactivate box

- [ ] "Deactivate" button → confirmation dialog appears
- [ ] Confirm → box becomes inactive
- [ ] Removed from active list

---

## 6. Restaurant profile

### View profile

- [ ] Shows: name, logo, email, phone, IBAN (masked), category
- [ ] Account status shows correctly (Approved / Pending / Suspended)

### Edit profile

- [ ] "Edit Profile" button works
- [ ] Can update any field (name, email, phone, etc.)
- [ ] Can change logo
- [ ] Save → updates profile

### Other features

- [ ] "Manage Khayr Boxes" link → goes to box management
- [ ] Language selector (EN / AR) works
- [ ] Logout button → goes to login

---

## 7. Error scenarios

- [ ] Invalid email format → validation error shown
- [ ] Passwords don't match → error message shown
- [ ] Image upload fails → retry option appears
- [ ] Try to access dashboard when pending → blocked
- [ ] Mark order picked up twice → no crash
- [ ] Create box with missing required fields → validation triggered

---

## 8. Integration checks

- [ ] Orders from customers appear in restaurant app
- [ ] Profile changes save to database
- [ ] Images upload to Firebase correctly

---

## Release checklist

- [ ] Sign-up flow works end to end
- [ ] Login and authentication work
- [ ] Dashboard loads correctly
- [ ] Orders can be viewed and marked as picked up
- [ ] KhayrBoxes can be created, edited, and deactivated
- [ ] Profile can be viewed and updated
- [ ] Error states are handled gracefully
- [ ] Integration with customer app and database works

---

*Last updated: April 2026*
