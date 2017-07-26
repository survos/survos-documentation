Survos Platform
===============

The Survos Platform provides researchers with powerful tools to interact with their study participants.  Participants can interact via random or fixed-interval SMS surveys, provide detailed, continuous information about their location, and collect photos via SMS or our app.  Researchers can extract information about those photos via Amazon's Mechanical Turk, a crowd-sourcing platform.

This documentation provides detailed instructions about what the tools do, and how they are configured.  As with many comprehensive systems, sometimes getting started is the hardest part.  The major parts of the data collection system are broken down into "Modules".  The basic workflow is the same for all the survey types.

Getting Started with Modules
----------------------------

The platform has 4 related but independent *modules*.  Each module collects a different type of data.  All modules
consist of protocols, surveys, waves, tasks, assignments, sets and channels.  These terms will be defined within each module, with examples.
Knowing these terms and how they are connected to each module is key to understanding the platform.

What can you do with the Survos Platform?   These four verbs answer that question, and are the names of the modules:

- **Recruit** recruit and enroll study participants or field workers
- **Study** collect personal data about a set of study participants
- **Audit** get objective (not personal) data about a set of inanimate objects, like images or places
- **Annotate** combination of Study and Audit, collects *personal data* about a set of places or events, basically a personal map or calendar annotation.

In general, the workflow to collect data within any module is as follows:

#. Establish a *set* of who or what those questions will be asked of
#. Configure a *protocol* associated with that set of data and a channel type for how that data will be collected.
#. Design one or more *surveys* -- the questions you want to ask
#. Add one or more surveys and timing information to the protocol, this is called a deployment wave, or simply *wave*.
#. Once the protocol has been configured with surveys and timing information, activate that protocol.

Recruit
-------

.. IMPORTANT::
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

.. TIP::
   Collect personal data about a set of study participants.  Study participants are created in the Recruit module, or by simply creating a participant account.

Participant Set
     The collection of participants who will be enrolled in each wave of this protocol.  The default set is "All Accepted Participants", or you can create a subset like "All participants who self-identify as smokers" or "All participants who have completed with baseline protocols" or "All participants who have completed the observation period and have a compliance score of greater than 80%".

Protocol
     The protocol configuration includes the participant set, the schedule type (e.g. just one time, like a baseline survey, or periodic, like a daily diary, or even a testing schedule, called a "blitz").  If the schedule type is periodic, then the duration of the protocol is also defined.  The method of communication is also defined in the protocol, e.g. SMS or web-based. For example, you can configure the "Observation Protocol" as a 2-week period communicating with pregnant smokers via SMS.  Note that when you initially set up the protocol, there are no surveys or schedules yet -- those come when the wave is configured.
Survey
    A list of questions and answer options.  For protocols with schedule type of for one-time surveys (e.g. a baseline protocol), these questions are likely to be in the form of "Have you ever...?" or "Do you...?"  For periodic protocols, like an observation period, the questions are likely be EMA (Ecological Momentary Assessments, "in-the-moment" surveys), or coverage surveys, like a daily diary.  An EMA survey may have questions in the form "Right now, are you...?", e.g. "Right now, are you with other people?", "Right now, how much do you want to use marijuana?".  A coverage survey typically contains questions like "Thinking about today only, did you purchase any tobacco products?" or "In the last 4 hours, did you exercise?"  The common theme of surveys in the Study Module is that they are questions about the participant.
Wave
    The deployment of the survey questions within a protocol, along with relevant configuration information.  If it's part of a periodic protocol, then the specific schedule is defined here.  Also, the communication channel is defined and the prompt channel (email, SMS, etc.).  Compliance thresholds are set, expiration times, reminders, etc.  The wave is where the majority of the settings are configured, and are defined in detail in this documentation.

A typical study protocol might be for 3 week to send SMS prompts 4 times per day asking participants who have completed the baseline protocol if they have smoked in the last 4 hours, as well as random prompts 6 times per day to ask if they are smoking right now, and if not, what their craving to smoke is.

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
