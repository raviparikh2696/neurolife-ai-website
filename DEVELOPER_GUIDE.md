# NeuroLife AI — Developer Guide: Tracking Contact Form Submissions

## How Contact Form Emails Work

When users fill out the contact form on the website and click "Send Message," the form opens their default email client with:

- **To:** ravi.parikh12345@gmail.com, dhruvdd6@gmail.com
- **Subject:** NeuroLife AI Contact Form - [Message Type] from [User Name]
- **Body:** Pre-filled with user's name, email, platform (iOS/Android), message type, and full message

Both developers receive the email directly in their inbox.

---

## How to Check & Organize Contact Form Emails

### Option 1: Gmail Labels (Recommended)

**Setup (One-time):**

1. Open Gmail
2. Go to **Settings** → **Labels** → **Create new label**
3. Create a label called `NeuroLife AI/Contact Forms`
4. Go back to **Settings** → **Filters and Blocked Addresses** → **Create a new filter**
5. In the "From" field, enter: `noreply@web3forms.com` (or leave blank to catch all contact emails)
6. In the "Subject" field, enter: `NeuroLife AI Contact Form`
7. Click **Create filter** → Check "Apply the label" → Select `NeuroLife AI/Contact Forms` → Click **Create filter**

**Now all contact form emails will automatically appear in the `NeuroLife AI/Contact Forms` label.**

### Option 2: Gmail Search

You can search for contact form emails anytime using:

```
subject:"NeuroLife AI Contact Form"
```

Or search by message type:

```
subject:"NeuroLife AI Contact Form - Bug Report"
subject:"NeuroLife AI Contact Form - Feature Request"
subject:"NeuroLife AI Contact Form - General Question"
subject:"NeuroLife AI Contact Form - Privacy / Data Request"
```

---

## Email Format Reference

**Subject Line Example:**
```
NeuroLife AI Contact Form - Bug Report from John Smith
```

**Email Body Example:**
```
Name: John Smith
Email: john@example.com
Platform: iOS (iPhone/iPad)
Message Type: Bug Report

Message:
The app crashes when I try to add a task with a very long title. I'm using iPhone 14 Pro with iOS 17.2.
```

---

## Responding to Users

1. **Reply directly** to the user's email address (shown in the email body)
2. **Reference the message type** in your response (e.g., "Thanks for reporting this bug...")
3. **Set expectations** — typically respond within 1–2 business days

---

## Organizing by Message Type

You can create separate labels for each message type:

- `NeuroLife AI/Bugs` — Bug reports
- `NeuroLife AI/Features` — Feature requests
- `NeuroLife AI/Questions` — General questions
- `NeuroLife AI/Privacy` — Privacy/data requests

Then create filters for each label using the subject line patterns above.

---

## Future Enhancement: Slack Webhook

If you want real-time notifications in Slack:

1. Create a Slack webhook URL in your workspace
2. Update the contact form to POST to the webhook instead of mailto
3. Slack will notify you instantly when a new message arrives

Contact the development team if you'd like to set this up.

---

## Summary

- **Emails go to:** ravi.parikh12345@gmail.com & dhruvdd6@gmail.com
- **Check emails in Gmail:** Search for `subject:"NeuroLife AI Contact Form"`
- **Organize:** Create labels like `NeuroLife AI/Contact Forms` for easy filtering
- **Respond:** Reply directly to the user's email address within 1–2 business days
