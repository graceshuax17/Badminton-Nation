# Badminton-Nation

## Run the prototype

Open `index.html` directly in a browser. No install, server, framework, or backend is required.

## How recommendations work

The questionnaire collects 12 answers and scores every racket in the JavaScript database. The weighted categories total 100%:

- Playing style: 20%
- Skill level: 15%
- Weight: 10%
- Balance: 15%
- Flexibility: 10%
- Playing type: 10%
- Swing speed: 10%
- Budget: 5%
- Priority: 5%

Exact matches receive full points, compatible/nearby matches receive partial points, and poor matches receive zero. Priority uses each racket's power, speed, and control ratings. A matching brand preference contributes an additional 5-point preference bonus. The top three final percentages are displayed with explanations.

Purchase links in the prototype point to Amazon search results for each racket model, so the recommendations can open directly to a retailer page when the user clicks a buy button.

## Add a racket

Add another object to the `racketDatabase` array in `index.html`. Keep the same fields as the existing records: `name`, `brand`, `price`, `weight`, `balance`, `flexibility`, `skill`, `playingType`, `style`, `swingSpeed`, `power`, `speed`, `control`, and `purchaseUrl`. The scoring and display code will include it automatically.