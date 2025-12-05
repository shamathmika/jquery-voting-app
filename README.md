# Studio Ghibli Food Voting App

A cozy, Studio-Ghibli-inspired interactive food voting web app.  
Built with **HTML**, **CSS**, **jQuery Mobile**, and a custom **slide-up modal**.  
Swipe, click arrows, or use keyboard keys to vote on foods, then view your results in a whimsical **storybook layout**.

## Features

- Beautiful Ghibli-styled UI and colors  
- Swipe left/right to vote (mobile + desktop)  
- Keyboard support (← = dislike, → = like)  
- Clickable food thumbnails  
- Results displayed as a **storybook with left/right pages**  
- Slide-up bottom modal with:
  - Food image (happy/sad depending on vote)
  - Heart / broken heart icon
  - Custom Ghibli-style lore text  
- Automatic animations and transitions  
- Works locally without a backend  

## Project Structure
```
/
├── index.html
└── images/
    ├── Pizza.png
    ├── Pizza-sad.png
    ├── Sushi.png
    ├── Sushi-sad.png
    ├── Pasta.png
    ├── Pasta-sad.png
    └── ...etc for all foods
```

Each food requires **two images**:

- `Food.png` → the normal (liked) image  
- `Food-sad.png` → the sad version (used when disliked)  

## How to Run

### Option 1: Open Directly (Chrome workaround needed)
Because Chrome blocks some script behaviors on `file://` pages:

1. Try opening `index.html` directly.
2. If modal or navigation breaks, use Option 2.


### Option 2: Run a Local Web Server (recommended)

#### **Python 3**
```bash
python3 -m http.server

```
Then open:
```
http://localhost:8000/
```

Node.js (using http-server)
```
npm install -g http-server
http-server
```

Then visit:
```
http://localhost:8080/
```
VS Code Live Server Extension

1. Install "Live Server" extension
2. Right-click index.html → Open with Live Server

## Controls
### Voting
- Swipe left → Dislike
- Swipe right → Like
- Click left/right arrow buttons
- Keyboard shortcuts:
  - Left Arrow → Dislike
  - Right Arrow → Like

## Results Page
Click any food to open a slide-up modal with:
- Full image
- Heart / broken heart
- Ghibli-style description

## Add or Change Foods
To add a new food:
- Add two images inside /images:
  ```
  FoodName.png  
  FoodName-sad.png
  ```
- Add lore text in foodLore inside index.html:
  ```
  "NewFood": "Ghibli-style text here."
  ```
- The app automatically picks it up.

## Demo:
https://github.com/user-attachments/assets/b7c52ab5-1b17-42ab-a5c5-500c901473da
