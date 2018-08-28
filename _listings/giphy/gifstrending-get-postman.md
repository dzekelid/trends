{
  "info": {
    "name": "Giphy Gif API Trending GIFs",
    "_postman_id": "33b0cd00-cefe-49c4-a2b8-6dbf153c8144",
    "description": "Fetch GIFs currently trending online. Hand curated by the GIPHY editorial team.  The data returned mirrors the GIFs showcased on the GIPHY homepage. Returns 25 results by default.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gifs",
      "item": [
        {
          "id": "d0066152-1110-46b4-bb74-f78b92f27b78",
          "name": "getGifsById",
          "request": {
            "url": "http://api.giphy.com/v1/gifs?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A multiget version of the get GIF by ID endpoint."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "e735c52d-687b-42bd-8f1a-5064c35652e1"
            }
          ]
        },
        {
          "id": "d86ab31c-51f8-4294-bae2-efd7a5fd45d2",
          "name": "randomGif",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/random?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a random GIF, limited by tag. Excluding the tag parameter will return a random GIF from the GIPHY catalog."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "7370fde5-5d18-48a9-a2bf-bc75c4d08591"
            }
          ]
        },
        {
          "id": "f9dcd82c-9308-41a3-8343-4eddfcc45063",
          "name": "searchGifs",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/search?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search all GIPHY GIFs for a word or phrase. Punctuation will be stripped and ignored.  Use a plus or url encode for phrases. Example paul+rudd, ryan+gosling or american+psycho."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "d2acaaaa-c057-4bbf-a8aa-78b8d2f50b14"
            }
          ]
        },
        {
          "id": "18632c47-9494-4739-ba82-07a6dc2bd7f2",
          "name": "translateGif",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/translate?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The translate API draws on search, but uses the GIPHY `special sauce` to handle translating from one vocabulary to another. In this case, words and phrases to GIF"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "f6f05238-dfd6-47ab-bfba-eba5f85531bd"
            }
          ]
        },
        {
          "id": "cb49459f-1a0f-4014-9fda-2be5b75f04e3",
          "name": "trendingGifs",
          "request": {
            "url": "http://api.giphy.com/v1/gifs/trending?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Fetch GIFs currently trending online. Hand curated by the GIPHY editorial team.  The data returned mirrors the GIFs showcased on the GIPHY homepage. Returns 25 results by default."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "c91d3cc8-5e3b-4538-90ba-7b6ab8ac2f22"
            }
          ]
        }
      ]
    }
  ]
}