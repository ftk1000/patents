2026.08.12

* https://chatgpt.com/c/6a7cf03b-d290-83ea-9740-00238c99f947

# Q

remind me how to find the list of all my patents on USPTO site?

# A 

Yes. The easiest way is USPTO’s **Patent Public Search**, rather than Patent Center. USPTO specifically supports searching patents and published applications by inventor name. ([USPTO][1])

### Steps

1. Open [USPTO Patent Public Search](https://ppubs.uspto.gov/pubwebapp/external.html?page=quick.html&type=quick&utm_source=chatgpt.com).
2. Use **Basic Search** initially.
3. Select **Inventor Name** as the search field.
4. Enter your name. If necessary, try variants such as:

   * `Khafizov Farid`
   * `Farid Khafizov`
   * just `Khafizov`
5. Make sure both **US-PGPUB** (published applications) and **USPAT** (issued patents) are selected. This is important if you want more than just granted patents. ([USPTO Publications][2])

For a cleaner search, use **Advanced Search** and search specifically by inventor. USPTO has a short tutorial devoted to exactly this: [USPTO: Search by inventor name](https://www.uspto.gov/learning-and-resources/uspto-videos/search-inventor-name?utm_source=chatgpt.com).

If you want, I can also **find your USPTO patents now and give you a table with patent number, title, filing date, grant date, and co-inventors**.

[1]: https://www.uspto.gov/patents/search/patent-public-search?utm_source=chatgpt.com "Patent Public Search | USPTO"

[2]: https://ppubs.uspto.gov/pubwebapp/external.html?page=quick.html&type=quick&utm_source=chatgpt.com "Patent Public Search | USPTO"


---------


# Q

where to specify inventor name

# A 

You're in the **Advanced Search** interface, so there isn't a separate "Inventor Name" box.

In the large search box where you currently have:

`Farid Khafizov Plano`

replace it with:

```text
"Farid Khafizov".IN.
```

Here `.IN.` means **Inventor Name**.

I would actually start broader with:

```text
Khafizov.IN.
```

Then click **Search**.

Also, on the right under **Databases**, check both:

* **US-PGPUB** — published patent applications
* **USPAT** — granted U.S. patents

If you want, I can also show you the **best query for finding all patents where you are an inventor, including name variations, while excluding unrelated Khafizovs**.




---------


# Q


where to specify that I live in Plano TX


# A 

In USPTO Patent Public Search, you generally **don't need to specify your residence** to find your patents. Search by inventor name first:

```text
"Farid Khafizov".IN.
```

If you want to use **Plano, Texas** to distinguish yourself from another inventor with the same name, the search syntax can include inventor city/state fields, but those fields depend on the USPTO search-field syntax.

I can look up the exact current USPTO query syntax for **Inventor = Farid Khafizov AND City = Plano AND State = TX** so you can paste it directly into that box.



---------


# Q


yes

# A 


Yes. I checked the current USPTO field codes. In the **Advanced Search** box you can specify inventor name, city, and state separately.

For your case, try:

```text
(Farid AND Khafizov).IN. AND Plano.INCI. AND TX.INST.
```

The fields mean:

* `.IN.` = **Inventor Name**
* `.INCI.` = **Inventor City**
* `.INST.` = **Inventor State** (two-letter code)

These are the current USPTO Patent Public Search field codes. ([USPTO][1])

I would actually try this slightly simpler query first:

```text
Khafizov.IN. AND Plano.INCI. AND TX.INST.
```

Then select **USPAT** for granted patents. Also select **US-PGPUB** if you want published applications as well.

One important point: the city/state are the inventor address **recorded on that particular patent**, so if some of your older patents list another city, restricting to `Plano` will cause those patents to disappear. Therefore, to get **all** of your patents, I recommend first searching:

```text
(Farid AND Khafizov).IN.
```

and then using Plano/TX only to resolve ambiguous results. ([USPTO][1])

[USPTO Patent Public Search field codes](https://www.uspto.gov/patents/search/patent-public-search/searchable-indexes?utm_source=chatgpt.com)

[1]: https://www.uspto.gov/patents/search/patent-public-search/searchable-indexes?utm_source=chatgpt.com "Searchable indexes | USPTO"

---------



