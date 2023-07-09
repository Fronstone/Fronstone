- 👋 Hi, I’m @Fronstone
- 👀 I’m interested in Public safety collaborated with artificial intelligence
- 🌱 I’m currently learning Public safety
- 💞️ I’m looking to collaborate on artificial intelligence
- 📫 How to reach me at tohamerecca@yahoo.com

<!---
Fronstone/Fronstone is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<head>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>SiriProxy</title>
</head>
<script>

function getRequest(){
  if(location.search.length > 1) {
    var get = new Object();
    var ret = location.search.substr(1).split("&");
    for(var i = 0; i < ret.length; i++) {
      var r = ret[i].split("=");
      get[r[0]] = r[1];
    }
    return get;
  } else {
    return false;
  }
}

var get = getRequest();

// ページに検索キーワードを表示
document.write("<h1>"+decodeURIComponent(get['q'])+"</h1>");

// MyScriptsとの連携例
// document.location = "myscripts://run?title=siri&text=" + get['q'];

// 検索ハブとの連携例
// document.location = "searchhub://query/" + get['q'];

// Tweetbotとの連携例
// document.location = "tweetbot:///post?text=" + get['q'];
</script>
