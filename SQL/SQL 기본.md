# SQL 기본문법

---

> 참고자료 : campus.datacamp.com
>
> ---

# <u>**1. Selecting columns**</u>

> ---
>
> #### SELECTing single columns
>
> #Select the `title` column from the `films` table.

```SELECT title AS films;```

---



SQL은 구조화된 쿼리 언어로 관계형 데이터베이스라고 불린다. 

관계형 데이터베이스는 테이블 집합이라고 생각할 수 있다.

SQL은 데이터베이스를 만들고 수정할 수 있다.

쿼리는 데이터베이스 테이블(혹은 테이블 조합)의 데이터 요청이다.



---

#### SELECTing multiple columns

#people테이블에서 두 개 컬럼(name, birthdate) 가져오기

``` SELECT name, birthdate FROM people ; ```

#people테이블에서 모든 컬럼 가져오기

``` SELECT * FROM people ; ```

#people테이블에서 모든 컬럼 중 10의 행만 가져오기

``` SELECT * FROM people LIMIT 10 ;```

---

#### SELECT DISTINCT

DISTINCT key로 열에서 고유값을 가져올 수 있다.

#films 테이블에서 country를 하나씩만 가져오기

``` SELECT DISTINCT country FROM films; ```

----

#### Learning to COUNT

하나 이상의 열에서 행의 수를 알 수 있다.

#reviews 테이블의 행의 수를 알아보자.

``` SELECT COUNT(*) FROM reviews;```

---

#### Practice with COUNT

#people 테이블의 행의 수

``` SELECT COUNT(*) FROM people; ```

#결측치없는 birthdates의 수

``` SELECT COUNT(birthdate) FROM people;```

#birth date 고유값 가져오기

```SELECT COUNT(DISTINCT birthdate) FROM people;```

