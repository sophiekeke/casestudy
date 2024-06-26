# References

## People 1
- [https://www.1point3acres.com/bbs/thread-799358-1-1.html](https://www.1point3acres.com/bbs/thread-799358-1-1.html)
- Python部分就是把SQL写的代码转换成Python而事实上Python部分是一个algorithm题目

## People 2
- [https://www.1point3acres.com/bbs/thread-914344-1-1.html](https://www.1point3acres.com/bbs/thread-914344-1-1.html)
- 第一轮techscreen考了SQL
- 第二轮casestudy是关于user onboarding tutorial里对一个步骤进行改变怎么evaluate

This markdown includes the references and descriptions formatted for inclusion in a GitHub markdown file.


# SQL Table Structures

## Table: `logical_cluster`

| Field            | Type          | Null | Key | Default | Extra |
|------------------|---------------|------|-----|---------|-------|
| id               | varchar(255)  | NO   | PRI | NULL    |       |
| type             | varchar(255)  | YES  |     | NULL    |       |
| org_id           | int           | YES  |     | NULL    |       |
| created_date     | date          | YES  |     | NULL    |       |
| created_at       | timestamp     | YES  |     | NULL    |       |
| deactivated_date | date          | YES  |     | NULL    |       |
| deactivated_at   | timestamp     | YES  |     | NULL    |       |

## Table: `organization`

| Field            | Type          | Null | Key | Default | Extra |
|------------------|---------------|------|-----|---------|-------|
| id               | int           | NO   | PRI | NULL    |       |
| created_date     | date          | YES  |     | NULL    |       |
| created_at       | timestamp     | YES  |     | NULL    |       |
| deactivated_date | date          | YES  |     | NULL    |       |
| deactivated_at   | timestamp     | YES  |     | NULL    |       |
| is_customer      | tinyint(1)    | YES  |     | NULL    |       |

# SQL Query

Write a query to get the count of orgs created per day in Nov 2020 and the 5-day rolling aggregation (i.e., number of orgs created in the past 5 days).


## 2nd Question
Write a query to get the number of 'kafka', 'connect', and 'ksql' clusters that were created by customers in August 2020 and September 2020.
