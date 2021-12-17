---
layout: handbook-page-toc
title: "Qualtrics Tips & Tricks"
description: "How to use Qualtrics at GitLab to run surveys"
---

## Creating a survey

1. Select `Blank survey project`
1. Give your project a name.
1. Enter survey questions. On the right hand side of the screen you will find:
    * [Question types](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/question-types-overview/) and formatting (number of answer choices, positioning and so on).
    * [Validation](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/validation/) (force respondents to answer a question or request that they consider answering the question before leaving the page).
    * Actions (such as [page breaks](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/add-page-break/), [skip logic](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/skip-logic/) and [display logic](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/display-logic/)).
1. Update the `Look & Feel` of your survey.
    * Please refer to [Look & Feel settings](#styling-look--feel-settings) for guidance.
1. Adjust your [Survey Options](https://www.qualtrics.com/support/survey-platform/survey-module/survey-options/survey-options-overview/) as appropriate.
1. Under the [Tools](https://www.qualtrics.com/support/survey-platform/survey-module/survey-tools/survey-tools-overview/) menu, you will find a host of useful features such as:
    * `Collaborate` - Allows you to share your survey with another Qualtrics user so you can edit it and/or analyze the results together.
    * `Spell check` - Supports English (US) only.
    * `Generate test responses` - Generate automated dummy responses for your survey to see what the dataset and report will look like before sending the survey to actual participants.
    * `Check survey accessibility` - Determine whether your survey is accessible for respondents who use screen readers, and receive suggestions for improving your survey’s accessibility.
    * `Analyze Survey` - Open [ExpertReview's](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/quality-iq-functionality/) suggestions for your survey.
    * `Import/export survey` - From/to a QSF, TXT or DOC file.
1. When you have finished building your survey, `Preview` it to ensure that everything is working the way you expect it to.
1. Once you are ready to launch your survey, click `Publish`.

## Styling (Look & Feel settings)

The following settings should be applied to your survey:
1. Theme: Blank
1. Layout: Modern
1. General
    * Progress bar: Without Text
    * Progress bar position: Top
1. Style
    * Primary colour: #554488
    * Secondary colour: #554488
    * Font: Arial   
    * Foreground contrast: Medium
    * Question spacing: Compact
    * Question text: 14px bold
    * Answer text: 14px
1. Motion
    * Page transition: None
    * Additional check boxes: Unticked
1. Logo
    * GitLab First Look Logo (stored in UX Research library)
    * Style: Banner
    * Placement: Left
    * Max height: 70px
    * Mobile scaling: 66%
1. Background
    * Background type: Color
    * Background color: #ffffff
    * Foreground contrast: Medium
    * Questions container: Off

## Avoiding spam responses from social media

Distributing a survey on social media is a great way to quickly expand your audience, reducing the time and cost of research. However, be aware that **surveys shared on social media are often targetted by bots or fake participants** to submit dozens or hundreds of responses in a short amount of time, affecting the integrity of the data and the whole research. **This especially affects surveys with rewards or surveys shared on Twitter.**

Some bots are more sophisticated then others. For example, basic bots will “speed” through the survey or provide illogical responses to open-ended questions; more sophisticated bots will intentionally take more time to complete the survey or even use language from the survey itself to compose logical responses to open-ended questions. That's right, some people go to great lengths to get the survey rewards.

Fear not, there are multiple things you can do to prevent or filter out _most of these responses_. We say “most of these responses” because the only true way to avoid spam in your surveys is to not share them on social media but rather to [send email survey invitations with individual links](https://www.qualtrics.com/support/survey-platform/distributions-module/email-distribution/emails-overview/#UnderstandingTheIndividualLink) that can only be used once, leveraging our First Look panel.

### Prevent spam responses before sharing the survey

Before sharing your survey, use the following approaches to prevent bots and fake participants. Note that while Qualtrics [captcha question](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/advanced/captcha-verification/) and [fraud detection features](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/fraud-detection/) help, they are insufficient in preventing more sophisticated bots.

- Add a [captcha question](https://www.qualtrics.com/support/survey-platform/survey-module/editing-questions/question-types-guide/advanced/captcha-verification/) at the beginning of the survey.
- Enable all [fraud detection features](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/fraud-detection/): Prevent multiple submissions, Bot detection, Security scan monitor, and RelevantID.
- Add a “honeypot” question, a question hidden from humans but “visible” to bots. Some bots will answer this question, allowing you to screen them out or filter out their responses.
   1. Add an **optional** single-choice question (checkbox) somewhere in your survey. The question and location is not relevant as it will be hidden from humans. For example, “Are you human?” `[ ] Yes`.
   1. [Add the following JavaScript](https://www.qualtrics.com/support/survey-platform/survey-module/question-options/add-javascript/) to that question, by replacing the existing `Qualtrics.SurveyEngine.addOnload` function:
      ```js
      Qualtrics.SurveyEngine.addOnload(function()
      {
          jQuery("#"+this.questionId).hide();
      });
      ```
   1. Preview the survey to check that the question is hidden when the page loads.
- Add a **required** choice question that checks respondent's attention and logic. For example, directly state which answer they should choose or ask which year it is.
- Add illogical options to multiple-choice questions. For example, in the question “Which of these tools do you use for code review?” add an illogical option like `[ ] Tanuki Code`.
- Ask the same **required** question at two separate points of the survey. Try to use a simple multiple-choice question that people can easily answer. For example, their job title or their team size.
- For all three question types above, if you want to screen out respondents based on their answers, see the **Branching Respondents Out of the Survey** section under the [Screening Out Respondents in the Survey Flow](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/advanced-elements/screen-out-management/#ScreeningOutRespondentsInTheSurveyFlow) section. After adding the survey flow logic described in that section, you can then decide to just [flag those responses](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/advanced-elements/screen-out-management/#FlaggingScreenedOutResponses) for later analysis or [immediately discard them](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/advanced-elements/screen-out-management/#DiscardingScreenedOutResponses).

In addition, if your survey is shared on multiple social media channels, you can track from what source a participant is accessing the survey by [passing information through query strings](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/standard-elements/passing-information-through-query-strings/#PassingInformationIntoASurvey). This can help filter out responses if one source seems to have more spam than others.

### Filter out spam responses after closing the survey

After closing your survey, its now time to see how much the prevention measures have mitigated spam responses and which responses we still need to filter out. The [Response Quality](https://www.qualtrics.com/support/survey-platform/data-and-analysis-module/data/response-quality-functionality/) feature automatically flags responses for you based on a [number of criteria](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/response-quality/).

- View the [Response Quality](https://www.qualtrics.com/support/survey-platform/data-and-analysis-module/data/response-quality-functionality/#ViewingResponseQuality) report and [filter out responses](https://www.qualtrics.com/support/survey-platform/data-and-analysis-module/data/response-quality-functionality/#FilteringResponsesbyIssue).
- Check for illogical responses to open-ended questions, if applicable.
- Check for respondents who complete your survey too quickly. The Response Quality feature attempts to [flag “speeder” responses](https://www.qualtrics.com/support/survey-platform/survey-module/survey-checker/response-quality/#Speeders) but it only works for surveys with at least 100 responses.
- Check for duplicate email addresses, if applicable. Also pay attention to `@aol.com`, `@yahoo.com`, and `@hotmail.com` email addresses that are frequently used to spam surveys.

## Distributing a survey to GitLab First Look 

**Note: These instructions are only applicable to UX Researchers and Research Coordinators.**
1. Select `Contacts` (top right menu).
1. Select `Lists` (far left menu).
1. Select `GitLab First Look`
1. Select `List Options`
1. From the dropdown menu, select `Create Sample From List`. 
1. Give your sample a name.
1. Select your sample size (the number of people who you ideally want to distribute your survey to).
    * It is advisable to send your survey to a small test sample of users to begin with, to ensure that you receive the kind of responses you are looking for. 
    * When you distribute your survey to a larger audience, to avoid contacting the same users who have already answered your survey as part of your test sample, click `Advanced Sampling Criteria`, ensure the sampling criteria statement reads: `All of the following are true`, change the `Contact Activity` filter to `Survey` and change the `Select survey` filter to the survey you have already distributed.
1. Click `Add Sampling Criteria`
1. Ensure the sampling criteria statement reads: `All of the following are true`
1. Select `Embedded data`, select an `Embedded Data field`, select an `Operator` and enter/select an `Embedded Data Value`.
    * For every sample you create, you must always add sampling criteria for `Stage groups` and `Types of research`. When a person signs up to GitLab First Look, they specify what they would like to receive studies about (stage groups) and what type of research they would like to take part in. It’s extremely important that when you contact users, you only email them in relation to their preferences.
    * Remember the embedded data for `Stage groups` and `Types of research` can contain multiple values (it’s rare that users sign-up to receive emails abouts one particular stage group or want to take part in one form of research). Therefore, your `Operator` will always be `Contains`.
    * For more information on what embedded data is available, please refer to the [embedded data](/handbook/engineering/ux/qualtrics/#embedded-data) section.
1. Click `New Condition` to add additional sampling criteria.
1. Click `Create` once you have finished entering your sampling criteria. 
1. A progress bar will appear, this indicates that Qualtrics is building your sample.
1. Once the sample is ready, click `Go to Sample` (Alternatively you can navigate to `Lists` and your new sample will be visible under `All Lists`. Click on your sample to access it).
1. The number of contacts in your sample will show on the left hand side of the screen. 
    * [What to do if your sample size is lower than expected](/handbook/engineering/ux/qualtrics/#what-to-do-if-your-sample-size-is-lower-than-expected)
1. If you are happy with the number of contacts in your sample, you are now ready to send your survey to users. To do this, go to `Projects`
1. Select the project/survey you want to distribute to users.
1. Click `Distributions`
1. Click `Compose Email`
1. In the `To` field, navigate to: `Group Library: UX Research` -> `GitLab First Look` -> `Samples` and select the sample you created earlier.
1. Update the `From` field to: `firstlook@gitlab.com`
1. Update the `From Name` to: `GitLab First Look`
1. The `Reply-To Email` can either be your own, personal GitLab email address or `firstlook@gitlab.com`
    * If you are planning to leave a survey running while you are on vacation, please use `firstlook@gitlab.com` as this will automatically forward to all UX Researchers who may be able to assist with any user queries in your absence.
1. Update the `When` field to the time you would like to send the email.
1. Enter your `subject line`. 
    * A standard subject line we use for campaigns is: `Quick, new research study available!` however, if you wish, you may experiment with this. Please ensure that you use a [subject line checker](https://www.subjectline.com/) to evaluate your subject line.
1. Delete the standard text/links which appear in the WYSIWYG text area.
1. Click `Load Message` next to the Message field.
1. Navigate to `Group Library: UX Research` and select the template you would like to use.
1. Select `Use Fixed Text` option from the `Load Message` dropdown after the template has loaded. This stops any changes you make to the template from being saved permanently.
1. Edit the message text as appropriate.
    * By default, the call to action always links to the current project/survey you are planning to send. As does the screening survey text link found in the body of templates for `Usability testing` and `User interviews`.
1. When you have finished building your email, click `Send Preview Email` and enter your GitLab email address. A copy of the email will be sent to you for review.
1. If you are happy with your email, click `Send`

### Embedded data

**Note: These instructions are only applicable to UX Researchers and Research Coordinators.**

When users sign-up to GitLab First Look, we automatically collect the following embedded data:
1. `Stage groups`
    * `1` - Manage
    * `2` - Plan
    * `3` - Create
    * `4` - Verify
    * `5` - Package
    * `6` - Release
    * `7` - Configure
    * `8` - Monitor
    * `9` - Secure
    * `10` - Protect
    * `11` - Enablement & Growth
1. `Types of research` *(Removed in Nov. 2020. Data for this question will exist for users that signed up previously but not for new panel members.)*
    * `Beta testing`
    * `Cards sorts`
    * `Design evaluations`
    * `Surveys`
    * `Usability testing`
    * `User interviews`
1. `GitLab user` - Whether or not the person is a GitLab user.
    * `Yes` - the person is a GitLab user.
    * `No` - the person is not a GitLab user.
1. `Job title` - What the person's job title is.
    * `Back-end Engineer/Developer`
    * `Designer`
    * `DevOps Engineer`
    * `Executive (VP of Engineering, CTO, CEO, etc)`
    * `Front-end Engineer/Developer`
    * `Full-stack Engineer/Developer`
    * `Infrastructure Engineer`
    * `Operations Engineer`
    * `Penetration Tester`
    * `Product Manager`
    * `Project Manager`
    * `Quality Assurance Engineer`
    * `Researcher`
    * `Security Analyst`
    * `Security Professional`
    * `Scientist`
    * `Site Reliability Engineer`
    * `Software Engineer/Developer`
    * `Student`
    * `Systems Administrator/Engineer`
    * `Unemployed`
    * `Other`
1. `Organisation size` - How many people work within the user's organisation? (Added August 2019)
    * `0-10 people`
    * `11-100 people`
    * `101-500 people`
    * `501-1000 people`
    * `1001-10,000 people`
    * `10,000+ people`
1. `Team size` - How many people work within the user's team (Added August 2019)
    * `0 - it's just me!`
    * `1-5 people`
    * `6-10 people`
    * `11-20 people`
    * `21-30 people`
    * `30+ people`
1. `SaaS (GitLab.com) package`
    * `Free`
    * `Bronze`
    * `Silver`
    * `Gold`
    * `I don't know`
1. `Self managed package`
    * `Core`
    * `Starter`
    * `Premium`
    * `Ultimate`
    * `I don't know`

* Something missing from this list? Let Sarah know and she will get it added!

* When using an `Embedded Data Value` Qualtrics doesn't automatically auto-complete the value as you begin typing it. The search functionality can also be haphazard. Therefore, ensure you type out the value in full, as it is displayed above.

* Embedded data fields used to be case-sensitive. For the vast majority of Qualtrics' users, embedded data is no longer case-sensitive, meaning “test” and “Test” would be treated as the same field. However, Qualtrics still advise matching cases as a best practice, as there are a small portion of accounts where this change has not been made.

* Not all Embedded Data Values were created at the point of GitLab's First Look creation. Therefore, we don't necessarily have completed values for every user. It's also worth noting that some values for users may change over time. For example, someone may change jobs which may impact their job title, organisation and team size. Therefore, there may be some discrepancies in the information we hold about users. We plan to reduce this risk by periodically asking members of GitLab First Look to check and, where necessary, update the information we have on file for them.


### What to do if your sample size is lower than expected

**Note: These instructions are only applicable to UX Researchers and Research Coordinators.**

There could be a couple of reasons why your sample number is lower than expected:
1. The contact frequency for GitLab First Look has been exhausted. By default, no member of GitLab First Look receives an email more than once a week or four times a month. If this is the case, you will need to either delay sending your survey (you may only need to delay sending your survey by a day - reach out to the UX Research Coordinator for confirmation) or source users outside of the GitLab First Look panel.
1. There aren’t enough GitLab First Look members that match your sampling criteria.
1. There’s an error in your sampling criteria.

* For options 2 and 3, navigate to your sample and click `List options`, select `Edit sample` to change your sampling criteria.

## Distributing your survey to GitLab.com users

**Note: These instructions are only applicable to UX Researchers and Research Coordinators.**

There will be studies where you wish to target specific populations of users based on some criteria (for instance, users that have authored at least 5 merge requests in the last 30 days). If it's possible to generate a list of user IDs for a given criteria (typically from the [data warehouse](/handbook/business-ops/data-team/#-data-warehouse)), you can use that list to push those users contact info into Qualtrics and distribute a survey. **Note that this is limited to users of GitLab.com and does not include Self-Managed users.**

1. Generate your list of GitLab.com user IDs and put them into the first column of a Google Sheet. The first entry in the first column (A1) should be `id`, as this confirms that this is a list of ids that you want to use.
1. The name of the specific sheet (or tab) should be what you want to name the Qualtrics mailing list, for example, `05/20 - CI Pipeline Prototype Testing`. **This name cannot contain the following characters: `. < >`. Doing so will case an error in the transfer to Qualtrics.**
1. The filename of the entire spreadsheet should be `qualtrics_mailing_list.` followed by the name of the worksheet/mailing list that you used in the step above. So keeping with our previous example, `qualtrics_mailing_list.05/20 - CI Pipeline Prototype Testing`
1. Once everything is ready, move the file into the `QualtricsRequest` Google Drive folder.
1. If everything was done correctly, within about 15 minutes, the `id` entry in A1 should turn into `processing`. That means the data pipeline is working on your request.
1. A1 will show `processed`.  Your mailing list should now be in Qualtrics at this point.
1. Add `processed_` to the filename in order to make it clear which files have been completed, as well as to keep the process executing as quickly as possible in the future.
1. The list will show up as a shared list for the *UX Research & Product* directory. You can access the list itself from the *Contacts* section of Qualtrics, or you can select the list as part of the process of sending an email distribution.
 
* The GitLab.com user ID you specified in your Google Sheet will be included in the Qualtrics mailing list as embedded data. You can use this to associate any responses you get with your original user list.

## How to create a tracked link

You may want to promote a survey using several methods, and keep track of which one performs the best (for example: GitLab social, ux team social, in a blog post, or in a banner within gitlab.com). You can do this by using query strings. Read the [documentation](https://www.qualtrics.com/support/survey-platform/survey-module/survey-flow/standard-elements/passing-information-through-query-strings/), or watch a [short video](https://share.getcloudapp.com/kpumEOvR). 

## How to delete a contact from our directory

UX Research Coordinators occasionally receive requests to remove a contact from all lists. It's important to note that each list is independent, so removing a contact from one list does not automatically remove them from others they may have subscribed to. 

UX Research Coordinators, or other team members with Qualtrics Brand Administrator access, must remove contacts on a global level to prevent them from receiving future emails.  

To remove a contact from your directory:
1. Log into your Qualtrics account
1. Click on the Contacts tab on the top right
1. Click on Directory Contacts
1. Search for the contact you want to delete
1. Select the contact
1. Options should display on the right side of the page after selecting a contact
1. Click on the wrench icon
1. Select Delete Contact




