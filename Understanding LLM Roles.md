## Understanding System, User, and Assistant Messages in LLMs

When working with Large Language Models (LLMs), you usually need to structure your input into **different types of messages**. The three common roles are:

### 1. **User Message**

* Represents the input or query from the end-user.
* Example:

  ```
  User: Translate "I love football" into French.
  ```

### 2. **System Message**

* Defines the **rules or behavior** of the model.
* Example:

  ```
  System: You are a professional translator. Always translate text into French.
  ```

### 3. **Assistant Message**

* Controls the **tone or style** of the response.
* Example:

  ```
  Assistant: Always reply in a casual and friendly way.
  ```

---

### Combined Example

```
System: You are a professional translator. Always translate text into French.  
Assistant: Use a casual and friendly tone.  
User: I love football.
```

**Model’s output →**

```
J’adore le foot !
```

---

## Agents vs. Chains

When building applications with LLMs, you will often hear about **Agents** and **Chains**.

### Chains

* A **Chain** is a simple pipeline:

  * You give the model some input → it produces an output.
* It usually doesn’t remember anything from past interactions.
* Example:

  ```
  Input: "Summarize this paragraph."
  Output: "This text is about..."
  ```

### Agents

* An **Agent** is more advanced:

  * It can decide what tools or actions to use before giving you the final answer.
  * It usually has **memory**, so it can remember previous interactions.
* Example:

  ```
  User: My name is Alex.
  (later)  
  User: What’s my name?
  Agent: Your name is Alex.
  ```

---

### Key Takeaways

* **System** → sets the rules and behavior.
* **User** → provides the actual input.
* **Assistant** → controls response style.
* **Chain** → simple request → response, no memory.
* **Agent** → smarter, can use tools and memory.
