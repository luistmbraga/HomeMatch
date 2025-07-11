# HomeMatch
HomeMatch is a futuristic AI powered search platform for home listings

## Functionalities
1. Listing description and neighborhood description using LLM (the initial data is on the `listings.cvs`)
2. Insertion of the generated data and the initial data on ChromaDB
3. Collect user preferences on the UI and use those preferences to perform semantic search on the Vector Database
4. Use RAG to return the user search result, augmenting the description, tailoring it to resonate with the buyer’s specific preferences
5. **Bonus Feature**: Realtor ChatBot Assistant that is connected to an AI agent and allows to list all listings and reserve a listing (When using this please click Enter to send the message)

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
├── venv/                   # Virtual environment (excluded from version control)
└── HomeMatch.ipynb/        # Jupyter Notebook with the code
```
