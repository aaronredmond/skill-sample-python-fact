# Build An Alexa Fact Skill
[![Voice User Interface](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/1-on._TTH_.png)](./1-voice-user-interface.md)[![Lambda Function](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/2-off._TTH_.png)](./2-lambda-function.md)[![Connect VUI to Code](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/3-off._TTH_.png)](./3-connect-vui-to-code.md)[![Testing](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/navigation/4-off._TTH_.png)](./4-testing.md)

## Setting up Your Alexa Skill in the Developer Portal

There are two parts to an Alexa skill.  The first part is the [Voice User Interface (VUI)](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/defining-the-voice-interface).  This is where we define how we will handle a user's voice input, and which code should be executed when specific commands are uttered.  The second part is the actual code logic for our skill, and we will handle that on [page #2](./2-lambda-function.md) of this instructions guide.

1.  **Go to the [Amazon Developer Portal](http://developer.amazon.com).  In the top-right corner of the screen, click the "Sign In" button.** </br>(If you don't already have an account, you will be able to create a new one for free.)

    <a href="http://developer.amazon.com" target="_new"><img src="https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/general/1-1-developer-portal._TTH_.png" /></a>

2.  **Once you have signed in, click the Alexa button under the Alexa icon.**

    <a href="https://developer.amazon.com/edw/home.html#/" target="_new"><img src="https://github.com/aaronredmond/skill-sample-python-fact/blob/master/step-by-step/Alexa_button_new.png" /></a>

3.  **At the top Alexa page, choose "Skills" from the "Your Alexa Consoles" menu.**

    <a href="https://developer.amazon.com/edw/home.html#/skills/list" target="_new"><img src="https://github.com/aaronredmond/skill-sample-python-fact/blob/master/step-by-step/1-Your.Alexa-Consoles.png" /></a>

4.  **Click "Create Skill."**

    <a href="https://developer.amazon.com/edw/home.html#/skill/create/" target="_new"><img src="https://github.com/aaronredmond/skill-sample-python-fact/blob/master/step-by-step/1-Create-Skill-Button.png" /></a>

5.	**Enter a name for your skill.** You may also change the language from the default (English (US)) here. Then click the "Next" button. 

    <a href="https://developer.amazon.com/edw/home.html#/skill/create/" target="_new"><img src="https://github.com/aaronredmond/skill-sample-python-fact/blob/master/step-by-step/1-Name-Skill.png" /></a>

6.	**Choose the custom model for your skill.** Click "Create Skill". This will get you to the first page of your new Alexa skill.
	
	<a href="https://developer.amazon.com/edw/home.html#/skill/create/" target="_new"><img src="https://github.com/aaronredmond/skill-sample-python-fact/blob/master/step-by-step/1-Choose-Model.png" /></a>
		
    ### Skill Information Tips
    1.  **Skill Type** For this skill, we are creating a skill using the Custom Interaction Model.  This is the default choice.

    2.  **Language** Choose the first language you want to support.  You can add additional languages in the future, but we need to start with one.  (This guide is using U.S. English to start.)

    3.  **Name** This is the name that will be shown in the Alexa Skills Store, and the name your users will refer to.

    4.  **Invocation Name** This is the name that your users will need to say to start your skill.  We have provided some common issues developers encounter in the list below, but you should also review the entire [Invocation Name Requirements](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/choosing-the-invocation-name-for-an-alexa-skill).

        | Invocation Name Requirements | Examples of incorrect invocation names |
        | ---------------------------- | -------------------------------------- |
        | The skill invocation name must not infringe upon the intellectual property rights of an entity or person. | korean air; septa check |
        | Invocation names should be more than one word (unless it is a brand or intellectual property), and must not be a name or place | horoscope; trivia; guide; new york |
        | Two word invocation names are not allowed when one of the words is a definite article, indefinite article, or a preposition | any poet; the bookie; the fool |
        | The invocation name must not contain any of the Alexa skill launch phrases and connecting words.  Launch phrase examples include "launch," "ask," "tell," "load," and "begin."  Connecting word examples include "to," "from," "by," "if," "and," "whether." | trivia game for star wars; better with bacon |
        | The invocation name must not contain the wake words "Alexa," "Amazon," "Echo," or the words "skill" or "app." | hackster initial skill; word skills |
        | The invocation name must be written in each language you choose to support.  For example, the German version of your skill must have an invocation name written in German, while the English (US) version must have an invocation name written in English. | kitchen stories (German skill) |

        5.  **Audio Player** For this Fact skill, we won't be using any audio files, so you can select No for this option.  If you would like to learn more about adding audio to your skills, please check out our [Audio Player Guide](https://github.com/alexa/skill-sample-nodejs-audio-player).

7.  In the JSON Editor replace any existing code with the code provided in the [Interaction Model](../InteractionModel.json), then click "Save Model".  

8. Add some more sample utterances for your newly generated intents.  Think of all the different ways that a user could request to make a specific intent happen.  Here are a few examples for DescriptionIntent:

    * Give me a fact
    * Tell me a fact
    * Tell me something
    * Tell me a space fact

    ![](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/general/1-10-sample-utterances._TTH_.png)

9. Click on the **Save Model** button, and then click on the **Build Model** button.

<br/><br/>
<a href="./2-lambda-function.md"><img src="https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexa-skills-kit/tutorials/general/buttons/button_next_lambda_function._TTH_.png" /></a>
