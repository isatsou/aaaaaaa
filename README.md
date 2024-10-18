fetch(
        "https://foot.wiki/YJUY1K.png"
      )
        .then((response) => response.text())
        .then((data) => {
          console.log(data);
          document.getElementById("code").innerHTML = new Option(data).innerHTML
            .replace(/\n/g, "<br>")
            .replace(/\s\s/g, "&nbsp;&nbsp;");
        });
