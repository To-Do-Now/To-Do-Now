# To Do Now GPT – Quick Start

---

## STEP 1	Create your Airtable base (free)

1. Click this template → <https://airtable.com/apph0Zh9pD0zbaqFT/shrFWh6cuQnOanNVS>  
2. Click **Use this data** (blue button, top-right)
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
Add "Buy groceries" - 30 min Due-soft once a week
```

### 📋  Whole list

```
Pay rent - 5 min due 1st of the month
Vacuum - 20 min repeat weekly
Paint fence
```

The GPT will:

1. Check each task for missing info (duration or priority)
2. Show you any estimates it makes
3. Wait for your OK before saving to Airtable

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
Add "Call mom" - 15 min Due-soft
Add "Team meeting tomorrow at 2pm"
```

---

## 🎯 Example Session

```
You: I have 30 minutes
GPT: With 30 minutes, you could:
     A. Call dentist (15 min) - Due-soft (4)
     B. File receipts (20 min) - If-free (5)
     
     Reply: done, skip, or add task

You: done a
GPT: ✅ Marked "Call dentist" as done.
     
     With 15 minutes left, you could:
     B. File receipts (20 min) - If-free (5)
     C. Water plants (10 min) - Would-love (6)
```

---

## ⏱️ Duration Tips

- Include time when adding tasks: `Paint fence - 2 hours`
- If you skip it, the GPT will estimate and ask you to confirm
- Durations help the GPT suggest tasks that fit your available time

---

## 🗂️ Priority Levels (1-6)

**Urgent stuff** → 1 Overdue-hard | 2 Overdue-soft | 3 Due-hard | 4 Due-soft  
**Regular stuff** → 5 If-free | 6 Would-love

Just use the number (1-6) or the word (Due-soft). The GPT handles the rest.

---

## 💡 Good to Know

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
