# To Do Now GPT – Quick Start (~ 3 min)

---

## STEP 1  Create your Airtable base (free)

1. Click this template → https://airtable.com/apph0Zh9pD0zbaqFT/shrFWh6cuQnOanNVS  
2. Press **Copy base** (top-right). Airtable will prompt you to sign up—email only, no card needed; your data.

---

## STEP 2  Generate one token

1. Open a new tab → <https://airtable.com/create/tokens>  
2. **Create token** → name it *To-Do-Now*  
3. Under **Scopes**, add/select these three scopes for your token: `data.records:read` · `data.records:write` · `schema.bases:read`  
4. Under **Access** pick the Airtable base you just copied from the template and added to your Airtable account → **Create token**.

---

## STEP 3 Tell the GPT your two codes do it can access your Airtable base

| Code | Where to find it |
|------|------------------|
| **Base ID** (`appXXXXXXXXXXXXXX`) | Open the base you just copied. <br>Look at your browser’s address bar — you’ll see `https://airtable.com/**appXXXXXXXXXXXXXX**/tbl…` <br>Copy everything from the **a** in `app` up to the next slash. |
| **Token** (`patXXXXXXXXXXXXXX`) | After you press **Create token** in STEP 2, Airtable shows a long string starting with **pat** — copy it. |

Paste the two lines back in ChatGPT — press **Enter** after each:

```text
BASE_ID: appXXXXXXXXXXXXXX
TOKEN:   patXXXXXXXXXXXXXX
```

You’ll see **✅ Airtable linked!**

---

## STEP 4  Add a task in the To Do Now GPT

```
Add "Buy groceries" – 30 min **Due-soft** once a week
```

*(Priority words you can use later: Overdue-hard · Overdue-soft · Due-hard · Due-soft · If-free · Would-love)*  

---

## STEP 5  Ask for help anytime in the To Do No GPT

```
Read quick-start guide
```

The GPT will show this page again inside the chat window.
