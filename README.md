<h2 align='center'>TikTok-Teller: A TikTok Video Scraping and Content Analysis Tool</h2>


<p align='center'><img src='https://github.com/jestlandia/tiktok-teller/blob/main/tiktok-teller.png' alt="Tiktok-Teller" width='50%;' ></p>

#### Description:

Search & download Tiktok videos by username and/or video tag, and analyze video contents. Transcribe video speech to text and perform NLP analysis tasks (e.g., keyword and topic discovery; emotion/sentiment analysis). Isolate audio signal and perform signal processing analysis tasks (e.g., pitch, prosody and sentiment analysis). Isolate visual stream and perform image tasks (e.g., object detection; face detection).

---

### Installation & Use

- Clone or download .zip of `tiktok-teller` python package.
```
git clone https://github.com/jestlandia/tiktok-teller.git
```

- Create a virtual environment inside the `tiktok-teller` directory.
```
cd tiktok-teller && python3 -m venv .venv 
```

- Activate virtual environment.  
```
source .venv/bin/activate
```

- Install package dependencies. 
```
pip install -r requirements.txt
```

- Execute `tiktok-teller` program.
```
python src/tiktok-teller.py
```

--- 

### Example 

See [example_data](https://github.com/jestlandia/tiktok-teller/tree/main/example_data) for more information.

![Example Face Recognition](https://github.com/jestlandia/tiktok-teller/blob/main/example_data/Snaptik.app_7261314534885870894.cv__output.gif)

```
Filename: /Users/jest/Snaptik.app_7261314534885870894.mp4

Text:  If you're a man, if you go watch the movie Barbie, you're 100% of beta. No, no, I can't come see the new Barbie movie. The sky fell on TikTok, you mostly post half naked videos. Talk me then, I'm not allowed. Yeah, yeah, I'm an alpha male.

Tokens: ['if', 'you', 'a', 'man', 'if', 'you', 'go', 'watch', 'the', 'movie', 'barbie', 'you', 'of', 'beta', 'no', 'no', 'i', 'can', 'not', 'come', 'see', 'the', 'new', 'barbie', 'movie', 'the', 'sky', 'fell', 'on', 'tiktok', 'you', 'mostly', 'post', 'half', 'naked', 'videos', 'talk', 'me', 'then', 'i', 'not', 'allowed', 'yeah', 'yeah', 'i', 'an', 'alpha', 'male']

Lemmas: ['if', 'you', 'a', 'man', 'if', 'you', 'go', 'watch', 'the', 'movie', 'barbie', 'you', 'of', 'beta', 'no', 'no', 'I', 'can', 'not', 'come', 'see', 'the', 'new', 'barbie', 'movie', 'the', 'sky', 'fall', 'on', 'tiktok', 'you', 'mostly', 'post', 'half', 'naked', 'video', 'talk', 'I', 'then', 'I', 'not', 'allow', 'yeah', 'yeah', 'I', 'an', 'alpha', 'male']

Determiners (Dets): ['a', 'the', 'the', 'the', 'an']

Nouns: ['man', 'movie', 'barbie', '%', 'beta', 'barbie', 'movie', 'sky', 'videos', 'male']

Verbs: ['go', 'watch', 'come', 'see', 'fall', 'post', 'talk', 'allow']

Adjectives (Adjs): ['new', 'tiktok', 'half', 'naked', 'alpha']

Adverbs (Advs): ['mostly', 'then']

Noun Phrases: ['you', 'a man', 'you', 'the movie barbie', 'you', '100%', 'beta', 'i', 'the new barbie movie', 'the sky', 'you', 'half naked videos', 'me', 'i', 'i', 'an alpha male']

Prepositional Phrases: ['of %', 'on fell']

Verb Phrases: ['go watch', 'watch', 'come see', 'see', 'fell', 'fell mostly post', 'talk then', 'talk then allowed']

Emotion: Words: []

Sentence:  If you're a man, if you go watch the movie Barbie, you're 100% of beta.
Sentiment Score: 0.0
Has Emotion: False
Is Derogatory: False
Derogatory Score: 0.00
Polarity: 0.0
Subjectivity: 0.0
Emotion_words: []
------------------------------

Sentence: No, no, I can't come see the new Barbie movie.
Sentiment Score: -0.5267
Has Emotion: False
Is Derogatory: False
Derogatory Score: 0.00
Polarity: 0.13636363636363635
Subjectivity: 0.45454545454545453
Emotion_words: [(['new'], 0.13636363636363635, 0.45454545454545453, None)]
------------------------------

Sentence: The sky fell on TikTok, you mostly post half naked videos.
Sentiment Score: 0.0
Has Emotion: False
Is Derogatory: False
Derogatory Score: 0.00
Polarity: 0.11111111111111112
Subjectivity: 0.35555555555555557
Emotion_words: [(['mostly'], 0.5, 0.5, None), (['half'], -0.16666666666666666, 0.16666666666666666, None), (['naked'], 0.0, 0.4, None)]
------------------------------

Sentence: Talk me then, I'm not allowed.
Sentiment Score: 0.0
Has Emotion: False
Is Derogatory: False
Derogatory Score: 0.00
Polarity: 0.0
Subjectivity: 0.0
Emotion_words: []
------------------------------

Sentence: Yeah, yeah, I'm an alpha male.
Sentiment Score: 0.5267
Has Emotion: False
Is Derogatory: False
Derogatory Score: 0.00
Polarity: 0.0
Subjectivity: 0.1
Emotion_words: [(['male'], 0.0, 0.1, None)]
------------------------------
```
