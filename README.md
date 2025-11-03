<!-- Banner / Header image -->
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=36BCF7&center=true&vCenter=true&width=500&lines=Mid-level+Flutter+Developer;GetX+%E2%80%A2+Laravel+%E2%80%A2+50k%2B+RPM;Code+is+poetry%2C+bugs+are+features" alt="Typing SVG" />
</p>

---

<p align="center">
  <a href="https://github.com/suleohis"><img src="https://komarev.com/ghpvc/?username=suleohis&label=Profile+Views&color=0e75b6&style=flat" alt="Views" /></a>
  <a href="https://github.com/suleohis?tab=followers"><img src="https://img.shields.io/github/followers/suleohis?label=Followers&style=flat&color=36BCF7" alt="Followers" /></a>
</p>

---

# 👋 Hi, I'm Ephraim — Mid-level Flutter Developer (4+ yrs)

**99% crash-free apps** • **20%↑ engagement** • **Full-stack: Flutter + Laravel (50k+ RPM)**  
Open to **100% remote / EU relocation (visa support)**

---

## 🧑‍💻 About Me

- 🧠 I code, therefore I am. (And sometimes, therefore, I debug.)
- 🥇 Master of none, but pretty decent at many.
- 🌐 I speak fluent English, sarcasm, and at least 7 programming languages. Sometimes all at once.

---

## 🛠️ Tech Stack

| Skill | Level | Proof |
|------|-------|-------|
| **Flutter** | Expert | [Chef Kiss](https://github.com/suleohis/chef_kiss) |
| **Dart** | Expert | |
| **GetX** | Expert | [GetX Snippet](#getx-state-management) |
| **Firebase** | Strong | Auth, Firestore, Chat |
| **RESTful API** | Strong | Laravel consumer |
| **Dio** | Strong | HTTP client |
| **OAuth** | Strong | Secure auth |
| **Laravel** | Strong | 20+ endpoints |
| **PHP** | Strong | Backend logic |
| **GitHub Actions** | Basic | CI/CD pipelines |
| **Git** | Strong | Team workflows |
| **Agile** | Strong | Sprint planning |

---

## 🚀 Featured Projects

- **Chef Kiss:** A Flutter mobile recipe app showcasing advanced UI/UX and state management, providing a Michelin-star culinary experience. [Check out the repo here!](https://github.com/suleohis/chef_kiss)
- **Voice Notepad:** A Flutter speech-to-text note-taking app demonstrating efficient audio processing and local storage solutions. [Check out the repo here!](https://github.com/suleohis/voice-notepad)

---
## 💻 Code Snippets (Click to Expand)

### GetX State Management
```dart
class RecipeDetailController extends GetxController {
  MealRepo mealRepo = MealRepo();
  FirebaseRepo firebaseRepo = FirebaseRepo();
  final String mealId;
  RecipeDetailController({required this.mealId});
  RxInt tabIndex = 0.obs;
  Meal? meal;
  YoutubePlayerController? youtubeController;
  RxBool isLoading = false.obs;
  UserModel? user;
  RxBool isBookmark = false.obs;


  @override
  void onInit() {
    super.onInit();
    getRecipeData();
  }

// UI
RefreshIndicator(
  onRefresh: () => controller.onRefresh(),
  child: Obx(
  () =>
    controller.isLoading.value || controller.meal == null
        ? RecipeDetailShimmer()
        : RecipeDetailBody(controller: controller),
    ),
  ),

//Laravel API Call (Flutter → Backend)
  Response response = await _dio.get(endpoint, queryParameters: params);
  return ResponseModel(
    isSuccess: true,
    message: response.data.toString(),
    statusCode: response.statusCode ?? 200,
    responseJson: response.data,
  );
```

```php
// routes/api.php
Route::middleware('auth:api')->get('/recipes', [RecipeController::class, 'index']);
```



## 🐞 What I'm Currently Debugging

- 🌱 I’m currently learning: advanced Flutter animations, server-side Dart, and new testing frameworks.
- 👯 I’m looking to collaborate on: open-source Flutter projects and innovative mobile fintech solutions.
- 💬 Ask me about: Flutter performance optimization, cross-platform UI/UX, or anything else that keeps you up at night as a developer!

---

## 📊 My GitHub Stats

<p align="center">
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img src="https://github-readme-stats.vercel.app/api?username=suleohis&show_icons=true&theme=tokyonight&title_color=00e19d&icon_color=00e19d&text_color=ffffff&bg_color=22272e" alt="GitHub Stats" />
  </a>
  <a href="https://github.com/denvercoder1/github-readme-streak-stats">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=suleohis&theme=tokyonight&background=22272e&ring=00e19d&fire=ffba08&currStreakLabel=00e19d" alt="GitHub Streak" />
  </a>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=suleohis&bg_color=22272e&color=00e19d&line=ffba08&point=ffffff&area=true&hide_border=true" alt="GitHub Activity Graph"/>
</p>

---

> "Code is like humor. When you have to explain it, it’s bad." — Cory House

<p align="center">
  Feel free to browse my repositories, leave a star, or just send good vibes (or memes).  
</p>

<!--
## 📌 Pinned Projects

On my profile page, you'll find my best work pinned for quick access:  
- Chef Kiss  
- Voice Notepad  
- ...and more!
-->

