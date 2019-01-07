# AzureDay.Global

## How to run your local AzureDay webpage?

### General

- Fork this repo.
- Create a new page.
- Create pull request and assign it to **Anton Boyko** (aka [boyko-ant](https://github.com/boyko-ant)).
- As soon as your pull request will be manually reviewed the website will be updated.

### Managing assets

All the assets (like speakers photos, partners logos, etc.) should be placed within `src/assets/` folder. The folder structure is more or less self explanatory.

### Submit conference data

- Create a file under `src/data/conferences/` with the name using the following convention: `<country code><year>.yml`, for example `ua2018.yml` for conference in Ukraine.
- Copy the content structure from `ua2018.yml` file as it has the latest template (at least for now).
- Adjust file content maintaining its original structure.

#### Root properties

| Name | Type | Description |
| --- | --- | --- |
| `url` | string | |  
| `name` | string | |  
| `date` | string | |  
| `venue` | object | |  
| `organizers` | array of objects | |  
| `sessions` | array of objects | |  
| `hasWorkshops` | boolean | |  
| `workshops` | array of objects | |  
| `partners` | array of objects | |  

#### `Venue` property


#### `Organizers` property


#### `Sessions` property


#### `workshops` property


#### `Partners` property



### Submit conference webpage

- Create a file under `src/pages/conferences/` with the name using the following convention: `<country code><year>.md`, for example `ua2018.md` for conference in Ukraine.
- Copy the content structure from `ua2018.md` file as it has the latest template (at least for now).
- Adjust file content maintaining its original structure.

#### Properties

| Name | Type | Description |
| --- | --- | --- |
| `url` | string | maintain the following format `conferences/<year>/<country code>.html` |  
| `template` | string | should be set to `conference.hjs` |  
| `title` | string | maintain the following format `AzureDay <year> - <country>` |  
| `Model.conference` | data | maintain the following format `Data.conferences.<country code><year>` |  
| `Model.banner` | data | *for now should remain without any changes, website owner will set it up properly* |  
