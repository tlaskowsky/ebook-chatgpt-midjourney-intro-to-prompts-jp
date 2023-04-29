### 「ChatGPT＋Midjourneyでデジタルアートを極める！英語プロンプト術入門」のリソース集

1. [第１章リソース](/chapter 1/readme.md)
1. [第２章リソース](/chapter 2/readme.md)
1. [第３章リソース](/chapter 3/readme.md)
1. [第４章リソース](/chapter 4/readme.md)
1. [第５章リソース](/chapter 5/readme.md)
1. [第６章リソース](/chapter 6/readme.md)


<ul id="chapter-files"></ul>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>

<script>
  $(document).ready(function() {
    var user = 'tlaskowsky';
    var repo = 'ebook-chatgpt-midjourney-intro-to-prompts-jp';
    var branch = 'gh-pages'; // or 'main' or 'master', depending on your default branch
    var subdirectory = 'chapter%201'; // Replace spaces with %20 for URL encoding

    $.getJSON('https://api.github.com/repos/' + user + '/' + repo + '/contents/_chapters/' + subdirectory + '?ref=' + branch, function(data) {
      $.each(data, function(index, file) {
        if (!file.name.startsWith('.')) {
          $('#chapter-files').append('<li><a href="' + file.download_url + '">' + file.name + '</a></li>');
        }
      });
    });
  });
</script>