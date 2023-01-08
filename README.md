# temp-repo

## Warming up

1. Please run the application
2. At the beginning please set the default port to something else e.g. 30508

## Task 1

Please write simple util class that accepts two parameters:

    "words": ["first", "second", "third"]
    "count": 3

And returns following String:

    "first second third first second third first second third"

## Task 2

Please modify above util class to ignore word that begins with //, so:

    "words": ["first", "//second", "third"]
    "count": 3

Returns:

    "first third first third first third"

## Task 3

Please write simple HTTP endpoint that accepts JSON:

    POST localhost:30508/logic
    With body:
    {
        "words": ["first", "//second", "third"],
        "count": 3
    }

That returns:

    200 OK
    with body:
    {
        "sentence": "first third first third first third"
    }
