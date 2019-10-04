# Mail Sink

A simple no frills mail sink for sending and receiving emails. 
For development purposes only, not production ready.

## To build

`docker build -t mail-sink .`

## To run
`docker run --name mail-sink -p 8765:8080 -p 8025:8025 -d mail-sink`

## To access via browser

http://localhost:8765 

username = smtp

password = smtp

## To send email

### Send email Within docker

```
SmtpHost=mail-sink
SmtpPort=8025
SmtpUser=smtp
SmtpPassword=smtp
```

### Send email local machine

```
SmtpHost=localhost
SmtpPort=8025
SmtpUser=smtp
SmtpPassword=smtp
```

