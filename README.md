|Actions|HTTP METHOD | URLS| ActiveRecord| SQL | Ruby|
|-|-|-|-|-|-|
Index| GET | /movies | Movie.all | SELECT * FROM movies | Movie.all |
|Show | GET | /tribunes/1 | Tribune.find(1) | SELECT * FROM tribunes WHERE id = 1 | Tribune.all.find { |tribune| tribune.id == 1 } |
Create | POST | /dogs/ | Dog.create(name: "Fluffy") | INSERT INTO dogs (name) VALUES (fluffy) | Dog.new
Delete | DELETE | /attorneysgeneral/1 | AttorneyGeneral.find(1).destroy | DELETE FROM attorney_generals WHERE id = 1 | 
Update | PATCH | /books/1 | Book.find(1).update(title: "Count of Monte Cristo") | UPDATE books SET books.title = "New Title" WHERE id = 1

