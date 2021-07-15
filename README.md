запрос(ы) для вставки данных минимум о двух книгах в коллекцию books
db.books.insertMany ([
    {
        title: "001",
        description: "001",
        authors: "001"
    }, 
    {
        title: "002",
        description: "002",
        authors: "002"
    }
])

запрос для поиска полей документов коллекции books по полю title
db.books.find (
    { title: 001 }
)

запрос для редактирования полей: description и authors коллекции books по _id записи
db.books.updateOne (
    { id: xxx },
    { $set: { description: "003"}, {authors: "003"}}
)
