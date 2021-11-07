# Squidle+の用語解説

## Terms for Datasources
Term | Description 
--- | --- 
`Platform` | The equipment/method used to collect the imagery data (eg: a specific AUV, ROV or camera platform) 
`Data Provider` | The organisation, institution or operator in charge of managing the data collected by the `Platform` 
`Datasource Repository` | An accessible, non-ephemeral, (usually online) archive for uploading raw underlying imagery and survey data collected by a `Data Provider`  
`Datasource Plugin` | A software module that facilitates reading from a `Datasource Repository`
`Datasource Definition`  | The parameters that define the structure and format of the data on the `Datasource Repository` and which `Datasource Plugin` to use. Each `Platform` must have at least one `Datasource Definition`.


## Terms for Datasets
Term | Description 
---- | ----
`Media Object` | a discreet visual data object from a `Deployment`, like and image, video, mosaic. `Media Objects` require Interpreter plugins to be viewable and annotatable using the online tools. 
`Campaign` | a group of `Deployments`. Eg: a specific expedition, cruise or data collection initiative 
`Deployment` | a dataset containing a group of `Media Objects` collected from an operation of the `Platform`, eg: a survey, transect or mission 
`Media Collection` | a user-defined collection of `Media Objects` grouped for further analysis. Can be a subset of `Media Objects` from one or more `Deployments`
`Annotation Set` | the definition of how to annotate the `Media Collection`. I.e. the annotation method, parameters and `Label Scheme` to be used. A `Media Collection` can have more than one associated `Annotation Set`
`Label Scheme` | the chosen list of possible `Labels` for which to apply to `Annotations`. There are multiple `Label Schemes`.
`Label` | a discreet concept from the `Label Scheme` that can be assigned to `Annotations`
`Annotation` | a linking of a `Label` to an observation in a `Media Object` (i.e. a `Label` on a `Point` in a frame)
`Point` | an annotatable object on a media frame, captures x,y,t and can have multiple Annotations associated with it. A point can also be associated with a bounding box, polygon, pixel map, etc... Each `Point` can have one or more `Annotations`
`Tag` | an additional modifier that can be applied to an `Annotation`. Each `Annotation` can have multiple `Tags`.
`Comment` | a freeform entry that can be associated with an `Annotation`. 

