# Milestone 1


## Functions & Test Cases
**Function 1)**


**Function 2)** `locate_na`: Returns a dataframe of the count and indices of NA values.  This function takes in a dataframe and finds NA values and returns the location of these values along the count of total NAs.

```
def locate_na(input_df):
"""Locate and return the indices to all missing values within an inputted dataframe.
   Parameters
   ----------
   input_df : dataframe
      This is the dataframe that the function will use to locate NAs.
      
   Returns
   -------
   List of tuples
   Each tuple in the list represents a the indices of a missing value in the dataframe. 
   >>> locate_na(pd.DataFrame(np.array([[“Yes”, “No”], [“”, “Yes”]])))
   [(1, 0)]
   >>> locate_na(pd.DataFrame(np.array([[“Yes”, “No”, “”], [“”, “Yes”, “Yes”]])))
   [(0, 2), (1, 0)]
"""
```

*Test cases for `locate_na`*:
- If `input_df` is not of type dataframe, the function will return an error telling the user that the input data is not a dataframe.
- Dataframe with 0 NAs should return an empty list with no NA indices.
- Dataframe with 1 NA should return a list with the indices of the NA. 

**Function 3)**