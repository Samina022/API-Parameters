# API-Parameters
OpenAI Chat Completion API Parameters
# OpenAI Chat Completion API Parameters

This README file provides an explanation of the parameters used in the OpenAI Chat Completion API. These parameters allow you to customize the behavior and responses of the AI model. Examples are included to help you understand their practical applications.

---

## Parameters

### 1. **Messages**
**Description**: Contains the conversation history as a list of JSON objects, each specifying the role (`system`, `user`, or `assistant`) and the message content.

**Example**:
```json
[
  {"role": "system", "content": "You are a helpful assistant."},
  {"role": "user", "content": "What is the capital of France?"},
  {"role": "assistant", "content": "The capital of France is Paris."},
  {"role": "user", "content": "Tell me more about Paris."}
]
```

---

### 2. **Model**
**Description**: Specifies the AI model to use, such as `gpt-3.5-turbo` or `gpt-4`.

**Example**:
```json
"model": "gpt-4"
```

---

### 3. **Max Completion Tokens**
**Description**: Sets the maximum number of tokens the model can generate in a response.

**Example**:
```json
"max_tokens": 50
```
Limits the response length to 50 tokens.

---

### 4. **n**
**Description**: Specifies the number of response options to generate for each request.

**Example**:
```json
"n": 3
```
Generates three different responses.

---

### 5. **Stream**
**Description**: Boolean flag to indicate whether to stream the response back in parts or send it as a complete message.

**Example**:
```json
"stream": true
```
Enables real-time streaming of the response.

---

### 6. **Temperature**
**Description**: Controls the randomness of the responses. Values range from `0` (deterministic) to `2` (highly random).

**Example**:
```json
"temperature": 0.7
```
Produces moderately random and creative responses.

---

### 7. **Top_p**
**Description**: Uses nucleus sampling to consider only the most probable tokens up to a cumulative probability of `p`.

**Example**:
```json
"top_p": 0.9
```
Includes the most probable tokens whose cumulative probability is 90%.

---

### 8. **Tools**
**Description**: Specifies external functionalities or APIs the assistant can use, such as browsing, code execution, or image generation.

**Example**:
If tools like Python execution or browsing are enabled, the assistant can fetch real-time data or execute code.

---



