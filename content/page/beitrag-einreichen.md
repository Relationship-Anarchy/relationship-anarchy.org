---
title: Beitrag einreichen
description: Einfach einen neuen Beitrag veröffentlichen
menu: hidden
comments: false
---

<form method="POST" action="http://formspree.io/beitrag@relationship-anarchy.org">
  <input type="hidden" name="_language" value="de" />
  <input type="hidden" name="_subject" value="Neuer Blog Beitrag" />
  <input type="hidden" name="_next" value="//relationship-anarchy.org/beitrag-eingereicht" />
  <input type="text" name="autor" placeholder="Autor Name / Pseudonym">
  <input type="email" name="email" placeholder="E-Mail Adresse">
  <textarea rows="10" name="message" placeholder="Dein Blog Beitrag"></textarea>
  <button type="submit">Beitrag einreichen</button>
</form>
