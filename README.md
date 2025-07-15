# HomeMatch
HomeMatch is a futuristic AI powered search platform for home listings

## Functionalities
1. Generate listing description and neighborhood description using LLM (the initial data is on the `listings.cvs`)
2. Insertion of the generated text data on ChromaDB (Text Collection)
3. Collection of images to insert on the DB (Image collection) (the initial data is on the `./images`)
4. Collect user preferences on the UI and use those preferences to perform semantic search on the Vector Database
5. Use RAG to return the user search result, augmenting the description, tailoring it to resonate with the buyer’s specific preferences
6. **Bonus Feature**: Realtor ChatBot Assistant (When using this please click Enter to send the message) that is connected to an AI agent that allows
    * List all listings
    * Reserve a listing by ID
7. **Bonus Feature**: Multimodal search to search both on the text collections

## How to run the project

1. Install the necessary dependencies using the provided `requirements.txt`
2. Install `jupyter notebook`
3. Run all all the cells and wait for the localhost server to be launched
4. Interact the UI
5. Enjoy!

## Project Structure
```
homematch/
├── .gitignore              # Git ignore file
├── README.md               # Project documentation
├── requirements.txt        # Python dependencies
├── images/                 # File with the listing images to load later on the DB
├── listings.csv            # File to seed the LLM descriptions to later store on the DB
├── venv/                   # Virtual environment (excluded from version control)
└── HomeMatch.ipynb/        # Jupyter Notebook with the code
```

## Notes about the Multimodal search

The multimodal search takes into account the 0.8 of the text score and 0.2 of the image score.

That could be improved because text score will win most of the times and image score will be almost residual.

That could be improved by having a more specific user input to searh on the image collection.


## UI Screenshots

<img width="756" height="493" alt="Screenshot 2025-07-15 at 00 00 56" src="https://github.com/user-attachments/assets/77028265-0c0f-40e4-b60f-90c5b8f19f75" />
<img width="756" height="493" alt="Screenshot 2025-07-15 at 00 01 10" src="https://github.com/user-attachments/assets/a0879954-0afc-49df-a411-05b3a89dc357" />
<img width="756" height="493" alt="Screenshot 2025-07-15 at 00 03 06" src="https://github.com/user-attachments/assets/3a0a85ae-3697-4dd8-83e5-577beb06a2b3" />
<img width="756" height="493" alt="Screenshot 2025-07-15 at 00 03 19" src="https://github.com/user-attachments/assets/41d4caa5-e6b6-49f3-8e0e-25165098cef5" />

