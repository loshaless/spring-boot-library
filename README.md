# Run Me First
Please run the migration.sql first from src/main/sql/migration.sql
Make sure that the data run on localhost:3306

# Description
this is the mini project of book lover.  
In this project maybe you wonder why there is no controller. 
The reason is because this project is using `spring-boot-starter-data-rest`.


# Table
there is 2 tables in this mini project:  
1. book
2. review

The relation between this tables is one to many: one book has many reviews

# Endpoint

1. GET: http://localhost:8080/books/{?page,size,sort}
2. GET: http://localhost:8080/books/{bookId}
3. GET: http://localhost:8080/books/{bookId}/reviews
4. GET: http://localhost:8080/books/search/findByTitleContaining{?title,page,size,sort}
5. GET: http://localhost:8080/books/search/findByCategory{?category,page,size,sort}
4. GET: http://localhost:8080/reviews{?page,size,sort}
5. GET: http://localhost:8080/reviews/{reviewId}
6. GET: http://localhost:8080/reviews/search/findByBookId{?bookId,page,size,sort}
