# Cekzu
Off-brand Bookmarklet that Bypasses Securly Classroom

## How it Works
To learn more checkout my blog post about it.
- It uses `data:text/html,` which loads HTML code into an `about:blank` tab
- Using this I can insert an iframe that loads a site based of user input
- And since its a `about:blank` site Securly cannot modify it

## Features
- Iframe for Bypassing Securly 
- Tab Spoofing (Title Only)

## How to Use
Make a new bookmarklet and paste this into it:
`data:text/html,<script>function cekzu() { var url = prompt('Enter URL: ', 'https://'); var iframe = document.createElement('iframe'); iframe.src = url; iframe.style.width = "100%"; iframe.style.height = "100%"; iframe.style.border = "none"; iframe.style.overflow = "hidden"; document.body.appendChild(iframe); document.body.style.width = "100%"; document.body.style.height = "100%"; document.body.style.margin = "0"; document.body.style.padding = "0"; }; function spoofie() { var title = prompt('Title: ', ''); document.title = title; }</script><button onClick="cekzu()">Cekzu</button><button onClick="spoofie()">Spoofie</button>`
