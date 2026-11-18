🍛 Rasoi Guide: Build Your Thali

An interactive web app where you build an Indian thali and chat with an AI assistant that talks only about Indian cuisine. Rasoi means kitchen.

Built for a topic-restricted chatbot assignment using Google AI Studio and the Gemini API.

Live demo: https://ai.studio/apps/f483fd64-0e3f-459b-8da4-d47abb17cbd9

Rasoi Guide screenshot

✨ Features
Tiffin intro: a steel tiffin box that opens into the builder.
Thali builder: drag dishes (rice, dal tadka, paneer butter masala, chole, aloo gobi, roti, raita, papad and more) onto a steel plate.
Prices, quantities and calories: every dish shows its price in ₹, portion size and approximate calories, with live totals.
Indian-food-only chatbot: ask for any Indian recipe, spice, technique, region or nutrition tip.
Smart refusals:
Indian dish → replies "Yes!" and gives the recipe.
Non-Indian dish (e.g. spaghetti, pizza) → says which cuisine it belongs to and suggests an Indian-style version.
Unrelated topics (coding, politics, sports) → politely declines.
Thali-aware answers: the bot knows what is on your plate, so you can ask "Is my thali balanced?".
Fast replies: streaming responses with an instant typing indicator.
Undo, start over and smooth animations.
🧠 How the chatbot stays on topic

The chatbot uses a detailed system instruction that gives it a clear role (a warm home-cook, food historian and patient teacher) and strict decision rules:

Indian dish or topic → confirm with "Yes!" and answer.
Non-Indian dish → name its origin, decline, and suggest an Indian-style version.
Indian-style version of a foreign dish (e.g. masala pasta) → answer with a recipe.
Anything unrelated to food → refuse politely in one or two lines.

The rules cannot be overridden by prompts like "ignore previous instructions".

🛠️ Tech stack
Part	Tool
App builder	Google AI Studio (Build mode)
AI model	Gemini API (@google/genai)
Frontend	React + Tailwind CSS
Fonts	Google Fonts

All tools used are free.

🚀 How to run
Open the live demo link above, or
Open the project in Google AI Studio, click Run, and use it in the preview.

To run your own copy, add your own Gemini API key in AI Studio. Never commit an API key to GitHub.

💬 Try these questions
Question	Expected result
"Recipe for dal makhani"	"Yes!" plus the recipe
"Why do we add hing to dal?"	A short explanation
"Is my thali balanced?"	An answer based on your plate
"Spaghetti recipe"	Says it is Italian and suggests an Indian-style version
"Indian-style pasta"	"Yes!" plus a masala pasta recipe
"Write a Python program"	Polite refusal
📚 What I learned
Writing system instructions with a clear role and strict rules.
Keeping a chatbot on one topic, including against prompt-injection attempts.
Improving response speed with streaming and shorter context.
Designing a polished, readable interface with AI-assisted building.
⚠️ Note

Calories and quantities are approximate home-style estimates and are meant for demonstration only. For medical diets, consult a doctor or dietitian.

👩‍💻 Author

Velaga Divya Deepika 3rd-year B.Tech, Computer Science (AI) GitHub: velaga-deepu
