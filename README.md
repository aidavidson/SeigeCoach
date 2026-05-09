# SeigeCoach

Description: this tracker will look at player stats, and current match information based on data of game strategy operators are suggested to players, along with weapons fitting their ability, after observing past data and current data suggestions are made to fix playstyle, bad habits, and game sensitivity for the player so they can progress in the game. This feature will of course be prevented to be used in ranked as it is a training software not intended to get AI help cheating ranked games 


## What needs to be stored

- Videos of Gameplay
- keystrokes/ controller inputs (maybe at certain times e.g. death/kill …
  - Video of player hand movements
- Actual Stats

Needed info
- Player Stats
  - Kills with certain operators
  - Best maps
  - Best weapon kills
  - Ranked round wins based on operator and map
- Current match data
  - Operators that are on your team
  - Operators owned by the player
  - Current map
  - attack/defense
- Past matches
  - Recoil pattern with different weapons
  - Utility use
  - Drone usage
  - Cause of death
    - Run out
      - Use AI to see if opponent is out of the building
    - Spawnpeak
      - Use AI to see where player was shot from
    - Gunfight
      - Swing/Swung
      - Player misses shots and computer sees so
    - Wallbang
      - Player is shot through wall preemptively

# R6 API
## Basic unchangeable stats useful for strategy
https://r6data.eu/api-docs#base-url 

## Player data
https://r6.tracker.network/r6siege/profile/xbl/Chancesavitar/overview 
https://tracker.gg/developers/docs/getting-started 

# AI analysis
- Google AI Studio — widely considered the best free AI API available. You get access to Gemini 2.5 Pro and Flash with no credit card required. The API is also OpenAI-compatible, so it's easy to plug into existing code. Awesome Agents
Other solid free options:
- Groq — free access to open-source models like Llama with extremely fast inference. No credit card needed for the free tier. DEV Community
- OpenRouter — lets you try 400+ models with one API key, including free tiers for models like DeepSeek and Llama. AIMLAPI
- Puter.js — a unique "user-pays" model where you can access GPT models from your frontend with no API key at all, and users cover their own usage costs. Puter

## Computer Vision
Computer Vision is Crucial to analyze how the player is moving and playing for future suggestions

To use AI API access and computer vision (CV) for game data analysis, you must capture visual frames from the game, process them through a CV model or API, and then analyze the extracted metadata to derive insights. This process is used across physical sports for tactical analysis and video games for botting or strategic coaching. [1, 2, 3, 4, 5]

Core Implementation Workflow
- Data Capture: Capture game footage via screen recording, direct webcam feed, or high-speed cameras.
- Preprocessing: Use libraries like OpenCV to resize, filter, or normalize images to make them readable for AI models.
- Analysis via AI APIs or Models:
- Cloud APIs: Use services like Google Cloud Vision API or AWS Rekognition for high-level object and text detection (OCR).
- Custom Models: Deploy models like YOLO (You Only Look Once) via the TensorFlow Object Detection API to track specific entities like players, balls, or UI elements in real-time.
- Metadata Extraction: Convert visual detections into structured data, such as coordinates, player speeds, or in-game stats like health and gold.
Strategic Analysis



