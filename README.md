# Pkmn_Img_Recognition
Exploration of Machine Learning and webscraping using Pokémon images

Models trained for the interatctive website [Sugimachine.](https://sugimachine.herokuapp.com/)

The repository for Sugimachine may be found [here.](https://github.com/Adebruler/SugiMachine)

## Webscraping
Images and Pokémon types were scraped from [Bulbapedia](https://bulbapedia.bulbagarden.net/wiki/List_of_Pok%C3%A9mon_by_National_Pok%C3%A9dex_number) using Beautiful Soup.

Bulbapedia's files structure is intentionally obscure, so the process of getting each Pokémon's pictures actually required getting the links for each Pokémon's page from the above index, and scraping each of those pages to find the main image.

## Machine Learning Models
Models were trained using the Keras package in Python.

Several models were trained to find the best fit for the unique needs of Pokémon (such as having two types for many Pokemon) and reduce overtraining.

Two hidden layers were determined to be sufficient to prevent the model from getting stuck guessing only the two most common types.

Droping nodes had better results than batch normalization.

The results were very color-dependent, so a grayscale model was also developed to see what progress could be made based on shapes. It was vastly less progress.
