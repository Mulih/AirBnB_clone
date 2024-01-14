This is a detailed document on the description of the Airbnb console
*Classes*
Public instance Attributes
- BaseModel:- id, created_at, updated_at
- User:- inherits from BaseModel
- State:- Inherits from BaseModel
- City:- Inherits from BaseModel
- Amenity:- Inherits from BaseModel
- Place:- Inherits from BaseModel
- Review:- Inherits from BaseModel
Public Instance Methods
- BaseModel:- save, to_dict
- FileStorage:- all, new, save, reload
- User:- Inherits from BaseModel
- State:- ""
- City:- ""
- Amenity:- ""
- Place:- ""
- Review:- ""
Public Class Attributes
- User:- email, password, first_name, last_name
- State:- name
- City:- state_id, name
- Amenity:- name
- Place:- city_id, user_id, name, description, number_rooms
        number_bathrooms, max_guest, price_by_night, latitude, longitude, amenity_ids
- Review:- place_id, user_id, text
Private Class Attributes
- FileStorage:- file_path, objects

*Storage*
The above classes are handles by the storage engine defined in the FileStorage class.

T
*Console*
The console is a command line interpreter that allows manaagement of the backend of the Airbnb clone. It can be used to handle and manipulate all classes utilized by the application(achieved by calls on the storage)