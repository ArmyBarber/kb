```javascript
var storedTheme = localStorage.getItem('theme') || (window.matchMedia("(prefers-color-scheme: dark)").matches ? "dark" : "light");

setTimeout(function() {
    var targetTheme = storedTheme == "dark" ? "light" : "dark";
    switchTweetTheme(targetTheme, storedTheme);
}, 1000);

function switchTweetTheme(currentTheme, targetTheme) {
    var tweets = document.querySelectorAll('[data-tweet-id]');

    tweets.forEach(function(tweet) {
        var src = tweet.getAttribute("src");
        tweet.setAttribute("src", src.replace("theme=" + currentTheme, "theme=" + targetTheme));
    });
}
```

