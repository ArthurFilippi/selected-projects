# X-HEC Hackathon: customer feedback intelligence for a casino

*Winning project, X-HEC Hackathon. Team project.*

## Challenge

A casino wants to better exploit its customers' feedback in order to:

1. identify **urgent problems** that need immediate solutions;
2. better **engineer the customer experience**.

## Approach

- Collection of all customer feedback and pre-processing.
- A first text-processing pass to extract high-level features (customer sentiment, themes, friction points).
- The processed feedback feeds a RAG, so that a casino manager can run **semantic search with sourced references**.
- An executive dashboard presents the results: themes grouped by customer-journey step, volumes of appreciated elements and frictions, and the underlying verbatims.

## What is in this folder

The code snapshot in [`code`](code) is the **dashboard** of the team repository: a Streamlit application and a React frontend, with the aggregated, theme-level data it displays (`data.json`, `journey.json`; text in French). To my reading, the RAG and semantic search components are not part of that repository snapshot.

- `code/Dashboard/dashboard.py`, `data_loader.py`: Streamlit application (Plotly, pandas).
- `code/Dashboard/frontend`: React 19, TypeScript, Vite, Tailwind CSS 4 and Recharts (treemap, bar charts, verbatim table, customer-journey view).
- `code/data.json`, `code/journey.json`: aggregated themes with counts and descriptions, and the customer-journey structure.

To run it, see `code/Dashboard/README.md`: `pip install -r requirements.txt` then `streamlit run dashboard.py` for the Streamlit version, and `npm install` then `npm run dev` in `frontend` for the React version.

## Credits

Original repository: [simonvielpeau/hackathon-x-hec](https://github.com/simonvielpeau/hackathon-x-hec). Commits by Simon Vielpeau and a teammate (GitHub handle `yboady`). The code is shown here as a snapshot of that repository (commit `b24466e`), without its committed virtual environment. All credit for the shared code goes to the team.

My contribution: *[to be completed]*

We won the hackathon, and got so many ElevenLabs credits!
