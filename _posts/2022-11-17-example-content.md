---
layout: post
title: "MongoDB 정리"
date: 2022-11-11 00:15:00 +0900
categories: jekyll update
comments: true
---

## MongoDB가 JS를 사용해서 얻은 특징

- 웹 개발자에게 쉬운 입문이 가능하다
- BSON 자료형을 사용
- 내부 명령어를 JS 형식으로 사용

## MongoDB의 CRUD

### MongoDB의 기본 구조

- 데이터베이스 (← database)
- 컬렉션 (← table)
- 도큐먼트 (← row)

### Document → BSON(Binary JSON) 자료구조

python
# import python-mongo module
import pymongo

# create connection between DB and Script
connection = pymongo.MongoClient('mongodb://localhost:27017/')

#access database (if not exist, create one!)
db = connection.get_database("testDB")

# access collection under database
collection = db.get_collection("testCollection")

# INSERT data in collection
collection.insert_one({'hello':'world'})