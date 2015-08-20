# h1-debate

## The possibilities

### Semantic

With html5 and all the sectioning elements it's possible to have a good semantic document like the following.

    <title>Page title | Site title</title>
    <header>
      <a href="/"><h1>Site title</h1></a>
    </header>
    <main>
      <article>
        <h1>Page title</h1>
      </article>
    </main>

### SEO

Most SEO expert will prefer to have the page title in the h1, leaving the site title out of any hn.

    <title>Page title | Site title</title>
    <header>
      <a href="/">Site title</a>
    </header>
    <main>
      <article>
        <h1>Page title</h1>
      </article>
    </main>

### SEO + h1 for site name on frontpage

Sometimes we see this alternative of the SEO solution above. All internal pages are like the one described above except the frontpage which will have the site title in h1.

    <title>Page title | Site title</title>
    <header>
      <a href="/"><h1>Site title</h1></a>
    </header>
    <main>
      <article>
        <h2>Frontpage title</h2>
      </article>
    </main>
    
## Testing

How to test if any of these method has a particular effect on SEO ranking? Feel free to submit a pull request if you have a good idea about this but here is how this could be done.

1. Have a micro website with one of those solution.
2. Wait a little to have the website indexed.
3. Change the method and go to step 2.

This solution will avoid possible duplicate content penalty which may happen if we would test all methods at the same time on different domain.

## Measuring the effect

- google webmaster tools
