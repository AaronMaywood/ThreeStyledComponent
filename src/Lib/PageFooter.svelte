<footer class="hello">
  <div>
    <h1>Location</h1>
    <p>113 Brooklyn Street<br>
      Brooklyn NY 11223<br><br>
      Monday-Saturday 10-6PM<br>
      Sunday 12-5PM</p>
  </div>
  <div>
    <h1>Get in Touch</h1>
    <ul>
      <li><a href="#">Instagram</a></li>
      <li><a href="#">TikTok</a></li>
      <li><a href="#">Facebook</a></li>
    </ul>
  </div>
</footer>

<style>
footer {
	display: flex;
	gap: 4rem; /* for Flexbox - https://developer.mozilla.org/ja/docs/Web/CSS/gap gap はflex, grid の両方に指定できる */
	background: #333;
	color: white;
	padding: 2rem;
	line-height: 2;
}

h1 {
    font-size: 14px;
    font-weight: 800;
    text-transform: uppercase;
    letter-spacing: 0.25px;
    margin: 0.5rem 1rem 0;
}

footer h1 {
	font-size: 3rem;
	font-weight: 200;
}

footer a {
	color: white;
}
</style>
