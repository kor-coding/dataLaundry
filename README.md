# dataLaundry
Purposely built to deal with tricky list nested dict


Laundry


Laundry – outer_data

Source is a list of nested dict, therefore, first in outer_data does is to “peel” the data. Peeling of each element once at a time, converting the source into a dict of general properties for each of the element and conclude one element (at a time) as compile_dict.


Laundry – prop_serializer

Source ‘properties’ consist of variety of dict inside the list, where such data basically non useable by any python, no way to iterate both list and dict at the same code time. Therefore, this action is to serialize, making all dict inside the list into enumerated, numbered dict. 


Laundry – change_num

As element extracted once at a time, change_num acts as a coordinator to give a whole new number to each new element, assuring no repetitive or duplication of number assigned to each element and properties. 


Laundry – temp_dict

With the number changed, using ** to act as append to bigger dict container, adding each element into the big nested dict, temp_dict.
Laundry – data_frame_serializer
As there are more list of dict inside, uses pandas data_frame to breakout all the elements, and reach directly to list item and dissolve it into proper dict.


Laundry, conclusion

First peel outer layer, take out an element a time. Then, serialize list of dict into normal dict. Then, convert with new numbering and append into new dict. Then, further serialize multiple lists of dict into normal nested dict. Lastly, do the same thing again for next element until all elements does.
