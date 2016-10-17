## Represent content in a modal in GitBook

Modified from [chudaol's GitBook YouTube plugin](https://github.com/chudaol/gitbook-plugin-modal-youtube-video).

This plugins requires gitbook `>=2.0.0`.

### Usage

Add plugin to your `book.json`, then run `gitbook install`:

```
{
    plugins: ["modals"]
}
```

Add the web source for the modal - another webpage, a YouTube video, etc. - within the template tags:

```
{% modalItems %}http://www.github.com Look, here's GitHub{% endmodalYoutube %}
```

### Add custom html code to the modal header

Custom html can be inserted within the template tag to appear in the modal's header. For example, if you would like a link to appear in the modal header, then you can use the pipe character to separate the URL link from the item label and from your custom html header code:

```
{% modalItems %}http://www.youtube.com/v/9bZkp7q19f0|Look at this video!|<a href="#">This is my custom header link!</a>{% endmodalItems %}
```

The text will appear left-justified in the modal header, complete with a link.
