# SQL 기본

---

> <기본 문법, SELECTing single columns>
>
> #Select the `title` column from the `films` table.

```SELECT title AS films;```

---

SQL은 구조화된 쿼리 언어로 관계형 데이터베이스라고 불린다. 

관계형 데이터베이스는 테이블 집합이라고 생각할 수 있다.

SQL은 데이터베이스를 만들고 수정할 수 있다.

쿼리는 데이터베이스 테이블(혹은 테이블 조합)의 데이터 요청이다.



---

<기본 문법, SELECTing multiple columns>

#people테이블에서 두 개 컬럼(name, birthdate) 가져오기

``` SELECT name, birthdate FROM people ; ```

#people테이블에서 모든 컬럼 가져오기

``` SELECT * FROM people ; ```

#people테이블에서 모든 컬럼 중 10의 행만 가져오기

``` SELECT * FROM people LIMIT 10 ;```

---



<기본 문법, SELECT DISTINCT>