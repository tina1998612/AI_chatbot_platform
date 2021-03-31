# AI_chatbot_platform

Backend: https://github.com/EasonC13/AI_chatbot_platform

Front-end: https://github.com/EasonC13/AI_Chatbot_website

(Please Checkout Dev Branch)

Demo Video: https://youtu.be/ES2mmcrhS10

# How To Run?

0. install dependency:

```
pip install -r requirement.txt
```

1. copy app/core/config_example.py to app/core/config.py and Edit the config file.

```
cp app/core/config_example.py app/core/config.py
```

2. Use the following command to run it:

```
cd app
uvicorn app:app --port {API_PORT} --host 0.0.0.0 --workers 8
```

3. Bulid front-end
If you want use front-end as well. 
Please [clone front end from another GitHub Repo](https://github.com/EasonC13/AI_Chatbot_website) at root.

```
cd AI_chatbot_platform
git clone https://github.com/EasonC13/AI_Chatbot_website.git
mv AI_Chatbot_website front-end
```

And then go inside it and build it. (Recommand Demo Branch since we havn't merge it.)

```
cd front-end
git checkout demo
npm i
npm run build
```
