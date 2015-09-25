#VOD ingest

##Structure
The main entities in the XML are

 - [PublishMetadata](publish.md)
    - The root element of the message
 - [Content](css.md)  
   - All the metadata regarding the content
 - [Season](css.md)
   - All the metadata regarding the season
 - [Series](css.md)
   - All the metadata regarding the series
 - [Material](material.md)
   - The technical metadata regarding the ingest media
 - [Event](event.md)
   - The metadata regarding the publication of the content to the end customer

##Updates
To update the content in EMP you just send a Publish-metadata message for the same content ID with updated field values and this will overwrite the current values. You don't need to send a complete XML for updates. Simply send the field you want to update and the other field will stay untouched.