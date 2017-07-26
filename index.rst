Survos Platform
===============

The Survos Platform provides researchers with powerful tools to interact with their study participants.  Participants can interact via random or fixed-interval SMS surveys, provide detailed, continuous information about their location, and collect photos via SMS or our app.  Researchers can extract information about those photos via Amazon's Mechanical Turk, a crowd-sourcing platform.

This documentation provides detailed instructions about what the tools do, and how they are configured.  As with many comprehensive systems, sometimes getting started is the hardest part.  The major parts of the data collection system are broken down into "Modules".  The basic workflow is the same for all the survey types.

Getting Started
---------------

The platform has 4 related but independent *modules*.  Each module collects a different type of data.  All modules
consist of protocols, surveys, waves, tasks, assignments, sets and channels.  These terms will be defined within each module, with examples.
Knowing these terms and how they are connected to each module is key to understanding the platform.

What can you do with the Survos Platform?   These four verbs answer that question, and are the names of the modules:

- **Recruit** recruit and enroll study participants or field workers
- **Study** collect personal data about a set of study participants
- **Audit** get objective (not personal), data about a set of inanimate objects, like images or places
- **Annotate** combination of Study and Audit, collects *personal data* about a set of *place*s or *event*s, basically a personal map or calendar annotation.

In general, the workflow to collect data within any module is as follows:

* Design one or more *survey*s -- the questions you want to ask
* Establish a *set* of who or what those questions will be asked of
* Configure a *protocol* associated with that set of data and a channel type for how that data will be collected.
* Add one or more surveys and timing information to the protocol, this is called a deployment wave, or simply *wave*.
* Once the protocol has been configured with surveys and timing information, activate that protocol.

Recruit
-------

Recruit and enroll study participants.  The purpose of this module is to create new participant accounts within the system.

Protocol
     The protocol configuration includes how the candidate will take the survey.  In most cases, this will be either self-enrolled via the participant website, or done as an interview by a researcher who will enter the data via the administrative website.
Survey
    A list of questions and answer options.  Answers can have scores associated with them, when a candidate fills out a survey, answers with scores are totaled and can be used in the wave configuration to automatically approve those candidates as participants.
Wave
    The deployment of the survey questions, along with the configuration data specific to automatic enrollment, like the minimum score required.

Most of the example projects use a self-enrollment protocol, with very minimal requirements for actual enrollment.

A typical recruit protocol might be to ask if someone smokes cigarettes, is above 18, and has not tried to quit in the last year.  Based on their answers, they may be accepted in the study.  At that point, they'd have an account tagged as active, and therefore would be added into the "accepted participants" set (used by Study protocols).

Study
-------

Collect personal data about a set of study participants.  Study participants are created in the Recruit module, or by simply creating a participant account.






If your projects has study participants, enable one or more of these modules:

 - *Ongoing*: Continous collection of data about a *participant*, .e.g an SMS survey 3x/day for 2 weeks, see :ref:`ongoing`
 - *Single*: A questionnaire of a participant, often web-based, e.g. "How often did your parents smoke indoors?" *disabled*
 - *Tracking*: Continuous location data (works with tracking app that runs on participant's phone) see *disabled*

We integration with Amazon's Mechanical Turk, to do the following:

 - *Turk Opinion*: Questions are answered by anonymous Turkers see *disabled*
 - *Turk Expert*: Questions are answered by a single, anonymous Turker about an image, place or other piece of data
 - *Turk Consensus*: Questions about things (not people) are answered by multiple, anonymous Turkers until consensus is reached.

If your project has a list of places that need to be visited by field workers, install

 - *Field*: Questions about a list of places visited by field workers.

If your project needs to pre-qualify participants, field-workers, or turkers, install

 - *Screener*: Scored Surveys that pre-qualify participants or Turkers before they begin work.  Unpaid.

Because the modules can be run independently and that often a study needs only one or two modules, this documentation describes each module as if it were a separate project.  While a real-world study may enable multiple modules, keeping them separate makes it easier to learn and understand the system.  In the appendix there are examples of more complex configurations.


Contents:

.. toctree::
    :maxdepth: 1

    getting-started
    workflows
    roles
    modules
    integration-types
    users-participants
    tutorials
    tracking






Indexes and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
