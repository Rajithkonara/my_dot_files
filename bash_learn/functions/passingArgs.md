```sh
#!/bin/bash

google() {
    search=""
    echo "Googling: $@"
    for term in $@; do
        search="$search%20$term"
    done
    google-chrome "http://www.google.com/search?q=$search"
}
google $@   #passing argument
```