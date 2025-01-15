# 🌐 Filimo Android Assignment

Welcome to the **Filimo Android Assignment**! This assignment is designed to evaluate your skills, problem-solving ability, and technical workflow. Let’s see how you approach building an Android app using the Filimo API! 

> ⏳ **Time Limit:** Aim to complete the assignment within 8 hours.

---

## 📖 Assignment Overview

Your task is to create a simple test app that uses the **Filimo API** for search functionality. Don’t stress too much about the UI—an input field and a list to display results will suffice! We’re more interested in:

- The architecture and design patterns you use.
- The clarity and organization of your code.

---

## 🕊️ Deliverables

Here’s what we’d like you to include in your submission:

1. **Source Code:** Share your project in a Github repository.
2. **Runnable APK:** Provide an archived version of the app (.apk file) so we can test it easily.
3. **README Instructions:** Add clear instructions on:
   - How to run the app.
   - How to test the solution.
   - Required software and versions.
4. **Assumptions:** Document any assumptions you made during development and explain the reasoning.
5. **Extras:** Include anything that might speed up the review process or showcase your skills.

---

## 🔍 Filimo Search API Details

Use the following API to fetch search results:

```http
GET https://www.filimo.com/api/en/v1/movie/movie/list/tagid/1000300/text/{Query}/sug/on
```

### Required Header
Ensure the following header is included in your requests:

```
"jsonType": "simple"
```

### Response
This will return a list of movies matching the provided query.

---

## 🎨 Evaluation Criteria

Your submission will be assessed based on the following:

1. 🔖 **Code Readability:** Is the code well-structured, easy to understand, and maintainable?
2. ✍️ **Testing:** Are there meaningful tests included?
3. ⚛️ **Technology Usage:** Did you use modern and relevant tools/libraries?
4. 🏛️ **Architecture:** Is the architecture sound and scalable?
5. 🔖 **Git Commits:** Are your commits clear and descriptive?
6. 🔬 **Documentation:** Is the README comprehensive and helpful?
7. 🎡 **App Quality:** How good is your app? Does it meet the functional requirements?
8. ⚖️ **Configuration Changes:** Have you handled configuration changes effectively?
9. 📊 **Performance:** Have you kept performance in mind while developing the app?

---


### Example Query
Search for the keyword **"Joker":**
```http
GET https://www.filimo.com/api/en/v1/movie/movie/list/tagid/1000300/text/Joker/sug/on
```

---

## 🛠️ Tech Stack Recommendations

You’re free to choose your tools, but here are some suggestions:

- **Language:** Kotlin
- **Architecture:** MVVM or Clean Architecture
- **Network Library:** Retrofit or Ktor
- **Dependency Injection:** Dagger Hilt
- **Testing:** JUnit, MockK, or Turbine
- **UI Framework:** Jetpack Compose (Mandatory)

---

## 📊 Sample Response

Here’s a sample JSON response you can expect from the Filimo Search API:

```json
{
    "data": [
        {
            "id": "5828",
            "link_type": "movie",
            "link_key": "QNz0D",
            "movie_id": "5828",
            "movie_title": "کد سکوت",
            "movie_title_en": "Code of Silence‏",
            "descr": "کد سکوت، به معرفی ماهیت رژیم اشغالگر قدس و طرفداری دولت های غربی از آن می پردازد.",
            "cover": "https://static.cdn.asset.filimo.com/flmt/mov_cvr_5828_2207.jpg?width=2560&quality=90&sharpen=50&secret=LeNbgo1pRhV_2PsrdgPJ6w",
            "categories": [
                {
                    "title": "جنگی",
                    "title_en": "war"
                },
                {
                    "title": "کوتاه",
                    "title_en": "short"
                }
            ],
            "duration": {
                "value": 2911,
                "text": "۴۸ دقیقه"
            },
            "countries": [
                {
                    "country": "ایران",
                    "country_en": "iran"
                }
            ],
            "director": "پی اسکات هنری"
        }
    ]
}
```

---

Good luck, and we’re excited to see your solution! 🎩

