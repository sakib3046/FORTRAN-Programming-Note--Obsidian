### ফোরট্রান প্রোগ্রাম তৈরি এবং চালানো মূলত দুটি ধাপে সম্পন্ন হয়: কম্পাইল (compilation    ) এবং চালানো (execution)।



### আগে যা হবে -
- টেক্সট এডিটর (Text Editor)
- ফাইল এক্সটেনশন সম্পর্কে জানতে


## Text Editor
যে সফটওয়্যারে প্রোগ্রামিং ল্যাঙ্গুয়েজ লেখা হয় তাকে টেক্সট এডিটর বলা হয়। টেক্সট এডিটর এর মাধ্যমে কম্পাইলারের সাথে সম্পর্ক স্থাপন করে লিখিত কোড কে বিল্ড ও রান করা যায়।

![[Pasted image 20240527225220.png |100]] ![[Pasted image 20240527225318.png| 100]]    ![[Pasted image 20240527225435.png |300]]



## **১. কোড লেখা :**
- যেকোনো টেক্সট এডিটরে তোমার কোডটি লেখতে হবে।
- সঠিক ফাইল এক্সটেনশন দিয়ে ফাইল সেভ করা 


## **২. কম্পাইল করা:**

- **কম্পাইলার:** আপনার মানবদ্বারা বোঝা যায় এমন কোড (সোর্স কোড) কে কম্পিউটার বুঝতে পারে এমন মেশিন কোডে রূপান্তর করতে ফোরট্রান কম্পাইলারের দরকার। কিছু জনপ্রিয় বিনামূল্যের কম্পাইলার হলো জিএনইউ ফোরট্রান (gfortran) এবং ওপেন ফোরট্রান (openf95)।
- **কোড কম্পাইল করা:** আপনার ফোরট্রান সোর্স কোড ফাইল (সাধারণত `.f` ,`.f77` বা `.f95` এক্সটেনশান থাকে) কম্পাইল করতে কম্পাইলারের কমান্ড লাইন ইন্টারফেস ব্যবহার করুন।

![[Compiler.png]]
**ফোরট্রান  কম্পাইলার**
ফোরট্রান কম্পাইলার হলো একধরণের বিশেষ সফটওয়ার প্রোগ্রাম যা মানুষের বোঝা যায় এমন ফোরট্রান কোড (সোর্স কোড) কে কম্পিউটার বুঝতে পারে এমন মেশিন কোডে রূপান্তর করে। এটি প্রোগ্রামার এবং কম্পিউটারের মাঝে সেতুবন্ধনের মতো কাজ করে।
ফোরট্রান কোড নিজেই সরাস্কভাবে কম্পিউটার দ্বারা বোঝা যায় না। কম্পাইলার দ্বারা জেনারেটেড মেশিন কোড কম্পিউটারকে নির্দেশাবলী প্রক্রিয়াজাত করতে এবং আপনার প্রোগ্রামে সংজ্ঞায়িত গণনা বা কাজগুলি সম্পাদন করতে দেয়।


## **৩. চালানো:**

- **এক্সিকিউটেবল চালানো:** একবার কম্পাইল হয়ে গেলে, আপনি তৈরি করা প্রোগ্রাম ফাইল (সাধারণত উইন্ডোজে `.exe` এক্সটেনশান বা লিনাক্স/ম্যাকওএস এ শুধু ফাইলের নাম) চালাতে পারবেন।
![[exe.png]]