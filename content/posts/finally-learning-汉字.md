---
title: "Finally Learning 汉字"
date: 2022-12-31T03:34:36Z
draft: true
description: "Finally learning 汉字 after 10 years"
type: "post"
tags: ["chinese", "hanzi", "learning", "memory"]
---


Four months ago, I made a [list](https://git.exozy.me/a/website/commit/eed700d00b27b98b182e15d66412741b86e91bb4) of things I wanted to learn, and it's mostly the usual suspects. Rust. Haskell. Object capabilities. Quantum mechanics. Math and physics and CS stuff. And one outlier: 汉字, AKA Chinese characters or Hanzi.

Some background about myself: I was born and live in the US, but both my parents are from China, so naturally I grew up speaking decently fluent Mandarin Chinese. While children who grow up speaking most other languages can also read the language without much effort, *reading* Chinese remained impenetrable to me up until around now. Now I'm not assuming you, the reader, are familiar at all with Chinese or 汉字, so here's a quick primer.

People sometimes describe Chinese characters as fancy pictograms, which is a load of absolute nonsense when you think about it, but isn't totally wrong. For instance, 一 means one, 日 means sun, 山 means mountain, and so on. Obviously, you can't represent anything except the basics with pictograms, so that won't work for a full-blown writing system.

We can get a lot more mileage out of this system by representing words that sound similar with the same character, since Chinese has a lot of homophones and near-homophones. However, then we'll get really confused, since we won't know what word this character is supposed to mean. We can disambiguate by adding a second component to the character, a *semantic* component (also called a radical) in addition to the *phonetic* component. For instance, 青 (qīng) means blue-green, 请 (qǐng) means to ask (this radical means the word has to do with talking), 清 (qīng) means clear (this radical means the word has to do with water), and 情 (qíng) means emotion (this radical means the word has to do with emotions).

Yay! This shouldn't be too hard to learn, right? There are only around 400 different syllables in Mandarin, not counting tones, so that's around 400 different phonetic characters to learn, and then I can guess the meaning and which word it corresponds to based on the radical. Easy!

Not so fast. Most characters were created thousands of years ago, so the phonetics have all shifted and jumbled around over the years while the characters have stayed more or less the same (Yes, simplification is a thing, but it just made the shapes simpler instead of updating them to reflect modern Mandarin phonology). Consider 猜, which you would expect to be pronounced like qing or similar, but nope it's actually cāi. Bonus misery: the radical means the word has to do with animals, which is related to its archaic definition, but definitions have changed over thousands of years too. However, in old Chinese, 青 and 猜 were pronounced [s.r̥]ˤeŋ and sʰlɯː respectively, and although I don't know IPA, I'm guessing they sound similar.

So yeah. Learning 汉字 is like learning a very convoluted representation of old Chinese phonology, that somehow corresponds to modern Mandarin words. Instead of being able to recognize 400 characters, you need to know at least 2000 to be able to read most stuff. Even if you know the 400 most common characters, most sentences contain uncommon characters (like how most English sentences contain uncommon words, or you're just going to be talking about boring stuff all the time), and they're usually important, so you'll have no idea what the sentence means. Fun.

Alright, so now that that's out of the way, time to talk about myself now!

The first step was setting up a Chinese input method, so that I could actually type 汉字, because you can't really type them with just a compose key. I guess you could memorize and input Unicode codepoints if you really hated yourself. I already know Pinyin so I went with Fcitx5 with the Pinyin plugin on my laptop (tip: you can make KDE Plasma manage the input method by selecting Fcitx5 in the "Virtual Keyboard" settings page instead of setting environment variables) and Trime for my Android phone. That took me an unbelievable amount of time to set up, because computers usually only work nicely in English.

I also wrote a flash cards app called [SD](https://git.exozy.me/a/SD) in Go and then [ported it to C](https://git.exozy.me/a/SDC), since spaced repetition is amazing! Usually whenever I see and look up a character, I forget it almost instantaneously, so if I want to remember it for more than 30 seconds, I'll just add it to my flash cards. I decided to seed my deck with the most common 1000 characters, courtesy of [Wiktionary](https://en.wiktionary.org/wiki/Appendix:Mandarin_Frequency_lists/1-1000). This failed badly. I didn't even know some of the words, and the definitions are kinda ridiculous. Plus, it was too much of a grind to grind a 1000-card deck, so I started over with something else.

Obviously, the only way to learn 汉字 is to read a ton of characters, so I followed [@felixsmli@donotban.com](https://donotban.com/@felixsmli) and [@Leeing@mastodon.social](https://mastodon.social/@Leeing) on fedi for Chinese-language posts and it actually worked pretty well, although the posts always had a ton of characters that I didn't recognize. I also found a [surprisingly good song](https://lyricstranslate.com/en/b%C5%8D-l%C3%AD-x%C4%ABn-fragile.html) filled with lots of double meanings which even more surprisingly was quite useful for reading. I added any character from the readings that I expected to come up again in the future, and my deck has ballooned now to 400 cards. I like practicing the cards whenever I'm bored and want to go on fedi or Lobsters (the better Hacker News), since I feel like I'm actually being productive instead of just draining my time away reading random discussions (although random fedi posts have changed my life twice: the [Gitea federation fuding post](https://social.gitea.io/@gitea/107576791626052697), and the MIT Mastodon call for help post which has since then been deleted).

I initially used [Lingva Translate](https://lingva.ml/) for translating characters I didn't recognize, but I switched to a combination of Wiktionary, the [Zhongwen browser extension](https://github.com/cschiller/zhongwen), and [Dong Chinese](https://www.dong-chinese.com/dictionary/search). I'm still looking for a libre Android app that'll let me scan a Chinese character with my camera and then OCR it and get the definition. There's an Android app called Hanping for this, but I'll try searching a bit longer for a libre app before shelling out $10 for this one.

I also have a lot of Chinese-language books from when I tried learning 汉字 many years ago, which failed, but I still have the books, so yay! I worked through an entire book over winter break!

Looking back, the number one reason my previous attempts failed was due to not using spaced repetition and flash cards. This totally works, trust me. Also, I'm a lot more personally motivated to learn 汉字 now, whereas in the past, my parents were part of the reason I tried to learn it. This time, I'm surprised at how fun this can get and all the amazing aha moments that I had. I thought this would just be a tedious memory exercise, but I get to read all sorts of cool stuff!

Looking forwards, I still have a long way to go. I know the most common 500-1000 characters by now, but there are still thousands of uncommon characters that'll stump me. My reading speed in Chinese has got to be 10 times slower than in English, but that might be because I usually quickly gloss over English text and reassemble the words in my brain in a way that makes sense. I don't know how useful learning 汉字 will be (bad idea: reading the [over 100000 articles on Moegirlpedia](https://zh.moegirl.org.cn/Special:统计)), but it was definitely worth the ride.

