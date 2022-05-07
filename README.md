# **Universal Category Identification Standard**

![GitHub issues](https://img.shields.io/github/issues/universalschedulestandard/UniversalCategoryIdentification)
![GitHub closed issues](https://img.shields.io/github/issues-closed/universalschedulestandard/UniversalCategoryIdentification)
![GitHub pull requests](https://img.shields.io/github/issues-pr/universalschedulestandard/UniversalCategoryIdentification?color=yellow)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/universalschedulestandard/UniversalCategoryIdentification?color=yellow)
![GitHub Repo stars](https://img.shields.io/github/stars/universalschedulestandard/UniversalCategoryIdentification?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/universalschedulestandard/UniversalCategoryIdentification?style=social)

Historically, categories have been considered to be unique to an individual project and have been subject to the tastes of each individual. For example, different individuals might refer to 'Cast Members' as 'Cast', 'Actors' or 'Talent'. 'Background Performers' might be 'Background', 'Extras' or 'BG'. When those individuals attempt to share their data, this practice can become problematic because the names of their categories had not been standardized. 

To solve this issue, the Universal Category Identification Standard assigns immutable identification numbers to each category type. This allows for an individual to alter the name of a category but still convey the intent of that category when the data is being transferred, parsed or stored. Regardless of what you call your actors, the data will refer to that category by its ID number. 

This standard does not in any way negate the ability of individuals to customize their categories to their projects. Categories may be named anything the user wishes to name them. Additionally, the standard allows for the addition of categories that pertain just to a particular project or the tastes of the person who is creating their schedule. See [Extending the Standard](#Extending-the-Standard) for more information about adding categories.  

Additionally, categories come in two flavors:

## Scene Categories

Scene categories refer to the entire scene as a whole. These include 'Set', 'Day/Night', 'INT/EXT', 'Unit', 'Sequence', etc. 

Here is a full list of the scene categories with their corresponding ID numbers:

    "id": 0, "name": "Set"
    "id": 1, "name": "INT/EXT"
    "id": 2, "name": "Day/Night"
    "id": 3, "name": "Script Day"
    "id": 4, "name": "Unit"
    "id": 5, "name": "Sequence"
    "id": 6, "name": "Location"

## Action Categories

Action categories contain elements found in the content of a scene, such as 'Cast Members', 'Props', 'Wardrobe', etc.

Here's a full list of the action categories with their corresponding ID numbers:

    "id": 100, "name": "Cast Members"
    "id": 101, "name": "Background Actors"
    "id": 102, "name": "Stunts"      
    "id": 103, "name": "Vehicles"    
    "id": 104, "name": "Props"       
    "id": 105, "name": "Special Effects"
    "id": 106, "name": "Wardrobe"    
    "id": 107, "name": "Makeup/Hair" 
    "id": 108, "name": "Animals"     
    "id": 109, "name": "Animal Wranglers"
    "id": 110, "name": "Camera"
    "id": 111, "name": "Music"
    "id": 112, "name": "Sound"
    "id": 113, "name": "Art Department"
    "id": 114, "name": "Set Dressing"
    "id": 115, "name": "Greenery"    
    "id": 116, "name": "Security"    
    "id": 117, "name": "Special Equipment"
    "id": 118, "name": "Additional Labor"
    "id": 119, "name": "Visual Effects"
    "id": 120, "name": "Mechanical Effects"
    "id": 121, "name": "Notes"
    "id": 122, "name": "Comments"    
    "id": 123, "name": "Miscellaneous" 
    "id": 124, "name": "Other"
    
The `name`s of the categories are merely the commonly used versions and are used here simply to communicate the intent of the category. 

## Maintaining the Intent

The most important part of the category standard is that all of the categories must retain their original intent. Renaming 'Cast Members' to 'Actors' is entirely allowable. But repurposing the 'Cast Members' category to 'Wagons' and filling it with elements such as 'Horse and Buggy' is not allowed. Maintaining the intent of the category allows for universal transfer of category data between individuals and platforms. 

## Extending the Standard

Note that the ID numbers for scene and action categories have a wide gap between them. The scene category IDs are numbered `0` - `6` and the action categories begin at `100`. This has been done to allow for future extensions of these standardized categories. 

If you need to add custom script categories, they should be assigned IDs starting at `50`, but may not exceed `99`. Any custom action categories should be assigned sequential ID numbers beginning at `500`. The ID numbers `0` - `49` and `100` - `499` are reserved for exclusive use by this standard for future expansions.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/">
  <img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nd/4.0/">Creative Commons Attribution-NoDerivatives 4.0 International License.
</a>
