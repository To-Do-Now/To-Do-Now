# To Do Now GPT – Quick Start

---

## STEP 1  Create your Airtable base (free)

1. Click this template → <https://airtable.com/apph0Zh9pD0zbaqFT/shrFWh6cuQnOanNVS>  
2. Click **Use this data** (top-right). Airtable will prompt you to sign up—email only, no card needed. Save the template as your base.

---

## STEP 2  Generate one Personal Access Token (PAT)

1. Open a new tab → <https://airtable.com/create/tokens>  
2. **Create token** → name it *To-Do-Now*  
3. Under **Scopes**, add/select these three scopes for your token: `data.records:read` · `data.records:write` · `schema.bases:read`  
4. Under **Access** pick the Airtable base you just created from the template and saved to your Airtable account → **Create token**. Copy the token and save it somewhere safe (it's only provided once).

---

## STEP 3 Tell the GPT your two codes so it can access your Airtable base

| Code                              | Where to find it                                             |
| --------------------------------- | ------------------------------------------------------------ |
| **Base ID** (`appXXXXXXXXXXXXXX`) | Open the base you just created. <br>Look at your browser’s address bar — you’ll see `https://airtable.com/appXXXXXXXXXXXXXX/tbl…` <br>Copy everything from the **a** in `app` up to the next slash. |
| **Token** (`patXXXXXXXXXXXXXX`)   | After you press **Create token** in STEP 2, Airtable shows a long string starting with **pat** — copy it. |

Paste the two lines back in the GPT — press **Enter** after each:

```text
BASE_ID: appXXXXXXXXXXXXXX
TOKEN:   patXXXXXXXXXXXXXX
```

You’ll see **✅ Airtable linked!**

---

## STEP 4  Add a task in the GPT **or** paste your full To Do List.

### ✏️  One task (example)

```
Add "Buy groceries" – 30 min Due-soft once a week
```

### 📋  Whole list (example)

```
Pay rent – 5 min due 1st of the month
Vacuum – 20 min repeat weekly
Paint fence
```

*What happens next?*  

1. The GPT imports each line.  
2. If a duration or priority is missing it can **estimate** and asks follow-ups.  
3. You confirm, and the tasks are stored in your Airtable base.

## How duration estimation works

* If you supply a duration, the GPT uses it.  
* If you leave it blank, the GPT calls an **Estimate Duration** tool under the hood. 
  * High-confidence result → stored immediately.  
  * Low confidence (< 50 %) → GPT asks you “About how many minutes will this take?”  
* Either way, the final value is saved, so future suggestions are usable.

## 🗂️ How priorities work 

| Level | Label            | Plain meaning                                           |
| ----: | ---------------- | ------------------------------------------------------- |
| **1** | **Overdue-hard** | A hard deadline that’s already missed. Highest urgency. |
| **2** | **Overdue-soft** | A “nice to have” deadline that’s already missed.        |
| **3** | **Due-hard**     | A non-missable deadline in the future.                  |
| **4** | **Due-soft**     | A flexible deadline in the future.                      |
| **5** | **If-free**      | Responsible but non-urgent chores.                      |
| **6** | **Would-love**   | Fun or wish-list items you can choose if you want.      |

To assign a priority, you can type either the **word** (e.g., `Due-soft`) or the **number** (`4`). The GPT will always show the word back to you.

---

## STEP 5 Get your next task

```
I have 25 minutes
```

The GPT lists the best-fit task (or bundle) based on priority, deadline, and your available time.

---

## STEP 6  Ask for help anytime in the GPT

```
Read quick-start guide
help
tutorial
```

