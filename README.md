# CodeT5 و CodeT5+

انتشار رسمی تحقیقاتی برای مدل‌های **CodeT5** و **CodeT5+** برای **درک و تولید کد** از Salesforce Research، که در مقالات زیر معرفی شده‌اند:

*عنوان*: [CodeT5+: مدل‌های بزرگ زبان کد باز برای درک و تولید کد](https://arxiv.org/pdf/2305.07922.pdf)

> *نویسندگان*: [Yue Wang](https://yuewang-cuhk.github.io/)\*, [Hung Le](https://sites.google.com/view/henryle2018/home?pli=1)\*, [Akhilesh Deepak Gotmare](https://akhileshgotmare.github.io/), [Nghi D.Q. Bui](https://bdqnghi.github.io/), [Junnan Li](https://sites.google.com/site/junnanlics), [Steven C.H. Hoi](https://sites.google.com/view/stevenhoi/home) (* نشان‌دهنده مشارکت برابر است)

*عنوان*: [CodeT5: مدل‌های یکپارچه پیش‌آموخته Encoder-Decoder با آگاهی از شناسه‌ها برای درک و تولید کد](https://arxiv.org/pdf/2109.00859.pdf)

> *نویسندگان*: [Yue Wang](https://yuewang-cuhk.github.io/), [Weishi Wang](https://www.linkedin.com/in/weishi-wang/), [Shafiq Joty](https://raihanjoty.github.io/), [Steven C.H. Hoi](https://sites.google.com/view/stevenhoi/home)

در عمل، مدل‌های CodeT5 و CodeT5+ می‌توانند به عنوان یک دستیار کدنویسی مبتنی بر هوش مصنوعی برای افزایش بهره‌وری توسعه‌دهندگان نرم‌افزار مستقر شوند. در Salesforce، ما یک دموی دستیار کدنویسی هوش مصنوعی با استفاده از CodeT5 به عنوان یک پلاگین VS Code ساخته‌ایم که سه قابلیت ارائه می‌دهد:

- **تولید کد از متن**: تولید کد بر اساس توصیف زبان طبیعی.
- **تکمیل خودکار کد**: تکمیل کل تابع کد با توجه به نام تابع هدف.
- **خلاصه‌سازی کد**: تولید خلاصه‌ای از یک تابع در توصیف زبان طبیعی.

![دموی CodeT5](./codet5.gif)

## چه چیز جدیدی است: 🎉

**مه 2023**

مقاله و مدل‌های **CodeT5+** منتشر شدند! 🔥 <br>
[مقاله](https://arxiv.org/pdf/2305.07922.pdf) | [کد](https://github.com/salesforce/CodeT5/tree/main/CodeT5+) | [مدل](https://huggingface.co/models?sort=downloads&search=codet5p) | [وبلاگ](https://blog.salesforceairesearch.com/codet5-open-code-large-language-models/)

**سپتامبر 2022**

مقاله **CodeRL** ما در NeurIPS 2022 پذیرفته شد! <br>
[مقاله](https://arxiv.org/pdf/2207.01780.pdf) | [کد](https://github.com/salesforce/CodeRL) | [وبلاگ](https://blog.salesforceairesearch.com/coderl)

**ژوئیه 2022**

ما دو چک‌پوینت بزرگ CodeT5 را در HuggingFace منتشر کردیم: [Salesforce/codet5-large](https://huggingface.co/Salesforce/codet5-large) و [Salesforce/codet5-large-ntp-py](https://huggingface.co/Salesforce/codet5-large-ntp-py)، که در [مقاله CodeRL](https://arxiv.org/pdf/2207.01780.pdf) معرفی شده‌اند.

**اکتبر 2021**

ما [چک‌پوینت‌های fine-tuned](https://console.cloud.google.com/storage/browser/sfr-codet5-data-research/finetuned_models) را برای تمامی وظایف پایین‌دستی که در مقاله پوشش داده شده‌اند، منتشر کردیم. علاوه بر این، ما یک چک‌پوینت fine-tuned از CodeT5-base ([Salesforce/codet5-base-multi-sum](https://huggingface.co/Salesforce/codet5-base-multi-sum)) را برای خلاصه‌سازی چندزبانه کد منتشر کردیم.

**سپتامبر 2021**

مقاله **CodeT5** در EMNLP 2021 پذیرفته شد و مدل‌ها منتشر شدند! <br>
[مقاله](https://arxiv.org/pdf/2109.00859.pdf) | [کد](https://github.com/salesforce/CodeT5/tree/main/CodeT5) | [مدل](https://huggingface.co/models?sort=downloads&search=codet5) | [کارت مدل](https://github.com/salesforce/CodeT5/blob/main/CodeT5/CodeT5_model_card.pdf) | [وبلاگ](https://blog.salesforceairesearch.com/codet5/)

## استناد

اگر این کد را برای تحقیقات خود مفید می‌دانید، لطفاً به آن استناد کنید:

```
@inproceedings{
    wang2021codet5,
    title={CodeT5: Identifier-aware Unified Pre-trained Encoder-Decoder Models for Code Understanding and Generation}, 
    author={Yue Wang, Weishi Wang, Shafiq Joty, Steven C.H. Hoi},
    booktitle={EMNLP},
    year={2021},
}

@inproceedings{
    le2022coderl,
    title={CodeRL: Mastering Code Generation through Pretrained Models and Deep Reinforcement Learning},
    author={Le, Hung and Wang, Yue and Gotmare, Akhilesh Deepak and Savarese, Silvio and Hoi, Steven C. H.},
    booktitle={NeurIPS},
    year={2022}
}

@article{
    wang2023codet5plus,
    title={CodeT5+: Open Code Large Language Models for Code Understanding and Generation},
    author={Wang, Yue and Le, Hung and Gotmare, Akhilesh Deepak and Bui, Nghi D.Q. and Li, Junnan and Hoi, Steven C. H.},
    journal={arXiv preprint},
    year={2023}
}
```

## مجوز

این کد تحت مجوز BSD-3 منتشر شده است (برای جزئیات بیشتر به `LICENSE.txt` مراجعه کنید)، اما از کاربران نیز می‌خواهیم که به موارد زیر احترام بگذارند:

این نرم‌افزار نباید برای ترویج یا سود بردن از:

خشونت، نفرت و تفرقه،

تخریب محیط زیست،

سوء استفاده از حقوق بشر، یا

تخریب سلامت جسمی و روانی افراد استفاده شود.

ما از کاربران این نرم‌افزار تشویق می‌کنیم که با ارسال ایمیل به آدرس codeT5@salesforce.com، ما را از کاربردهایی که در آن استفاده می‌کنند مطلع کنند و از [مستندات مناسب](https://arxiv.org/abs/1810.03993) [مستندات](https://www.partnershiponai.org/about-ml/) هنگام توسعه کاربردهای با ریسک بالا از این مدل استفاده کنند.

## مشارکت کنید

لطفاً اگر سوال، پیشنهاد، درخواست یا گزارش اشکالی دارید، یک issue در GitHub ایجاد کنید. ما PRها را نیز می‌پذیریم!
