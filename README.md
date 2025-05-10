# 🤖 AI Assistant: User Info Collector (with Streaming + Tool Calls)

This project demonstrates a smart **AI Assistant** built using the **OpenAI Agent SDK**. It collects user information like name, age, gender, and country by **calling tools one-by-one** with **real-time streamed output** in the terminal.

---

## 🔍 Context Concept Highlight

In this project, we use a powerful feature of the OpenAI Agent SDK: **Context Passing**.

```python
@dataclass
class UserInfo():
  name : str
  age : int
  gender : str
  country : str

🧰 **Tool-Based Information Retrieval**  
Calls the following tools, one at a time:
- `fatch_user_name`
- `fatch_user_age`
- `fatch_user_gender`
- `fatch_user_country`

🔄 **Real-Time Streaming**  
Uses `Runner.run_streamed()` to stream agent messages and tool outputs directly in the terminal.

🗣️ **Catchy & Polite Responses**  
The assistant uses a friendly, multi-line, and polite tone as instructed.

---

## 📦 Technologies Used

- **Python 3.10+**
- **OpenAI Agent SDK**
- **Asyncio for real-time streaming**

---

## 🧪 How It Works

### 🧾 Prompt:
```text
please provide all about user info
