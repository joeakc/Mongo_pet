# Steps
1. Initializing git repo
2. Initializing mongodb ( register a connection)
3. Modify the classes (snakes, owners, cages) by using meta(a dictionary) and creating db_alias and a collection
4. Specify the type of the fields (string, float, bool, datetime)
5. Each class is must extend the document class (mongoengine.Document)
6. A class as the cage which has a list of booking documents, will have a list of type embedded documents.
    bookings=mongoengine.EmbeddedDocumentListField(Booking)
    Class of bookings will extend EmbeddedDocument
7. Ids in mongodb are objectidfields.