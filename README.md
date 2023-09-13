[![DOI](https://zenodo.org/badge/676508766.svg)](https://zenodo.org/badge/latestdoi/676508766)

# Multimodal fall detection dataset

Multimodal dataset for fall detection. Includes acceleration data collected from a tag and two smartwatches, and location reported by the tag. More details about the data collection procedure can be found in `notes.md`.

The dataset is archived [in Zenodo](https://doi.org/10.5281/zenodo.8340378).

## Contents

The repository contains:
- `data/location_data.csv` and `data/full_acceleration` – preprocessed acceleration and location data from 10 participants and mannequin simulated falls with target variable identified
- `data/subsampled_acceleration_data.csv` – subsampled acceleration dataset used for training the AI model
- `notes.md` – description of activities performed and notes from data collection
- `videos` – reference videos for performed activities

## Authors

- [Anastasiya Danilenka](https://orcid.org/0000-0002-3080-0303) – research methodology, data collection and processing
- [Piotr Sowiński](https://orcid.org/0000-0002-2543-9461) – research methodology, data collection and processing
- [Monika Kobus](https://orcid.org/0000-0003-3217-1050) – research methodology, data collection
- [Anna Dąbrowska](https://orcid.org/0000-0003-4295-3005) – research methodology, methodological supervision
- [Kajetan Rachwał](https://orcid.org/0000-0003-1524-7877) – data collection
- [Karolina Bogacka](https://orcid.org/0000-0002-7109-891X) – research methodology
- [Krzysztof Baszczyński](https://orcid.org/0000-0002-9572-2705) – research methodology, data collection

## Acknowledgements

This work is part of the [ASSIST-IoT project](https://assist-iot.eu/) that has received funding from the EU’s Horizon 2020 research and innovation programme under grant agreement No 957258.

The [Central Institute for Labour Protection – National Research Institute](https://www.ciop.pl/en) provided facilities and equipment for data collection.

## License

The dataset is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
