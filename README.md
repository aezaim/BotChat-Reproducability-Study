# BotChat-Reproducability-Study
The same repository was used in the paper and minimal changes were required to run the code.
In the app.py file,
In order to run the LLMs in studied in the report, use the following string representations for each LLM:
in this portion of the code in line 19,

hf_model_map = {
    'qwen-7b-chat-int4': HFChatModel('Qwen/Qwen-7B-Chat-Int4', system_prompt=default_system_prompt),
    'chatglm2-6b-int4': HFChatModel('THUDM/chatglm2-6b-int4', system_prompt=default_system_prompt),
}

For Qwen-14, 
change this line: 'qwen-7b-chat-int4': HFChatModel('Qwen/Qwen-7B-Chat-Int4', system_prompt=default_system_prompt),
with this line:  'qwen-14b-chat-int4': HFChatModel('Qwen/Qwen-14B-Chat-Int4', system_prompt=default_system_prompt),

Qwen-7B is provided to you by default.

For Vicuna 7-B, 
change this line: 'qwen-7b-chat-int4': HFChatModel('Qwen/Qwen-7B-Chat-Int4', system_prompt=default_system_prompt),
with this line: 'vicuna-7b-v1.5': HFChatModel('lmsys/vicuna-7b-v1.5', system_prompt=default_system_prompt),

#Using ChatGPT
To use GPT models, you need to provide your API key after you run the app.py. A gradio link website for BotChat will appear when you run the code and you can copy your API key for ChatGPT in the designated area. 

