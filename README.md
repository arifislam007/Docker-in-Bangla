## Docker বেসিকস ফর বিগিনার্স

### Docker কি ?
Docker হলো একটি ওপেন-সোর্স প্ল্যাটফর্ম যা ডেভেলপারদের অ্যাপ্লিকেশনগুলি কনটেইনারে প্যাকেজ করতে এবং চালাতে সাহায্য করে, যা সফটওয়্যার ডেভেলপমেন্ট প্রক্রিয়াকে আরও নির্ভুল ও সহজ করে তোলে। Docker ব্যবহার করে, ডেভেলপাররা তাদের অ্যাপ্লিকেশন এবং পরিষেবাগুলি বিভিন্ন পরিবেশে একই ভাবে চালাতে পারেন, যা সহজে পোর্টেবলিটি এবং স্কেলিং সুবিধা প্রদান করে।

---

### Docker এর মূল ধারণাগুলি:
#### কনটেইনার: 
   Docker কনটেইনারগুলি হল লাইটওয়েট, পোর্টেবল কম্পিউটেশনাল প্যাকেজ যা একটি অ্যাপ্লিকেশন এবং এর সমস্ত নির্ভশীল অন্যান প্যাকেজগুলো ধারণ করে।
#### ইমেজ: 
   Docker ইমেজগুলি হলো রিড-অনলি টেমপ্লেট যা কনটেইনার তৈরির জন্য ব্যবহৃত হয়। 
#### ডকারফাইল: 
   এটি একটি স্ক্রিপ্ট যা Docker ইমেজ তৈরির পদ্ধতিগুলি নির্ধারণ করে।

---

## Docker ব্যবহারের সুবিধাগুলি

Docker টেকনোলজি ডেভেলপারদের এবং সিস্টেম প্রশাসকদের জন্য অনেক সুবিধা প্রদান করে। এর মাধ্যমে সফটওয়্যার ডেভেলপমেন্ট, টেস্টিং, এবং প্রোডাকশন পর্যায়ে বেশ কিছু সমস্যা সমাধান করা যায়। নিচে Docker ব্যবহারের কিছু প্রধান সুবিধা উল্লেখ করা হলো:

### 1. **সহজ কনফিগারেশন:**
   Docker সফটওয়্যার ডেলিভারিকে আরও সহজ করে তোলে কারণ এটি অ্যাপ্লিকেশনের সব নির্ভরতা একটি Docker কনটেইনারে প্যাকেজ করে দেয়। এই কনটেইনার যেকোনো পরিবেশে একইভাবে চলতে সক্ষম।

### 2. **দ্রুত ডেপ্লয়মেন্ট:**
   Docker কনটেইনার চালু হতে মাত্র সেকেন্ড সময় লাগে, যা ভার্চুয়াল মেশিনের তুলনায় অনেক কম সময় যা মিনিট সময় নিতে পারে। এই দ্রুত ডেপ্লয়মেন্ট প্রক্রিয়া ডেভেলপমেন্ট এবং টেস্টিং চক্রকে গতিশীল করে তোলে।

### 3. **পোর্টেবিলিটি:**
   Docker কনটেইনার যেকোনো মেশিনে চালানো যায় যেখানে Docker ইনস্টল করা আছে। এটি ডেভেলপারদের লোকাল মেশিন থেকে প্রোডাকশনে সহজেই কোড ট্রান্সফার করতে দেয়।

### 4. **সার্বজনীনতা:**
   Docker বিভিন্ন লিনাক্স ডিস্ট্রিবিউশন এবং ম্যাক ওএস, উইন্ডোজে সমর্থন করে। এটি প্ল্যাটফর্ম নির্ভরতা কমায় এবং অ্যাপ্লিকেশনের আরও বিস্তৃত ব্যবহার নিশ্চিত করে।

### 5. **স্কেলেবিলিটি এবং ম্যানেজমেন্ট:**
   Docker স্বয়ংক্রিয়ভাবে কনটেইনারগুলির স্কেলিং এবং ম্যানেজমেন্ট করে, যা বড় স্কেলের অ্যাপ্লিকেশনগুলিকে সহজেই হ্যান্ডেল করতে সাহায্য করে। Docker Compose বা Docker Swarm এর মাধ্যমে মাল্টি-কনটেইনার অ্যাপ্লিকেশন ডিপ্লয় করা এবং ম্যানেজ করা যায়, যা প্রোডাকশন পরিবেশে অ্যাপ্লিকেশনগুলির কার্যকারিতা বৃদ্ধি করে।

### 6. **আইসোলেশন:**
   Docker প্রতিটি কনটেইনারকে পৃথক পরিবেশ প্রদান করে যা নিরাপত্তা এবং ডিপেন্ডেন্সি কনফ্লিক্টগুলি এড়িয়ে চলে। এই পৃথকীকরণ নিশ্চিত করে যে একটি কনটেইনারের ক্র্যাশ অন্য কনটেইনারগুলির উপর প্রভাব ফেলবে না।

### 7. **সংস্করণ নিয়ন্ত্রণ এবং রোলব্যাক:**
   Docker ইমেজ সংস্করণ নিয়ন্ত্রণ এবং রোলব্যাক সহজ করে তোলে, যা ডেভেলপারদের পুরানো সংস্করণে ফিরে যাওয়া বা নতুন সংস্করণে আপগ্রেড করা সহজ করে তোলে। এটি প্রযুক্তিগত সমস্যাগুলির সমাধানে দ্রুত পদক্ষেপ নিতে সাহায্য করে।

### 8. **মিনিমাল ওভারহেড:**
   Docker কনটেইনারগুলি খুব কম সম্পদ ব্যবহার করে এবং খুব দ্রুত চালু হয়, যা সার্ভার সম্পদগুলির ব্যবহারকে মিনিমাইজ করে এবং স্কেল করতে এবং ব্যবস্থাপনা করতে সক্ষম, যা বড় স্কেলের অ্যাপ্লিকেশন পরিচালনা করা সহজ করে তোলে। Docker Compose এবং Docker Swarm এর মতো টুলসগুলি একাধিক কনটেইনার চালানো এবং তাদের নেটওয়ার্ক কনফিগারেশন সহজে সেটআপ করতে সাহায্য করে।

---
##  Docker ইমেজ ব্যাখ্যা :

### ১. ডকার ইমেজ কি?
Docker ইমেজ হল একটি রিড-অনলি টেমপ্লেট যা এক বা একাধিক ডকার কনটেইনার তৈরির জন্য ব্যবহার করা হয়। এটি সফটওয়্যার অ্যাপ্লিকেশন, তার নির্ভরতাসমূহ, লাইব্রেরি এবং অন্যান্য কনফিগারেশন ফাইলগুলি ধারণ করে, যা কনটেইনারের রানটাইম পরিবেশ তৈরি করে।

### ২. ডকার ইমেজের লেয়ার বিন্যাস (Layered Architecture):
Docker ইমেজগুলো একটি লেয়ার আর্কিটেকচারে তৈরি হয়। প্রতিটি স্তর পূর্ববর্তী স্তরের উপর নির্মিত হয় এবং পরিবর্তনগুলি নতুন স্তরে সংরক্ষিত হয়। এটি ইমেজ বিল্ড প্রক্রিয়াকে দ্রুত করে তোলে কারণ শুধুমাত্র পরিবর্তিত স্তরগুলিই আপডেট বা পুনর্নির্মাণ করা হয়।

### ৩. ডকারফাইল থেকে ইমেজ তৈরি:
Docker ইমেজগুলি সাধারণত একটি `Dockerfile` থেকে তৈরি করা হয়, যা একটি টেক্সট ডকুমেন্ট যা বিল্ড কমান্ড এবং প্যারামিটারগুলি ধারণ করে। `Dockerfile` বিল্ড প্রক্রিয়াকে অটোমেটেড করে, যা নির্ভুল এবং পুনরাবৃত্তিযোগ্য ইমেজ তৈরি করে।

### ৪. ইমেজ সংরক্ষণাগার (Registry):
Docker ইমেজগুলো ডকার হাব বা অন্যান্য প্রাইভেট রেজিস্ট্রিতে সংরক্ষিত হয়। ডকার হাব একটি পাবলিক রেজিস্ট্রি যেখানে কেউ তার ইমেজ আপলোড করতে পারে এবং অন্যান্য ডেভেলপাররা এই ইমেজগুলি ডাউনলোড করতে পারে।

### ৫. ইমেজ ব্যবহার এবং ডিস্ট্রিবিউশন:
Docker ইমেজগুলি ব্যবহার করে কনটেইনার চালু করা হয় এবং এক Environment থেকে অন্য Environment সহজে মাইগ্রেট করা যায়। এই পোর্টেবিলিটি ডেভেলপারদের প্রোডাকশন, টেস্টিং, এবং ডেভেলপমেন্ট প্রক্রিয়াগুলোর মধ্যে অ্যাপ্লিকেশনগুলির সাথে কাজ করা সহজ করে তোলে।

---

## Docker অ্যপলিকেশন ডেভলপমেন্ট: 

একটি বেসিক ওয়েব সার্ভিসের জন্য যা "Hello World" প্রদর্শন করে, তার একটি Dockerfile তৈরি করার প্রক্রিয়া ব্যাখ্যা করা হলো। এখানে আমরা Node.js ব্যবহার করব, কারণ Node.js সাধারণত ওয়েব অ্যাপ্লিকেশনগুলি তৈরির জন্য জনপ্রিয়।

### প্রথমে, আপনার প্রজেক্ট ডিরেক্টরিতে একটি `Dockerfile` তৈরি করুন:
```
mkdir myproject
cd myproject
vi Dockerfile
```
### তারপার নিচের কন্টেন্টটি কপি করে Dockerfile এ পেষ্ট করুন। 

```dockerfile
# বেস ইমেজ নির্ধারণ করুন
FROM node:14-alpine

# আপনার অ্যাপ্লিকেশন কোড রাখার জন্য ওয়ার্কিং ডিরেক্টরি তৈরি করুন
WORKDIR /usr/src/app

# আপনার প্যাকেজ ফাইলগুলি কপি করুন
COPY package*.json ./

# নির্ভরতা ইনস্টল করুন
RUN npm install

# আপনার অ্যাপ্লিকেশন সোর্স কোড কপি করুন
COPY . .

# অ্যাপ্লিকেশন চালানোর জন্য পোর্ট খুলুন
EXPOSE 3000

# অ্যাপ্লিকেশন রান করার কমান্ড সেট করুন
CMD ["node", "app.js"]
```

### পরবর্তীতে, `app.js` ফাইলে নিম্নলিখিত Node.js কোড লিখুন:

```javascript
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hello World!');
});

app.listen(3000, () => {
  console.log('Application is running on http://localhost:3000');
});
```

### এবং `package.json` ফাইলে নিম্নলিখিত কনফিগারেশন যোগ করুন:

```json
{
  "name": "hello-world-app",
  "version": "1.0.0",
  "description": "A simple Node.js app displaying 'Hello World'",
  "main": "app.js",
  "scripts": {
    "start": "node app.js"
  },
  "dependencies": {
    "express": "^4.17.1"
  }
}
```

এই Dockerfile এবং কোডের মাধ্যমে আপনি একটি সাধারণ "Hello World" ওয়েব সার্ভিস তৈরি করতে পারবেন যা Docker কনটেইনারে চালিত হবে।


---
## Docker ভলিউমস 
Docker স্টোরেজ একটি জটিল বিষয় যা Docker কনটেইনারের ডেটা স্থায়ীত্বকরন ও ম্যানেজমেন্ট সম্পর্কিত। Docker স্টোরেজ ডেটা ব্যবস্থাপনা করার জন্য মূলত তিনটি উপায় প্রদান করে: ভলিউমস (Volumes), বাইন্ড মাউন্টস (Bind Mounts), এবং tmpfs মাউন্টস (tmpfs mounts)।

### ১. ভলিউমস (Volumes):
- **ভলিউমস** হল Docker দ্বারা পরিচালিত স্টোরেজ যা হোস্ট মেশিনের ফাইল সিস্টেমের নির্দিষ্ট ফাইল সিস্টেমের সাথে সংরক্ষিত হয়। 
- এগুলি ডেটাকে কনটেইনার বাইরে সংরক্ষণ করে যা কনটেইনার রিস্টার্ট হলেও স্থায়ী থাকে এবং একাধিক কনটেইনারের মধ্যে ভাগ করা যায়।
- এটি বিশেষ করে ডাটাবেসের মতো স্টেটফুল অ্যাপ্লিকেশনের জন্য উপযুক্ত।

### ২. বাইন্ড মাউন্টস (Bind Mounts):
- **বাইন্ড মাউন্টস** সরাসরি হোস্ট মেশিনের ফাইল সিস্টেমের কোনো অংশকে কনটেইনারের সাথে ম্যাপ করে।
- এই পদ্ধতিতে কনটেইনার থেকে সরাসরি হোস্ট মেশিনের ফাইলগুলি পড়া ও লেখা যায়।
- ডেভেলপমেন্ট পরিবেশে এই পদ্ধতি খুবই জনপ্রিয়, যেখানে ডেভেলপাররা কোড পরিবর্তন সরাসরি হোস্ট মেশিনে দেখতে চান।

### ৩. tmpfs মাউন্টস (tmpfs mounts):
- **tmpfs মাউন্টস** মেমরি-ভিত্তিক স্টোরেজ

 প্রদান করে যা কনটেইনার বন্ধ হলে ডেটা মুছে ফেলা হয়।
- এটি সেনসিটিভ ডেটা যেমন পাসওয়ার্ড বা কী সংরক্ষণের জন্য উপযুক্ত নয়, কিন্তু টেম্পোরারি ডেটা স্টোরেজের জন্য আদর্শ। এটি হোস্ট মেশিনের মেমরির সাথে যুক্ত থাকে তাই এটি অ্যপলিকেশনের পারফরমেন্স বাড়িয়ে দেয়। 

Docker স্টোরেজ কনফিগারেশন এবং ম্যানেজমেন্ট কনটেইনারাইজড অ্যাপ্লিকেশনের স্কেলিং, পোর্টেবিলিটি এবং নিরাপত্তা নিশ্চিত করে। Docker কমান্ড লাইন ইন্টারফেস বা Docker Compose ফাইলের মাধ্যমে এই সব স্টোরেজ অপশন কনফিগার করা যায়, যা ডেভেলপারদের অ্যাপ্লিকেশন ডেপ্লয়মেন্ট প্রক্রিয়াকে সহজ করে তোলে।

----
## Docker নেটওয়ার্কিং
Docker নেটওয়ার্কিং একটি গুরুত্বপূর্ণ অংশ যা Docker কন্টেইনারগুলির মধ্যে যোগাযোগ স্থাপন এবং বাইরের নেটওয়ার্কের সাথে ইন্টারফেস করার ক্ষমতা প্রদান করে। এটি বিভিন্ন প্রকারের নেটওয়ার্ক ড্রাইভারের মাধ্যমে কাজ করে, যা বিভিন্ন ধরনের যোগাযোগ পরিস্থিতির জন্য উপযুক্ত।
### Docker নেটওয়ার্কিং ধরনগুলি:
1. **ব্রিজ (Bridge) নেটওয়ার্ক:**
   - ডিফল্ট নেটওয়ার্ক ড্রাইভার। যখন আপনি Docker ইনস্টল করেন, তখন একটি ব্রিজ নেটওয়ার্ক অটোম্যাটিকভাবে তৈরি হয়।
   - এটি একই Docker হোস্টের মধ্যে কন্টেইনারগুলির মধ্যে প্রাইভেট ইন্টারনাল নেটওয়ার্ক তৈরি করে।

2. **হোস্ট (Host) নেটওয়ার্ক:**
   - এই ড্রাইভার কন্টেইনারকে হোস্ট মেশিনের নেটওয়ার্ক পরিবেশের সাথে সরাসরি যুক্ত করে।
   - এটি পারফরম্যান্স উন্নতি সাধন করে কিন্তু নিরাপত্তা প্রশ্ন তৈরি করতে পারে।

3. **ওভারলে (Overlay) নেটওয়ার্ক:**
   - এটি মাল্টি-হোস্ট নেটওয়ার্কিং সাপোর্ট করে, যা Docker Swarm বা Kubernetes এর মতো অর্কেস্ট্রেশন সল্যুশনের সাথে ব্যবহার করা হয়।
   - ওভারলে নেটওয়ার্ক বিভিন্ন হোস্টের উ

পর চালিত কন্টেইনারগুলির মধ্যে যোগাযোগ সক্ষম করে।

4. **নান (None) নেটওয়ার্ক:**
   - এই নেটওয়ার্ক ড্রাইভার কন্টেইনারকে কোনো নেটওয়ার্কে যুক্ত করে না।
   - এটি সুরক্ষা-কেন্দ্রিক অ্যাপ্লিকেশনের জন্য উপযুক্ত যেখানে নেটওয়ার্ক বিচ্ছিন্নতা প্রয়োজন।

### নেটওয়ার্ক কনফিগারেশন:
- Docker কন্টেইনারের নেটওয়ার্ক কনফিগারেশন `docker network` কমান্ডের মাধ্যমে করা হয়।
- নেটওয়ার্ক তৈরি, মুছে ফেলা, এবং ইন্সপেক্ট করার জন্য বিভিন্ন কমান্ড রয়েছে।

### উদাহরণ:
একটি নতুন ব্রিজ নেটওয়ার্ক তৈরি করতে:
```bash
docker network create --driver bridge my-bridge-network
```
একটি কন্টেইনার চালানোর সময় এটি এই নেটওয়ার্কে যুক্ত করতে:
```bash
docker run -d --name my-container --network my-bridge-network nginx
```

Docker নেটওয়ার্কিং ডেভেলপারদের বিভিন্ন হোস্ট এবং পরিবেশের মধ্যে সহজে কন্টেইনার মাইগ্রেট করতে এবং সহজে স্কেল করতে সাহায্য করে, যা অ্যাপ্লিকেশনের নিরবচ্ছিন্নতা এবং কার্যকারিতা নিশ্চিত করে।
