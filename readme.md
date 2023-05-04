# Cekzu
Off-brand Bookmarklet that Bypasses Securly Classroom

## How it Works
To learn more checkout my blog post about it.
- It uses `data:text/html,` which loads HTML code into an `about:blank` tab
- Using this I can insert an iframe that loads a site based of user input
- And since its a `about:blank` site Securly cannot modify it

## How to Use
Make a new bookmarklet and paste this into it:
`data:text/html,<title>WAttS</title><script>function cloak() %7Blet url %3D prompt("Enter URL%3A "%2C "https://")%3Bvar iframe %3D document.createElement('iframe')%3Biframe.src %3D url%3Biframe.style.width %3D "100%25"%3Biframe.style.height %3D "100%25"%3Biframe.style.border %3D "none"%3Biframe.style.overflow %3D "hidden"%3Bdocument.body.appendChild(iframe)%3Bdocument.body.style.width %3D "100%25"%3Bdocument.body.style.height %3D "100%25"%3Bdocument.body.style.margin %3D "0"%3Bdocument.body.style.padding %3D "0"%3B%7D</script><button onclick="cloak()">WAttS</button><script>function spoofie() {let title=prompt("Title: ", ""); document.title = title;};</script><button onClick="spoofie()">Spoofie</button>`
