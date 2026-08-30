# DA3408 AIOps Lab - Assignment 1

Find the 1-pager writeup in `Writeup.pdf` and the video walkthrough of the solutions [here](https://drive.google.com/file/d/1WDqPfaH7gk7JPDn_i4KZYrw9ArXQVrpS/view?usp=sharing).

## Q1. Conceptual
All subquestions answered in `Writeup.pdf`.

## Q2.
`q2.ipynb` contains the code that was used to train 6 MLP Classifiers with the final metrics and evaluation of results given in `Writeup.pdf` and the video.

## Q3.
A Backblaze bucket was created to act as a remote server and the names of all files were stored in `filenames.csv`. Consequently only `filenames.csv.dvc` was pushed to GitHub while the original csv file is stored on the remote server. The data files were not stored anywhere as it was not asked to track them. More details in the video.

## Q4. Capstone
Find the shared GitHub repository (with both our commits) [here](https://github.com/Pakshal-Nagda/AIOps-Lab-Assignment-1-Q4)

## Instructions for running the codes:
- Set up a virtual environment and install all the dependencies from `requirements.txt`.
- Set up MLFlow server using the command
```mlflow server --backend-store-uri sqlite:///mlflow.db --default-artifact-root ./mlruns --host 0.0.0.0 --port 5000 --allowed-hosts "*" --cors-allowed-origins "http://localhost:5000, http://127.0.0.1:5000"```
(Note that this will work for Q2. For Q3, you will require access to the corresponding Backblaze bucket.)

## LLM Usage Disclosure

ChatGPT was used to understand some concepts and getting familiar with Linux commands. It included:
- Understanding git and dvc commands and their implications.
- Understanding `sklearn`'s `MLPCLassifier`.
- Asking how to generate csv of filenames from the data/ directory.
- Setting up Backblaze bucket and related settings required in DVC and MLFlow.
- Getting ideas for video editing software.
- Debugging dependency conflicts.

It was NOT used to write any part of the final code or writeup and I take the full responsibility of my work.