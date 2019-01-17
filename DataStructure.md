# Storage

  > This is where Firebase stores binaries such as images.

* profile_pics/
  * uid-00001/
    * profile_image
* listing_pics/
  * uid-00001/
    * lid-00001/
      * image-00001
      * image-00002
      * image-00003
      * image-00004
    * lid-00003/
      * image-00008
      * image-00009
  * uid-00002/
    * lid-00002/
      * image-00005
      * image-00006
      * image-00007


# DataBase

  > This is where Firebase stores information as documents (noSQL).

* users/
  * uid-00001/
    * profile_image_url
    * my_listings/
      * lid-00001
      * lid-00003
  * uid-00002/
    * profile_image_url
    * my_listings/
      * lid-00002
* listings/
  * lid-00001/
    * address
    * header_photo_url
    * photo_urls/
      * image-00001_url
      * image-00002_url
      * image-00003_url
      * image-00004_url
    * description
    * tags/
      * smoking_permitted/
        * true
      * dogs_permitted/
        * false

# Auth

  > This is where Firebase stores and configures users and auth options.

* User
  * email
  * password
  * display name
  * uid
  * date created
  * last date signed in
