# AzureDay.Global

## How to run your local AzureDay webpage?

### General

- Fork this repo.
- Create a new page.
- Create pull request and assign it to **Anton Boyko** (aka [boyko-ant](https://github.com/boyko-ant)).
- As soon as your pull request will be manually reviewed the website will be updated.

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

