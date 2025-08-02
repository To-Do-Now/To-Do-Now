# To Do Now GPT – Quick Start

---

## STEP 1	Create your Airtable base (free)

1. Click this template → <https://airtable.com/apph0Zh9pD0zbaqFT/shrFWh6cuQnOanNVS>  
2. Click **Use this data** (top-right)
3. Sign up with just your email (no credit card)
4. Give your base a name and click **Create base**

---

## STEP 2	Generate one Personal Access Token (PAT)

1. Open a new tab → <https://airtable.com/create/tokens>  
2. **Create token** → name it *To-Do-Now*  
3. Under **Scopes**, click **+ Add a scope** and check these 3 boxes:
   ☐ data.records:read
   ☐ data.records:write  
   ☐ schema.bases:read
4. Under **Access** pick the base you just created → **Create token**
5. Copy the token immediately (you only see it once!)

---

## STEP 3	Tell the To Do Now GPT your two codes

| Code        | Where to find it                                             |
| ----------- | ------------------------------------------------------------ |
| **Base ID** | Open your base. Look at the address bar: `https://airtable.com/appXXXXXXXXXXXXXX/tbl…` <br>Copy from **app** to the next slash. |
| **Token**   | The long code starting with **pat** that you copied in STEP 2. |

Paste both lines into the To Do Now GPT chat exactly like this:

```text
BASE_ID: appXXXXXXXXXXXXXX
TOKEN:   patXXXXXXXXXXXXXX
```

You'll see **✅ Airtable linked!**

---

## STEP 4	Add tasks

### ✏️  One task

```
Add "Call dentist" Due-soft
```

*The GPT will estimate this takes about 15 minutes*

### 📋  Whole list

```
Pay rent Due-hard 1st
Call dentist Due-soft
Vacuum repeat weekly
Paint fence
Clean bathroom
```

The GPT will:

1. Automatically estimate task durations using AI
2. Show you the time estimates for confirmation
3. Save everything to your Airtable base

---

## STEP 5	Get your next task

```
I have 25 minutes
```

The GPT finds tasks that fit your time and priority.

---

## 📝 Common Commands

**Managing tasks:**

```
done               Mark current task complete
skip               Skip for today (reappears tomorrow)  
delete Paint fence Delete a specific task
list               Show all your tasks
search 30 min      Find tasks by time, name, or priority
```

**Working with time:**

```
I have 45 minutes  Get task suggestions that fit
I have 2 hours     Shows multiple options if available
```

**Quick adds:**

```
Add "Call mom" Due-soft
Add "File taxes" Due-hard April 15
Add "Team meeting tomorrow at 2pm"
Add "Paint bedroom" - 3 hours      (include duration if you want)
```

---

## 🎯 Example Session

```
You: I have 30 minutes
GPT: With 30 minutes, you could:
     A. Pay bill (10 min) - Due-hard (3)
     B. Call dentist (15 min) - Due-soft (4)
     C. File receipts (20 min) - If-free (5)
     
     Reply: done, skip, or add task

You: done a
GPT: ✅ Marked "Pay bill" as done.
     
     With 20 minutes left, you could:
     B. Call dentist (15 min) - Due-soft (4)
     C. File receipts (20 min) - If-free (5)
```

---

## ⏱️ Smart Duration Estimates

- The GPT can automatically estimate how long tasks will take 
- Just paste your tasks and it figures out the timing
- You can include your own duration if you prefer: `Paint fence - 2 hours`
- Either way, durations help match tasks to your available time

---

## 🗂️ Priority Levels (1-6)

**Hard vs Soft deadlines:**

- **Hard** = firm deadline with real consequences (rent due, tax filing)
- **Soft** = flexible target date you'd prefer to hit (call friend, paint room)

**Urgent stuff** → 1 Overdue-hard | 2 Overdue-soft | 3 Due-hard | 4 Due-soft  
**Regular stuff** → 5 If-free | 6 Would-love

Just use the number (1-6) or the word (Due-soft). The GPT handles the rest.

---

## 💡 Good to Know

**AI-powered features:**

- Automatically estimates task durations
- Intelligently suggests tasks based on your available time
- Learns common task patterns for better estimates

**Import limits:** 

- 25 tasks at a time (for easy confirmation)
- 300 new tasks per day maximum

**Recurring tasks:**

- Use "repeat weekly" or "every 7 days"
- Completed recurring tasks auto-create the next one

**Task selection:**

- When you get multiple options (A, B, C), reply with the letter
- Type "skip" to see more options

**Can't find something?**

- Search is your friend: `search paint` or `find urgent tasks`

---

## STEP 6	Ask for help anytime

```
help
```

---

## 🔧 Quick Fixes

**"Airtable seems unavailable"** → Wait 60 seconds and try again  
**Wrong duration on a task?** → Say `update Paint fence to 3 hours`  
**Need to start over?** → Type `delete all` (requires confirmation)

---

✅ **You're in control**

- Your tasks stay in YOUR personal Airtable base 
- Only you can access your data
- You can disconnect anytime by revoking your Airtable token
- The To Do Now GPT simply connects you to your own task storage
- By using this tool, you acknowledge that you control your own data
