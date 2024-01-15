# Full cycle - Challange go

The challenge consists of publishing in the docker hub lightweight image with
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

### Step by step
In case you don't have the golang installed on your machine, as in my case, you can run the following command
`docker run --rm -it -v $(pwd):/usr/src/app golang`.


After you run this command you are going to be inside the container 
terminal
```
root@a31134937a2b:/go#
```
Execute
```
go mod init <APP_NAME>
```
This is going to generate the `go.mod` file. It's like the package.json does JS, composer.json does PHP or requirements.txt does Python.

After that, you can create the main.go by typing 
```
touch main.go
```
and then copy and paste the following [hello world](https://gobyexample.com/hello-world) example.

Last but not least, you will have a working `go` file.
And you can execute the [Extra command](##Extra commands) 

##### Images sizes

Using `multistage building` - `1.8MB`

Not using `multistage building` - `885MB`



