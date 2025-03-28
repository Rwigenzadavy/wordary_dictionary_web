# wordary_dictionary_web
this  is a simple web application that works as Dictionary. you can use this to get the explanation of any word you want to know its meaning in English. it shows all the definition of the words in English. it is easy to use and its user interface its user friendly. 

## How It works
This Application has a search bar where the user enter an English word the he/she wants to know its meaning and then it provides a simple definition of that word.

## API used
`https://api.dictionaryapi.dev/api/v2/entries/en/${word}` from free dictionary API. 

## Technologies used

- HTMl
- CSS
- Javascript
- REST APIs to fetch data

# GET start with it
 ## 1. clone the repository
   ```bash
   git clone https://github.com/Rwigenzadavy/wordary_dictionary_web.git
   ```
  ## 2. Navigate to the project directory:
   ```bash
   cd wordary_dictionary_web  
   ```
  ## 3. open the index.html file in your browser 
     you see the form with search bar
  - enter the word you want to know its definition in the search bar
  - press the Search button to see the definition of the word you search for

# Demo video of how it works:
https://youtu.be/sLBwyZK1kXM

# credit

free dictionary API from https://dictionaryapi.dev/

## Deployment

-The loadbalancer configuration
```bash
# Frontend: Listen for incoming traffic on port 80
frontend http_front
    bind *:80                      
    default_backend http_back

backend http_back
    balance roundrobin              
    server web01 184.72.203.182:80 check  
    server web02 54.162.102.135:80 check  
```

## The web link is:
http://davyrwi.tech/
