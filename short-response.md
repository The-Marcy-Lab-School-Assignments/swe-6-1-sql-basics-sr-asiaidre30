# Short Response: SQL Basics

Answer each question below. Write in complete sentences (3–5 per answer).

---

## Question 1

What is a database? Why do we use one instead of storing data in a JavaScript array on your server?

**Your answer:**

A database is a system used to store, organize, and manage data so it can be easily accessed and updated. We use a database instead of a JavaScript array because databases can handle much larger amounts of data and keep it safe even if the server restarts. They also allow multiple users or applications to access the data at the same time without conflicts. In addition, databases provide powerful tools like querying, filtering, and indexing, which make working with data much faster and more efficient

---

## Question 2

What is a primary key? Why does every table need one?

**Your answer:**

A primary key is a unique identifier for each record (row) in a table. It ensures that no two rows have the same value, which helps keep the data accurate and organized. Every table needs a primary key so you can easily find, update, or delete specific records without confusion. It also helps connect tables together using relationships, like linking users to their orders.

---

## Question 3

In one sentence, describe what this query does in plain English:

```sql
SELECT * FROM books WHERE genre = 'fiction' ORDER BY year DESC LIMIT 5;
```

Aim for something like: _"It returns the 5 most recently published fiction books."_

**Your answer:**

It returns the 5 most recently published books that are in the fiction genre.

---

## Question 4

Why is it dangerous to run `DELETE FROM books` without a `WHERE` clause? What does it actually do?

**Your answer:**

Running `DELETE1` FROM books without a `WHERE` clause is dangerous because it removes every single record in the table. It does not delete just one row, it deletes all the data stored in the books table. This can lead to permanent data loss if there is no backup. That’s why it’s important to always include a WHERE clause when you only want to delete specific records.

---

## Question 5

What is the difference between `ORDER BY` and `LIMIT`? Could you use one without the other? Give an example to support your answer.

**Your answer:**

`ORDER BY` is used to sort the results of a query, while `LIMIT` is used to control how many results are returned. You can use one without the other depending on what you need. For example, you could use ORDER BY year DESC to sort books from newest to oldest without limiting how many are shown. Or you could use LIMIT 10 to return only 10 records without caring about the order.
