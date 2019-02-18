# Storage

  > This is where Firebase stores binaries such as images.

* pictures/
  * listings/
    * lid/
      * profile picture
      * pictures/
        * picture ...



# DataBase

  > This is where Firebase stores information as documents (noSQL).

* users/
  * uid/
    * name : `String`
    * email : `String`
    * phone : `String`
    * profile_url : `String`
    * listings : `[ lid ]` (max 2)
    * tags : `{ String : Any }`
      * smoking : `Boolean`
      * dogs : `Boolean`
      * cats : `Boolean`
      * other_pets : `Boolean`
    * preferences : `{ String : Any }`
      * measurement_unit : `String`
    * school : `sid`
    * major : `mid`
* listings/
  * lid/
    * address_1 : `String`
    * address_2 : `String`
    * zip_code : `String`
    * unit_number : `String`
    * hm_bed : `String` 
    * hm_bath : `String`
      > Floor plan = hm_bed & hm_bath
    * tags : `{ String : Any }`
    * dates : `{ String : Timestamp }`
    * map_location : `Geopoint`
    * location_name : `String`
    * looking_for : `String` ??? what is this?
    * costs : `{ String : Number }`
    * vacancies : `Number`
    * Comments : `String`

* schools/
  * sid/
    * name : `String`
* majors/
  * mid/
    * title : `String`



# Auth

  > This is where Firebase stores and configures users and auth options.

* User
  * identifier (email)
  * providers (auth methods)
  * date created
  * last date signed in
  * uid
    > *not stored visibly*
      * *password*
      * *display name*
