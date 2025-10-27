## 1. Manipulating Environment Variables

**Command (Print):**
```bash
printenv <environment variable (optional)>
```

- This command will print out environment variables in the console. 
- Running `printenv` without any arguments prints all the environment variables.
- Providing a specific variable's name as an argument will only print that variable's value.

![Printing All Env's](envimages/envimage1.png)

![Printing only the PWD env](envimages/envimage2.png)

Using the command, `printenv PWD` prints the current working directory.

**Command (Set an ENV):**
```bash
export <ENV>=<Value>
```

This command will create an environment variable that is accessible to all shells like bash, zh, and sh.

**Command (Unset an ENV):**
```bash
unset <ENV>
```

This command will remove an environment variable's value.

![Setting and Unsetting a environment variable's value](envimages/envimage3.png)