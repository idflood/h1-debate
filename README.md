# h1 Debate

There is many ways to structure an html page. Some may prefer good semantic and other pure SEO. This is an attempts to define if really one of these method has significant impact on SEO ranking.

## Table of contents

* [The possibilities](#the-possibilities)
* [Testing](#testing)
* [Measuring the effect](#measuring-the-effect)

## The possibilities

### Semantic

With html5 and all the sectioning elements it's possible to have a good semantic document like the following.

    <header>
      <a href="/"><h1>Site title</h1></a>
    </header>
    <main>
      <article>
        <h1>Page title</h1>
      </article>
    </main>

#### pros
- Good css outline [1](http://html5doctor.com/outlines/)
- Consistent
- ...

#### cons
- Page title not indexed as much as it can
- Possibly less accessible since there is no know support of outline [1](http://www.w3.org/html/wg/drafts/html/master/semantics.html#outlines) [2](http://www.paciellogroup.com/blog/2013/10/html5-document-outline/)
- ...

### SEO

Most SEO expert will prefer to have the page title in the h1, leaving the site title out of any hn.

    <header>
      <a href="/">Site title</a>
    </header>
    <main>
      <article>
        <h1>Page title</h1>
      </article>
    </main>
    
#### pros
- Page title should have a better search ranking
- Consistent across the whole website
- ...

#### cons
- Don't follow html5 best practice [1](http://html5doctor.com/outlines/)
- ...

### SEO + h1 for site name on frontpage

Sometimes we see this alternative of the SEO solution above. All internal pages are like the one described above except the frontpage which will have the site title in h1.

    <header>
      <a href="/"><h1>Site title</h1></a>
    </header>
    <main>
      <article>
        <h2>Frontpage title</h2>
      </article>
    </main>

#### pros
- Good semantic on frontpage
- Pages title should have a high search ranking
- ...

#### cons
- Not consistent across website
- Don't follow html5 best practice except on frontpage [1](http://html5doctor.com/outlines/)
- ...

## Testing

How to test if any of these method has a particular effect on SEO ranking? Feel free to submit a pull request if you have a good idea about this but here is how this could be done.

1. Have a micro website with one of those solution.
2. Wait a little to have the website indexed.
3. Change the method and go to step 2.

This solution will avoid possible duplicate content penalty which may happen if we would test all methods at the same time on different domain.

## Measuring the effect

- google webmaster tools
