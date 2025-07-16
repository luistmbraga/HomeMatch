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

## Udacity review and feedback

### Additional References

<img width="951" height="709" alt="Screenshot 2025-07-15 at 15 06 16" src="https://github.com/user-attachments/assets/a56d34fe-ef9d-4ba5-9807-ea5519e094f7" />
<img width="1023" height="206" alt="Screenshot 2025-07-15 at 15 06 23" src="https://github.com/user-attachments/assets/62005b3c-03fa-43f3-b00d-4e7183ca6022" />


Retrieval-Augmented Response Generation for Knowledge-Grounded Conversation

https://ieeexplore.ieee.org/document/9982598

Vector databases in LLMs and search

https://www.infoworld.com/article/2335281/vector-databases-in-llms-and-search.html


## Images

<img width="1344" height="768" alt="1" src="https://github.com/user-attachments/assets/2b2ccc46-65d3-400f-9f65-44c30e5fae3a" />
<img width="1344" height="768" alt="2" src="https://github.com/user-attachments/assets/ea8156c3-e06c-4175-a08b-e02af99c5906" />
<img width="2048" height="2048" alt="3" src="https://github.com/user-attachments/assets/69303f11-7376-4be7-862f-6f23b26bdd5e" />
<img width="1344" height="768" alt="4" src="https://github.com/user-attachments/assets/605f244a-dd71-488b-8601-4c95ccba6ae1" />
<img width="2816" height="1536" alt="5" src="https://github.com/user-attachments/assets/2da69f0b-54e8-46c7-9aae-2c27fba838e7" />

<img width="2816" height="1536" alt="6" src="https://github.com/user-attachments/assets/3d80d053-90b4-494e-87d2-01674e67a016" />
<img width="2816" height="1536" alt="7" src="https://github.com/user-attachments/assets/fd1928e6-1d67-444b-a7bb-f92c7ee10bfb" />
<img width="2816" height="1536" alt="8" src="https://github.com/user-attachments/assets/de308766-9754-4290-82c5-7fa5ab2c6057" />
<img width="2816" height="1536" alt="9" src="https://github.com/user-attachments/assets/ae1abb63-2826-4f0c-b53d-33aca42ad1fc" />
<img width="2816" height="1536" alt="10" src="https://github.com/user-attachments/assets/f93c43f3-da7f-43fb-a539-8611a3bac832" />





