এইটি লারাভেল ৫.৩ দিয়ে বানানো একটি হল ম্যানেজমেন্ট অ্যাপ। এই প্রজেক্টটি সবার জন্য উন্মুক্ত করা হয়েছে, আশা করি এর মাধ্যমে সবাই উপকৃত হবেন। প্রয়োজনে কেউ কন্ট্রিবিউট করতে পারেন। কেউ আশা করি কোন অংশ না বুঝলে আমাকে অবশ্যই জানাবেন। এই ম্যানেজমেন্ট অ্যাপ এর টেমপ্লেট হিসেবে admin lte ব্যাবহার করা হয়েছে।

এই অ্যাপের ফিচারগুলোঃ-

১। ৩ ধরনের user রয়েছে; প্রভোস্ট(admin), হল স্টাফ(employee), ছাত্র(student)। ACL এর ব্যাবস্থা রয়েছে। অর্থাৎ admin যে কারো user role পরিবর্তন করতে পারবেন বা user কে delete করতে পারবেন।

২। প্রত্যেক user কোন কোন ছাত্র হলে অবস্থান করে তা দেখতে পারবে, প্রত্যেক ছাত্রদের প্রোফাইল দেখতে পারবে। এইক্ষেত্রে ছাত্রদের রোল নং দিয়ে search এর জন্য ajax ব্যাবহার করা হয়েছে। floor ভিত্তিক pagination ব্যাবহার করা হয়েছে, অর্থাৎ ১ম তলা একটি page, ২য় তলা ২য় page।

৩। শুধুমাত্র হল স্টাফ আর প্রভোস্টরা registration করতে পারবে। হল স্টাফরা ছাত্রদের আর প্রভোস্টরা সবাইকে  register করতে পারবে।

৪। প্রত্যেক user তাদের নিজস্ব password পরিবর্তন করতে পারবেন। তবে admin সবার password পরিবর্তন করতে পারবেন।

৫। হল স্টাফ এবং প্রভোস্ট যেকোনো ছাত্রের প্রোফাইল edit করতে পারবেন। চাইলে তাদেরকে delete করতে পারবেন।

৬। প্রত্যেক user এই মাসের হল ম্যানেজার কারা, তাদের প্রোফাইল দেখতে পারবে। সাথে হল স্টাফ আর প্রভোস্টদের লিস্ট-ও দেখতে পারবে। এর ফলে যেকোন প্রয়োজনে যাতে তাদের সাথে যোগাযোগ করতে পারে।

৭। প্রত্যেকের নিজস্ব প্রোফাইল আছে আর এই প্রোফাইল তারা edit করতে পারবে।

৮। প্রত্যেক মাসের জন্য হল স্টাফ আর প্রভোস্টরা হল ম্যানেজার বাছাই করতে পারবেন ছাত্রদের মধ্য থেকে।

৯। প্রত্যেক রুমের জন্য সর্বাধিক কতজন থাকতে পারবেন তা নির্ধারণ করে দিতে পারবেন। এই ছাড়া প্রত্যেক রুমে সর্বাধিকের চেয়ে অতিরিক্ত বা কম আছে তা ছাত্রদের লিস্টে দেখা যাবে।

প্রজেক্টি কিভাবে run করবেনঃ-

প্রজেক্ট রানে জন্য পুরা প্রজেক্টটি git থেকে clone করুন বা download করুন। এরপর .env বানিয়ে সেইখানে database এর নাম, username, password ঠিক করুন।

এরপর নিচের command গুলো run করুন

composer install

php artisan key:generate

php artisan migrate:refresh –-seed

php artisan serve
অবশ্যই প্রজেক্টের কোন অংশ না বুঝলে জানাবেন। আর এইটি একটি ফ্রি প্রজেক্ট, তাই এইটি দিয়ে উপকৃত হওয়ার চেষ্টা করুন। কেউ এই প্রজেক্ট দিয়ে ব্যাবসায়িক কিছু করা থেকে বিরত থাকবেন।
