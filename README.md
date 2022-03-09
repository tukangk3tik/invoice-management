Written in Kotlin.

Thankyou for Artivisi Intermedia. <br />
Youtube channel: https://www.youtube.com/user/artivisi <br />
Note: In this video, the application is written using Java

# INVOICE MANAGEMENT APPLICATION #

This application is used to manage invoices and connect with various modern payment methods.
Payment methods that will be supported include:

* Virtual Account Bank
  * Bank BNI
  * Bank CIMB
  * Bank BSI
  
* E-Wallet
  * Ovo
  * Gopay
  
* QR Payment 
  * QRIS 


# Setup Database #

1. Jalankan postgres di docker
  ```
  docker run --rm \
    --name invoice-db \
    -e POSTGRES_DB=invoicedb \
    -e POSTGRES_USER=invoice \
    -e POSTGRES_PASSWORD=gaLqm1BV8J5wojS0hNhG \
    -e PGDATA=/var/lib/postgresql/data/pgdata \
    -v /m/'Learn cool stuff'/Spring/invoice-management-kotlin/invoicedb-data:/var/lib/postgresql/data \
    -p 5432:5432 \
    postgres:13