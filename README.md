# Sentences mentioned Trump from 2012 to 2016

Web scraping: extract sentences from [The Guardian](https://www.theguardian.com/) that mentioned 'Trump' and related metadata.

## The Guardian data

The [data](https://github.com/letitbevi/sentences-mentioned-Trump-from-2012-to-2016/tree/master/data) folder contains 5 JSON files:

- 2012-01-01-to-2012-12-31_sents_mentioned_trump.json
- 2013-01-01-to-2013-12-31_sents_mentioned_trump.json
- 2014-01-01-to-2014-12-31_sents_mentioned_trump.json
- 2015-01-01-to-2015-12-31_sents_mentioned_trump.json
- 2016-01-01-to-2016-11-08_sents_mentioned_trump.json

## Params

| Field        | Description           | Type  |
| ------------- |:-------------:| -----:|
| `docs`      | The number of news | Integer |
| `sentences`      | The number of sentences      |  Integer |
| `results` | All the data related to Donald Trump     | List/Array |

##### Within results

| Field        | Description           | Type  |
| ------------- |:-------------:| -----:|
| `publicationDate` | The date of publication      |    String |
| `sentences` | Sentences that include 'Trump'       | String list |
| `tags` | Related tags   | String list |
| `title` | The title of the news  | String |
| `webUrl` | The URL to the web page   | String |

## Example

##### JSON

Let's take a snippet of data in _2016-01-01-to-2016-11-08_sents_mentioned_trump.json_ as an example:

```JSON
{
  "docs": 6029,
  "sentences": 63555,
  "results": [
    {
      "publicationDate": "2016-01-01T21:41:19Z",
      "sentences": [
        "Opponents of the Republican presidential frontrunner took to the skies over California on Friday, in order to leave their message: “Anybody but Trump.”    Related: Carly Fiorina tweets support for alma mater's Rose Bowl opponent – Iowa    The message appeared towards the end of the Rose Parade, an annual march through Pasadena, California that is celebrated each New Year’s Day.",
        "Trump is disgusting” and “Iowans dump Trump”, dotted through a cloudless sky.",
        "Though Trump was notified of the skywriting through his Twitter account, as of Friday afternoon he had not responded.",
        "Trump trails Texas senator Ted Cruz in most polls concerning the Republican presidential field in Iowa.",
        "The anti-Trump messages did not represent the only politicking of the afternoon."
      ],
      "tags": [
        "Donald Trump",
        "California",
        "US news",
        "US politics",
        "US elections 2016",
        "Republicans"
      ],
      "title": "'Trump is disgusting': skywriters leave message high above Rose Parade",
      "webUrl": "https://www.theguardian.com/us-news/2016/jan/01/trump-is-disgusting-skywriters-rose-parade-california"
    },
    {
      "publicationDate": "2016-01-02T01:25:42Z",
      "sentences": [
        "Historically, the most striking thing about the campaign so far is not Trump’s ascension, but the fact that a self-proclaimed socialist is running a close race with heir apparent Hillary Clinton.",
        "Sanders, much more than Trump, is a pure-bred social media phenomenon.",
        "Trump has obviously used Twitter effectively, but his name recognition derives from network television and his real estate empire.",
        "And there is ample precedent for the Trump candidacy; in a sense, The Donald is a fusion of the two dark horses from the 1992 campaign: nativist outsider Pat Buchanan and eccentric billionaire Ross Perot.",
        "An observer of that 1992 campaign would hardly blink an eye at the premise that a Trump-like figure might play a role in future presidential campaigns.",
        "Perhaps we are just at the beginning stages of the social media revolution, and in two years President Trump will be building his gold-plated wall along the Mexican border."
      ],
      "tags": [
        "Politics and technology",
        "Facebook",
        "Social media",
        "Social networking",
        "Technology",
        "US politics",
        "Media",
        "US news",
        "Digital media"
      ],
      "title": "Is Facebook the enemy of truth and civic unity?",
      "webUrl": "https://www.theguardian.com/technology/2016/jan/01/facebook-truth-trump-obama"
    },
  ]   
}
```
