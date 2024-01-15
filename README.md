# Full cycle - Challange go

The challenge consists of publishing in docker hub lightweight image with
max size of 2MB

## Check results
```
# Exec
 docker run marcos2020souza/fullcycle
# Outcome in terminal
 Full Cycle Rocks!!
```

## Extra commands
If you want to execute without the `multistage building`, execute:
```
# Exec
 docker build -t fullcycle .
 docker run --name hello-fullcycle-rocks fullcycle .
# Outcome in terminal
 Full Cycle Rocks!!
```

##### Images sizes

Using `multistage building` - `885MB`
Not using `multistage building` - `1.8MB`



