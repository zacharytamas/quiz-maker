# quiz-maker

A declarative interactive-quiz builder library using Polymer custom elements.

There are two methods of configuring your quiz: 1) imperatively by passing in a JavaScript object or a JSON string of it, 2) declaratively using special tags, like this:

  <quiz-maker>

    <qz-title>My quiz title.</qz-title>

    <qz-questions>
      <qn-question type="multichoice">
        <qn-prompt>Which of the following were not Beatles?</qn-prompt>
        <qn-answer>John</qn-answer>
        <qn-answer>Paul</qn-answer>
        <qn-answer correct>Charlie</qn-answer>
        <qn-answer>Ringo</qn-answer>
        <qn-answer correct>Yoko</qn-answer>
      </qn-question>

      <qn-question type="openended">
        <qn-prompt>What is your opinion of the color green?</qn-prompt>
      </qn-question>
    </qz-questions>

  </quiz-maker>

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Developing quiz-maker

If you wish to work on quiz-maker in isolation, I recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve
