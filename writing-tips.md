# General writing guidelines for writing

Follow these writing guidelines when developing content using the templates available in this repository.

## Language and Tone

* Use consistent language and tone throughout your docs.
* Describe things as clearly and accurately as possible.
* Run your text through a grammar linter to check how readable it is.
  * Tools like Grammarly help you identify grammar issues
  * Tools like `Vale` help you identify style issues.
* Avoid colloquialisms and jargon because it makes it harder for a non-native English speaker to understand your words.
* Avoid adding your own opinions, or the opinions of others. Doing this clouds a reader's ability to draw conclusions about the discussion.

## Writing procedural steps

Here are some recommendations you can use when creating procedural steps:

* Usability studies show that procedures should not be more than seven primary steps long.
* Each step is a single sentence (you should be able to read it aloud, and it should make grammatical sense).
* When describing a step, include a lead-in sentence to remind the reader what they will be doing when following the sub-steps.
* Aim for no more than four sub-steps in any primary step.
* If you are indenting sub-steps beyond one indent level, break out your steps into a new main step block.
* Too many sub-steps could suggest that you need to break out some of these steps into a new step section.
* Screenshots and images are recommended, particularly if you can include call outs to the specific parts of the screen you are referring to.

## Page Structure

* Create a skeleton of the headings you want to include in the document before you start writing.
  * You can use this skeleton to test the information progression in your articles.
  * It's a lot easier to move things around with headings than to move blocks of content.
* You may also find that you need to create two articles if the subject starts to branch.
* Add any links you mention in the body of your discussion topic into the "See also" section. The inline links may get lost in long articles, and scanning for links add to your audience's cognitive load.

### Mirror the directory structure

If you are documenting a UI-based tool or code-base, structure the docs using the same directory structure or page tree navigation as the tool or code base.

## Titles and Filenames

* Make the title descriptive of the content contained within the article.
* Make the title unique within your application space.
* Make the title and filename the same: it makes it difficult to identify the file name when the title and filename differ.
* Use unique words in titles so you can search and replace text later on without getting fuzzy matches.

Here are some title examples and their suggested file name structures:

* Using a toaster
  * `using-a-toaster.md`
  * `using-a-toaster.adoc`
* Toast a slice of bread.
  * `toast-slice-of-bread.md`
  * `toast-slice-of-bread.adoc`

## Definitions

If you are repeatedly using terms throughout a large article, you can define them once and then use them repeatedly in the body of the article.
