# PY Country Details Finder

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![CI](https://github.com/webkolog/py-country-details-finder/actions/workflows/python-tests.yml/badge.svg)](https://github.com/webkolog/py-country-details-finder/actions)

**Version:** 1.0

**Created Date:** 2026-09-02

**Last Updated:** 2026-09-02

**Compatibility:** Python 3.x

**Created By:** Ali Candan ([@webkolog](https://github.com/webkolog))

**Website:** [http://webkolog.net](http://webkolog.net)

**Copyright:** (c) 2026 Ali Candan

**License:** MIT License ([http://mit-license.org](http://mit-license.org))

---

**PY Country Details Finder** is a lightweight Python script that fetches and displays detailed information about any given country. Utilizing the `countryinfo` module, it quickly returns key data including capital, population, total area, region, currencies, spoken languages, and neighboring borders.

## Installation

1. **Clone the repository:**
```bash
   git clone https://github.com/webkolog/py-country-details-finder.git
   cd py-country-details-finder

```

2. **Install required dependencies:**
Make sure you have Python installed, then install the `countryinfo` package:
```bash
pip install countryinfo

```



## Usage

Run the main Python script:

```bash
python py-live-internet-speed.py

```

Upon execution, enter the name of the target country when prompted:

```text
Enter Country Name: Turkey

```

### Output Data Fields

* **Capital:** The capital city of the specified country.
* **Population:** Estimated total population.
* **Area:** Land size expressed in square kilometers.
* **Region & Subregion:** Geographical classification.
* **Demonym:** The term used for inhabitants of the country.
* **Currency:** Official currencies used in the nation.
* **Languages:** Officially spoken languages.
* **Borders:** List of neighboring countries (ISO alpha-3 codes).

## Example Output

```text
Enter Country Name: Japan
Capital: Tokyo
Population: 126476461
Area (in square kilometers): 377835
Region: Asia
Subregion: Eastern Asia
Demonym: Japanese
Currency: ['JPY']
Languages: ['ja']
Borders: []

```

## Error Handling

If an invalid country name is entered, `countryinfo` may throw a `KeyError`. It is recommended to verify the spelling or handle exceptions when integrating into larger workflows:

```python
from countryinfo import CountryInfo

try:
    country = CountryInfo(input("Enter Country Name: "))
    print("Capital:", country.capital())
except KeyError:
    print("Error: Country not found. Please check the spelling.")

```

## Dependencies

* Python 3.x
* [countryinfo](https://pypi.org/project/countryinfo/) library

## License

This project is open-source software licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for features, feel free to open an issue or submit a pull request on the GitHub repository.

## Support

For questions, issues, or suggestions, please open an issue in the repository or visit [webkolog.net](http://webkolog.net).

```
