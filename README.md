### Hi, I am Namrata! 👋

![image](https://github.com/namrata3098/namrata3098/assets/60501115/9cb4dc3d-beda-4841-8289-758d0acb10b3)

### A passionate full-stack developer with an eye for design. I'm passionate about this work because I enjoy building and creating visually pleasing projects and having the ability to see the result of my work 😄.

 - 🌱 I’m currently learning **TypeScript** and **Python**
 
 - 📫 How to reach me: namnp917@gmail.com
 
 - 💬 Ask me about **React** and **Node**
 
 - Website About me: https://master--funny-meerkat-e36bc0.netlify.app/#AboutMe

fetch('https://api.github.com/users/<your_username>/repos')
  .then(response => response.json())
  .then(data => {
    const languages = {};
    data.forEach(repo => {
      const { language } = repo;
      if (language) {
        if (languages[language]) {
          languages[language]++;
        } else {
          languages[language] = 1;
        }
      }
    });
    const sortedLanguages = Object.entries(languages)
      .sort((a, b) => b[1] - a[1])
      .map(([language, count]) => `${language}: ${count}`);
    console.log(sortedLanguages);
  })
  .catch(error => console.error('Error:', error));

  
