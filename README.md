# 🎓 AI Agent: Student Course Enquiry Assistant (n8n + Twilio + Airtable + OpenAI)

## 🚀 Try It Out!
This **n8n workflow** template provides a smart and automated **Course Enquiry Assistant** that communicates over SMS.

It demonstrates how AI Agents can:
- Understand a database schema,
- Plan their response logic,
- Generate Airtable queries autonomously, and
- Communicate effectively with users through Twilio.

> 💡 [Explore the Example Airtable Course Database »](https://airtable.com/appO5xvP1aUBYKyJ7/shr8jSFDaghubDOrw)

---

## 🔧 How It Works

1. **Twilio Trigger**  
   - Incoming SMS is captured via a webhook and passed into the workflow.

2. **AI Agent Execution**  
   - The user’s question is forwarded to the AI Agent.
   - The agent is trained to use the **Airtable database** for referencing course data.

3. **Agent Planning & Querying**  
   - It first inspects the Airtable schema.
   - It then formulates a `filter_by_formula` query to fetch relevant data.

4. **Search & Respond**  
   - The agent analyzes results and generates a suitable reply.
   - All responses are logged in a secondary Airtable sheet.

5. **Twilio Response**  
   - The final response is sent back to the user via SMS.

---

## 💬 Example Questions

Try asking the agent:
- _“Which courses are available on Wednesday mornings?”_
- _“Are there any courses taught by Professor Lee?”_
- _“I’m interested in Creative Arts. What options do I have?”_

---

## 📦 Requirements

| Tool      | Purpose                              |
|-----------|--------------------------------------|
| Twilio    | SMS communication (webhook + reply)  |
| OpenAI    | LLM-powered Agent & query planning   |
| Airtable  | Course database backend               |
| n8n       | Workflow orchestration               |

---

## 🔨 How to Use

1. Clone or import this workflow into your n8n instance.
2. Set your **Twilio phone number** to point to your n8n webhook URL.
3. Ensure your **OpenAI** and **Airtable** credentials are set in n8n.
4. Update the Airtable base with your courses (or any relevant data).
5. Start texting your Twilio number to see it in action!

---

## ⚙️ Customization

- Replace **Airtable** with **PostgreSQL**, **MySQL**, or other databases.
- Extend the AI Agent with new tools (e.g., calendar lookup, internal API access).
- Log queries for lead generation or feedback loops.
- Modify prompt templates to suit a different use case (e.g., Inventory Assistant, HR Bot).

---

## 🧠 Example Use Cases

- University/College Course Recommendation
- Career Counseling Bots
- Campus Enquiry Systems
- Corporate Training Schedule Assistant

---

## 🙋 Need Help?

- 🧵 [Join n8n Discord](https://discord.com/invite/XPKeKXeB7d)
- 🛠️ [Ask the n8n Community](https://community.n8n.io/)

---

## 🧑‍💻 Author

**Sagar Zujam**  
B.Tech CSE Student • NCER Pune  
AI, Data Science, and Cybersecurity Enthusiast  
[LinkedIn](https://www.linkedin.com/) | [GitHub](https://github.com/)

---

> 🧪 Built using: `n8n`, `OpenAI`, `Twilio`, `Airtable`

