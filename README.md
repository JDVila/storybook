# Storybook
## Our Story
### A story full of Stuff
#### Not like a Story in a building
##### More Like a story from a book
###### You know, like a storybook

<h1>Storybook</h1>
<h2>Our Story</h2>
<h3>A story full of Stuff</h3>
<h4>Not like a Story in a building</h4>
<h5>More Like a story from a book</h5>
<h6>You know, like a storybook</h6>

*This is Italisized*
_This is also Italisized_

**This is Italisized**
__This is also Italisized__

***This is both both and Italisized***
___This is both both and Italisized___

*This is italisized, but this is **bold and italisized***.

This is an unordered list:
* Apples
  * A Fruit with seeds
* Oranges
* Pears

This is an ordered list:
1. Cats
1. Dogs
1. Koalas

<ul>
  <li>One</li>
  <li>Two</li>
  <li>Three</li>
</ul>

> This is a blockquote.

\*Coughing Intensifies\*

www.google.com

[Google Website](www.google.com)

![Awesome Cat Burrito Photo: Purrito](https://i.ytimg.com/vi/Ep3jK1bZrB8/maxresdefault.jpg)

<img src="https://i.ytimg.com/vi/Ep3jK1bZrB8/maxresdefault.jpg" width="300">

This README.MD file is a file for the current repository. Is a story consisting only of hipster ipsum text.

`System.out.println("Hello World");`
'System.out.println("Hello World");'

```java
public Dialog showEmptyListDialog(final int shouldShowInterstitial) {
        AlertDialog.Builder builder = new AlertDialog.Builder(this);
        // TODO: Move strings to xml string resources
        builder.setTitle("All Facts Reviewed!");
        builder.setMessage("Review List is Empty - Do you want to refresh the deck?");
        builder.setPositiveButton("REFRESH", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int id) {
                SharedPreferences.Editor editor = flipcardPrefs.edit();
                editor.putBoolean(SHOW_EMPTY_LIST_DIALOG_KEY, false);
                editor.commit();
                if (shouldShowInterstitial == YES_INTERSTITIAL) {
                    initiateInterstitial();
                }
                populateList();
            }
        });
        builder.setNegativeButton("Leave Empty", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int id) {
                SharedPreferences.Editor editor = flipcardPrefs.edit();
                editor.putBoolean(SHOW_EMPTY_LIST_DIALOG_KEY, true);
                editor.commit();
                if (shouldShowInterstitial == YES_INTERSTITIAL) {
                    initiateInterstitial();
                } else {
                    finish();
                }
            }
        });
        // TODO: Fix issue where dialog is dismissed, but sharedprefs are not updated.
        return builder.create();
    }
```
