---
title: "Yéil Learning"
layout: default
---

# [Support Me on Patreon!](https://www.patreon.com/yeillearning)

If you haven't yet, go ahead and read the [About](#about) blurb at the bottom of the page to understand my mission. Quickly put, I'm writing books to teach and make topics in science and engineering more accessible to those who want to learn. If you want to support my endeavour, consider subscribing to my [Patreon!](https://www.patreon.com/yeillearning)

{% assign books = site.data.books.books %}

# Books

Here are my books! (Works in progress have the <span id="span-draft">Drafting</span> border)

<div class="books">
    <div class="container">
        <div class="row align-items-center">

            {% for book in books %}
                
                <div class="col-lg-6">
                    {% if book.draft %}
                        <fieldset id="fieldset-draft"><legend id="legend-draft">Drafting</legend>
                    {% else %}
                        <fieldset id="fieldset-published"><legend id="legend-published">Published</legend>
                    {% endif %}
                            <div class="book">
                                <img src="{{ book.image }}" class="book-cover">

                                <h2>{{ book.title }}</h2>

                                {{ book.abstract }}
                            </div>
                        </fieldset>
                </div>

            {% endfor %}

        </div>
    </div>
</div>

# <a name="about"></a>About

Hi all! I'm Doug! I'm a PhD student (soon to defend my thesis) in oceanography and I like to learn and teach. As a way to scratch the itch to teach, I've started writing books to help others learn seemingly very challenging and advanced topics in the fields of science and engineering, like Calculus, Partial Differentiation, and/or Vibrations (maybe even a touch of Thermodynamics or Fluid Mechanics sometime). And while the different books that I'm writing will be intended for different starting levels of knowledge, the point of these books are to help those who want to learn and to learn these complex topics _by themselves_.

A lot of the introductory textbooks for topics in science and engineering are typically made to go along with a course at a university, not as the sole resource for an autodidact. Sure, to the already enlightened they may seem full enough to understand the topic without an instructor, but, a lot of the time, they skip steps with the expectation that an instructor will fill in the gaps. That's not what I'm doing here. Here, in these books, I am giving you all the information needed to lead you through the work as though _the text itself was the instructor_. And by doing so, opening up the world of science and engineering to those who don't necessarily want to go to university to learn a topic or to those who want a better resource to teach themselves, by themselves.

Enjoy!

Oh and if you're wondering what the logo and name is all about, yéil is the Tlingit word for raven. Ravens are known for their intelligence, and unlike in more western culture where they are typically associated with death, in the cultures of the Indigenous peoples of Pacific Northwest, the raven is associated with creation (and sometimes a little trickery). And, well, here we're trying to create and promote knowledge, so it only seems fitting.

# Contact

{% assign contacts = site.data.contacts.contacts %}

<div class="contacts">
    <div class="container">
        <div class="row justify-content-evenly">

            {% for contact in contacts %}
                
                <div class="col-lg-1 align-self-center">

                    <a href="{{ contact.link }}"><img src="{{ contact.image }}" class="contact-image"></a>

                </div>

            {% endfor %}

        </div>
    </div>
</div>
