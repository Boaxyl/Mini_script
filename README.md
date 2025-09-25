# Mini_script

Perfect — I can help you turn this into a neat **markdown report** that documents what you learned, including the screenshots and explanation. Here’s a structured version:

````markdown
# Shell Scripting: Passing Arguments and Environment Variables

## What I Learned

In this exercise, I learned how to pass an **argument** to a shell script so that the outcome of the script can be changed dynamically based on the value provided.  

I used the command:  

```bash
export ENVIRONMENT=production
````

to pass the environment as a parameter to the script (`aws_cloud_manager.sh`).

I also learned that arguments provided to a script can be **validated** by adding logic such as:

```bash
# Checking the number of arguments
if [ "$#" -ne 1 ]; then 
    echo "Usage: $0 <environment>"
    exit 1
fi
```

This ensures the script only runs if the correct number of arguments is provided.

---

## Screenshots

### Running the script without arguments

![No environment specified](f2cb8f00-63a5-4917-be57-b6e664c60832.png)

---

### Running the script with arguments

Example: passing `testing` as the environment.

```bash
./aws_cloud_manager.sh testing
```

Output:

```
Running script for Testing Environment...
```

![Script running with testing argument](917fded7-1c03-4e0b-a8b4-da866aadfbb4.png)

---

## Key Takeaways

* I can pass arguments to scripts to modify their behavior dynamically.
* I can set environment variables using `export`.
* Input validation (`$#`) ensures proper usage and prevents errors.
* Adding such logic improves the reliability and consistency of scripts.

```

Do you want me to save this as a **`.md` file** for download, just like I did with your AWS setup guide?
```

