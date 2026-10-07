# HireHustle — C2C job autopilot · Setup & User Guide

![HireHustle](https://raw.githubusercontent.com/eswarkalla/job-outreach-app/main/banner.jpg)

HireHustle finds C2C / contract roles that match your resumes, mails the recruiter from **your own Gmail** with
the best resume (retitled to the role), follows up, and tracks every reply, RTR, submission and call — all on
your own Mac.

> 👋 **Built by Eswar Kalla.** If this app helps you, please **follow me on LinkedIn**:
> **https://www.linkedin.com/in/eswarakalla** — I post updates, new features and C2C job-search tips there.

---

## 🎁 Free trial: 3 working days, everything unlocked

- Install and set up for free. Your trial starts the **first time you press Start**: full features, no mail limit,
  for **3 working days** (Mon–Fri, US Eastern; weekends don't count; a start after noon counts from the next day).
- **One trial per Mac and per email.** Starting it needs internet once and registers this Mac's ID and your Gmail
  address with the HireHustle trial server. Changing Gmail accounts, reinstalling or deleting the app doesn't
  start a new trial.
- When it ends, your data stays; mails pause until you buy a license.

## 🔄 Stays working by itself
- Every few hours the app checks in with the HireHustle server and receives **fixes** (for example when LinkedIn or
  TextNow change their pages), announcements and license status. No mail contents, names or addresses are sent:
  only the Mac's ID, app version, plan, today's counts and short problem notes with personal details removed.
- A license needs internet at least **once every 30 days**.
- If a version has a serious problem, the app asks you to update and pauses sending until you do.

## 💳 Price: $199 one-time

- One license = one Mac, yours forever, including all updates. No monthly fee.
- **To buy:** message **Eswar on WhatsApp: +1 845 253 9604** (https://wa.me/18452539604) with your **Machine ID**
  (HireHustle → Settings → License → Copy). The **💬 Buy on WhatsApp** button writes the message for you.
- **Coupons:** ask on WhatsApp. Coupons look like **`PAVI` + 3 letters + the discount**, e.g. `PAVIKQX50` = 50% off
  (25%, 50%, 75% or 100%). Your coupon is **emailed to you**, works **only for your email address**, once, for 30 days.
  Send the code, your Machine ID and that email on WhatsApp.
- After payment you get a **license key** (starts with `JOL1-`) on WhatsApp → paste it in **Settings → License → Activate**.
- After the free trial, mails stay paused until you activate (your data is kept).
- By activating you accept the **license agreement** (personal use on one Mac; no copying, sharing, reselling or reverse-engineering).

| Coupon | You pay |
|---|---|
| none | $199.00 |
| 25% off | $149.25 |
| 50% off | $99.50 |
| 75% off | $49.75 |
| 100% off | $0 (free) |

---

## 1. Before you start (what you need)

| Need | Why | How to get it |
|---|---|---|
| A Mac with Apple Silicon (M1/M2/M3/M4…), macOS 13 or newer | The app runs on your own Mac | Apple menu > About This Mac shows the chip |
| Gmail with **2-Step Verification** on | Mails go out from your own Gmail | https://myaccount.google.com/security |
| A Gmail **App Password** | Lets the app send and read mail | https://myaccount.google.com/apppasswords → create one called "HireHustle" |
| Gmail **IMAP on** | To read replies | Gmail > Settings > See all settings > Forwarding and POP/IMAP > Enable IMAP |
| Your resumes (.docx or .pdf) | Attached to each mail | One per kind of role works best (e.g. Data Engineer, AI/ML Engineer) |
| Optional: Claude Code or an Anthropic API key | Tailored resumes, reply drafts, Ask assistant, interview prep | https://claude.com/claude-code (then `claude auth login`) |
| Optional: Google Chrome | LinkedIn capture and TextNow calling (add-on) | — |
| Optional: TextNow account | Click-to-call and caller pop-up | https://www.textnow.com |

---

## 2. Install (one time, about 3 minutes)

1. Download **JobOutreach-macOS.zip** from **https://github.com/eswarkalla/job-outreach-app/releases/latest**
   (no GitHub account needed).
2. Double-click the zip, then drag **HireHustle.app** into your **Applications** folder.
3. Open it. The first time, macOS may say it "can't verify the developer": click **Done**, then go to
   **System Settings → Privacy & Security**, scroll down and click **Open Anyway** next to HireHustle (once only).
4. **Activate:** Settings → **License** → copy your Machine ID → **💬 Buy on WhatsApp** → when you get your key,
   tick **I accept the license agreement**, paste the key → **Activate**.

> Your data (mails, resumes, database, calls) lives only on **your** Mac in
> `~/Library/Application Support/JobOutreach`. Updates replace the app, never your data.

---

## 3. First-time setup (the Welcome checklist)

The Dashboard shows a green **Welcome** card until these are done. Click **Open** next to each item.

0. **Free trial / License:** your 3-working-day trial starts when you press **Start**; activate a license any time in Settings → License.

1. **Settings → About you:** your name, phone, availability. (Your LinkedIn URL is only used when you choose to send it — it's never added to mails automatically.)
2. **Settings → Gmail:** your Gmail address and the 16-letter App Password → click **Test Gmail login**.
   - **Always CC:** anyone who should be copied on every mail (e.g. your employer/manager).
   - **Your employer / bench-sales contacts:** your employer's team, so RTRs they handle are tracked and you never double-submit.
3. **Settings → Job search:** the roles you want (e.g. "Data Engineer, Azure Data Engineer, AI Engineer") and skills.
4. **Resumes tab → Upload resume:** add each resume. Use **Test the matching** to see which resume fits a sample job.
5. **Settings → Your answers:** your rate, work authorization, location/relocation, availability, interview availability. Reply drafts use **only** these facts (anything missing becomes `[fill in: …]`).
6. **Settings → Sending hours:** default 8 AM–6 PM US Eastern, weekdays.
7. **Settings → Claude (optional):** choose Claude Code or API key → **Test Claude**.
8. Press **Start** (bottom-left). Automation keeps running even when you close the window. **Quit** stops it.

### Chrome add-on (optional, recommended)
1. Open `chrome://extensions` → turn on **Developer mode** (top right).
2. In HireHustle: **LinkedIn tab → Show the add-on folder**. In Chrome click **Load unpacked** and choose that folder
   (`~/Library/Application Support/JobOutreach/chrome-extension`). After app updates, click ↻ **Reload** on the add-on.
3. Pin it. While you scroll LinkedIn, posts with recruiter emails are sent to the app; on TextNow it dials and shows the caller card.

---

## 4. Everyday use

- Open the app in the morning and press **Start** if it's off.
- Check **Dashboard → Waiting for your answer** and **Follow-ups**.
- Check **Daily report** for your numbers and the **Call list**.
- Answer recruiters (use the reply **Draft** button), log calls, and note RTRs.
- An **8 AM morning brief** arrives by email/notification: who's waiting on you, interviews, new vendor mails.

---

## 5. Features, tab by tab

### Dashboard
- Live tiles: first mails today (vs your daily cap), follow-ups, vendor first responses (today / overall), queue, interviews.
- **Follow-ups card:** *Due now / Upcoming / In queue*, grouped by day (Today, Yesterday, older).
  - Today's follow-ups go out by themselves; older ones wait for you — **Send group / Skip group** or pick rows.
  - **Pause / Resume** all follow-ups with one button.
- **Daily limit reset:** if you hit the daily first-mail cap, click **Reset count & continue**; the whole day's total is still tracked.

### Where jobs come from
- **nvoids.com** — watched continuously; **today's nvoids roles are always sent first**. Hotlists ("I have an excellent consultant available…") are excluded automatically. If nvoids is down, the app heals itself and catches up.
- **corptocorp.org** — public feed every 30 min.
- **Your inbox** — requirement mails vendors send you (answered in their thread).
- **LinkedIn** — via the Chrome add-on or copy-paste. Job **seekers** and bench/hotlist posts are filtered out; only real openings get your resume.

### What happens to each job
1. Skills are matched against each resume; the best one is picked (ties go to the resume with the better reply rate).
2. The resume title and file name are changed to the job's title; optionally Claude tailors it.
3. The mail is personalised: recruiter's first name, role-specific pitch, A/B-tested subject and opening, unique subject per recruiter (so Gmail never mixes threads).
4. Duplicate guard: no second mail to the same recruiter for the same role; no submission your employer already made.
5. Up to 2 follow-ups in the same thread if there's no reply.

### Mails, Pipeline, Replies, Opportunities
- **Mails:** every thread with status; click a row for the full story.
- **Pipeline:** who's waiting on you and where each lead stands (replied → RTR → submitted → interview).
- **Replies:** what recruiters wrote, with **✍️ Draft a reply** (never sent without your OK; ID numbers are never written).
- **Opportunities:** requirements vendors mailed you.

### Submissions (RTRs & submissions)
- RTR / Right to Represent / Rate confirmation mails are captured automatically — from vendors **and** your employer's team.
- **One conversation = one RTR**, counted on the day it started; client, rate and location are merged from the thread.
- **Duplicate warning** if the same client/role was already submitted by someone else.
- Rate tracker: your rates vs market by role family.

### Daily report
- **Call list** with its own search (name, company, phone) — repliers first; signature details (name, org, phone) from their replies are shown.
- First mails within sending hours, follow-ups, applied online (per site), RTRs & submissions, vendor first responses (one per vendor per day, 7 AM–9 PM ET), calls, goals and streak, note for the day.
- **Download Excel** of the whole day.

### Calling (TextNow)
- Click **Call** → TextNow opens and dials the number.
- **Caller card** (inside the app, draggable): role they're calling about, location, organization, how many times they've called, talking points.
- After each call: **We talked / No answer**, or **Log later**. Missed calls go to a **call-back list** with a reminder and a **Text back** option (you confirm before it sends).
- Call stats on the Daily report.

### Stats & insights
- Reply rate by resume, role, source; when people reply; A/B test results.
- **Vendor quality score** (warm vendors are prioritised), **skill-gap report**, **hot-lead alert** (90%+ match with a phone number).
- **Weekly report** + **Monday review** by email.

### Applied online
- Applications you made yourself on LinkedIn, Dice, ZipRecruiter etc. are detected from confirmation mails and counted per site.

### Ask (assistant)
- Ask anything about your data: "How many RTRs this week?", "Who called me today?", "What should I do now?".
- Action buttons (draft reply, log call, pause sending…) always ask for confirmation. Voice input, charts, Excel export.

### Interview prep
- When a thread reaches Interview, Claude writes a one-page prep sheet from the job post, the resume you sent and the recruiter's messages (also emailed to you).

### Contacts, Jobs, Resumes
- **Contacts:** every recruiter found, searchable by name/email/phone.
- **Jobs:** every post the app has read and why it was or wasn't mailed.
- **Resumes:** upload, see matches, test matching.

### Remote viewing (optional)
- View the app from your phone through a private Tailscale link with a password. Pause/Resume need your PIN.

---

## 6. Rules the app always follows

- Never puts your location, work authorization or LinkedIn in mails automatically.
- Never sends a reply, text or message without your confirmation.
- Never writes passport / SSN / visa / license numbers in drafts.
- Stays within Gmail's safe sending limits (follow-ups pause first so new roles keep going).

---

## 7. Updates

**Settings → App version & updates → Check for updates → Update now.** The newest version downloads and the app
reopens by itself in a few seconds. Your data is never changed.

---

## 8. Troubleshooting

| Problem | Fix |
|---|---|
| "Gmail login failed" | Re-create the App Password; make sure IMAP is on and there are no spaces. |
| Nothing is sending | Is **Start** on? Is it inside sending hours? Is the daily cap reached (use **Reset count & continue**)? |
| Claude features not working | Settings → Claude → **Test Claude**. If you hit a usage limit, it resumes by itself later. |
| LinkedIn posts not captured | Reload the add-on in `chrome://extensions`, refresh LinkedIn, scroll slowly. |
| TextNow doesn't dial | Reload the add-on; keep one TextNow tab open and signed in. |
| App window won't open | Quit it (right-click the Dock icon → Quit), open it again. Log: `~/Library/Application Support/JobOutreach/server.log`. |
| "Can't verify the developer" | System Settings → Privacy & Security → **Open Anyway** (first open only). |
| New Mac | Your license works on one Mac; message on WhatsApp for a key for the new Mac. |

---

### 🤝 Stay connected
If HireHustle saved you time, **follow me on LinkedIn: https://www.linkedin.com/in/eswarakalla** — and share
it with friends who are job hunting.
