 User Interface of Wolfram Mathematica
![[Pasted image 20240702014705.png]]
---

## Comments
ম্যাথমেটিকাতে কমেন্ট যোগ করার দুটি প্রধান উপায় রয়েছে:

---

**১.  মাল্টি লাইন কমেন্ট**

প্রথম ব্রাকেট এবং তারকা চিহ্ন  ব্যবহার করে: এটি ম্যাথমেটিকাতে কমেন্ট যোগ করার সবচেয়ে সাধারণ পদ্ধতি. যার মাধ্যমে আমরা একাধিক লাইনের কমেন্ট লিখতে পারি। এটি কীভাবে কাজ করে তা এখানে দেওয়া হল:

---

- `(*` *(খোলা পেরেন্থাসিস এবং তারকা চিহ্ন)* এবং `*)` *(বন্ধ করা তারকা চিহ্ন এবং  পেরেন্থাসিস )* এর মধ্যে স্থাপন করা যেকোনো কিছুই একটি *কমেন্ট* হিসাবে বিবেচিত হবে।
- আপনার কোড মূল্যায়ন করার সময় ম্যাথমেটিকা কমেন্ট করা পাঠ্য সম্পূর্ণরূপে উপেক্ষা করবে।
- লাইনের শুরুতে এই প্রতীকগুলি রেখে আপনি একটি লাইন কোডকে কমেন্ট আউট করতে পারেন।
---

উদাহরণ স্বরূপ:

```
(* এই লাইনটি একটি কমেন্ট *)
x = 5 + 3; (* এটি এক্সপ্রেশনের পরে আরেকটি কমেন্ট *)
Print[x] (* এই লাইনটি x এর মান প্রিন্ট করবে *)
```

---

২. **সিঙ্গেল লাইন কমেন্ট**  
ডবল ফরোয়ার্ড স্ল্যাশ (//) ব্যবহার করে:  এই পদ্ধতিটি কোনো এক্সপ্রেশনের পরে লাইনের বাকি অংশ কমেন্ট আউট করার জন্য উপযোগী। এটি কীভাবে কাজ করে তা এখানে দেওয়া হল:

---

- লাইনে `//` (ডবল ফরোয়ার্ড স্ল্যাশ) এর পরে স্থাপন করা যেকোনো কিছুই একটি কমেন্ট হিসাবে বিবেচিত হবে।
- প্রথম পদ্ধতির মতো, ম্যাথমেটিকা কমেন্ট করা পাঠ্য উপেক্ষা করবে।

---

উদাহরণ স্বরূপ:

```
x = 5 + 3 // এটি এক্সপ্রেশনের পরে একটি কমেন্ট
Print[x] (* এই লাইনটি এখনও x এর মান প্রিন্ট করবে *)
```


---
## ম্যাথমেটিকাতে পার্সেন্ট চিহ্ন (%) এর  কাজ :

পূর্বের গণনার আউটপুটকে নির্দেশ করতে পার্সেন্ট চিহ্ন ব্যবহার করা যেতে পারে। যাইহোক, এই ব্যবহারটি সুপারিশ করা হয় না কারণ এটি বিভ্রান্তিকর এবং ত্রুটিপূর্ণ হতে পারে। ম্যাথমেটিকার একটি বিল্ট-ইন প্রক্রিয়া রয়েছে যা `%` (একক পার্সেন্ট) বা `%%` (ডবল পার্সেন্ট) এর পরে একটি সংখ্যা দ্বারা পূর্বের আউটপুটগুলিকে উল্লেখ করতে পারে, যা সাধারণত আরও স্পষ্ট এবং নির্ভরযোগ্য পদ্ধতি।

---
আগের আউটপুটগুলিকে উল্লেখ করার সুপারিশকৃত পদ্ধতিটির একটি বিশ্লেষণ এখানে দেওয়া হল:

---

- `%` (একক পার্সেন্ট) ঠিক আগের সেলের আউটপুটকে নির্দেশ করে।

---

- `%%` (ডবল পার্সেন্ট) বর্তমান সেলের আগে দ্বিতীয় সেলের আউটপুটকে নির্দেশ করে।
---
