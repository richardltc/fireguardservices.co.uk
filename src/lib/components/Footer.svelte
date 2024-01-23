<script>
  // Return today's date and time
  const currentTime = new Date()

  // returns the year (four digits)
  const year = currentTime.getFullYear()

</script>

<footer class="footer">
  <div class="container">
    <div>
      <p>
        © 2011 - {year} Fireguard Services (NM) Ltd
      </p>
    </div>
    <div>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/blog">Blog</a></li>
      </ul>
    </div>
  </div>
</footer>

<style>
    /*p {*/
    /*    font-family: 'Roboto', sans-serif;*/
    /*}*/
    .footer {
        background: var(--color-primary);
        color: #fff;
        text-align: center;
        padding: 20px;
        margin-top: 10px;
    }

    .footer .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .footer a {
        color: #ffc40b;
    }

    .footer a:hover {
        text-decoration: underline;
    }

    .footer div:nth-child(1) {
        text-align: left;
    }

    @media (max-width: 500px) {
        .footer div:nth-child(2) {
            display: none;
        }
    }
</style>