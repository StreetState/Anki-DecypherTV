# DecypherTV

## To Get Started:

1. Fork this repository and clone your own local copy onto your computer

2. Download Anki for your operating system [here](https://apps.ankiweb.net/)

3. Install the [CrowdAnki plugin](https://ankiweb.net/shared/info/1788670778)
 
4. Install [AnkiHub plugin](https://ankiweb.net/shared/info/116826216)


**NOTE:** To browse the list of/install add-ons (plugins), select the Tools>Add-ons>Browse & Install menu item. You can also use Tools>Add-ons to check which add-ons are installed.

4. Fork this repository

#### How to upload changes

When you want to upload changes you've made to Github, you need to:

1. Get the latest changes from the Github:
    
    ```
    git pull
    ```
2. [Import the deck](#import) to combine changes you've made with the changes other people have made.
3. Export the deck the same directory where your repository is located so that export will overwrite media directory and json file in the repository. (As an alternative you can export it elsewhere and copy json file and media directory yourself to overwrite the ones that are in repository directory.)
4. Add the changes to the repository:

    ```
    git add *
    git commit -m "new updates"
    ```
5. Upload changes you've made to the Github:

    ```
    git push origin master
    ```

If you just want to **get latest changes from other people** - you need to perform only steps 1 and 2.


## Generic collaboration workflow
The current workflow could be described as following:
* The user creates or imports an Anki deck.
* He makes some modification to it (i.e. to notes, deck settings, deck structure or note models).
* Then the user can export the deck in JSON format (accompanied by media directory with media files used in that deck) and share it with other users. For example by creating Github repository with it.
* Other people then can either modify JSON directly or import the deck to their instance of Anki and then make some modifications to it.
* Original JSON then can be updated the with the changes, these people made (merging several changes together if necessary).
* After that original user (and other people) can import updated deck to integrate these new changes into their collection.

## Export
To perform the deck export go to menu File>Export

Select the deck (**note**: export of "All decks" is not supported, you need to select a specific deck) and the export format "CrowdAnki JSON representation".
After pressing the Export button - select directory where the result should be stored.

## Import
To perform the import go to menu File>"CrowdAnki: Import from disk" and select the directory where the deck is stored.

