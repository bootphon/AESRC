How to split the data?
=====================
- Prepare thet dataset (AESRC).
- Copy the dataset to the work folder.

- Gender split process:

run the script `python3 aesrc_gender_split.py`on your dataset  to get the Male/Female lists.

  - `input : dataset path`.
  - `output :  an output file`, with all the sublist Male and Female for each accent.
  
see the [aesrc_speakers_list.txt]() for the lists we got after the split.

- Data split process:

  - creat folder `derived_data_10`: 10 min for each speaker, it contains the results files, with total duration of 2h.
  - creat folder `derived_data_2`: 2 min for each speaker.
  - run the script `python3 aesrc_dataset_split.py dataset_path duration`.

  - split the dataset on 10 min for each speaker to get total 2h of speech (1h audio for Male and 1h for Female speech) for test and dev set.
  - split the rest of the dataset on 2 min for each speaker to get total 

From the rest files, re-run the script to get files with 2 min.

  - `input: dataset path, duration*`
  - `output: audio files with total duration 10 min/spk or 2 min/spk`.


*duration : 10 min/spk => 600sec and 2 min/spk=>120sec/spk
