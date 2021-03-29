# PaymentRecords

## Downloads

支付管理后台演示地址：[国内领先的支付管理平台](https://paycloud.vip)

## Steps

1）mvn clean install

2）cp payments.db target

3) java -jar target/cd paymentrecords-0.0.1-SNAPSHOT.jar

4）curl http://localhost:8080/update?currency=HKD&amount=1200
   record:HKD 1200

5）curl http://localhost:8080/scheduled/task
   start up query for all payment_record  every 60 seconds


## Introduction

1) Demo uses Springboot And Sqlite to Show 
   Use synchronized and Pessimistic  lock of DB for  concurrent access 
