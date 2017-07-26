.. This file was automatically generated from SCRIPT_NAME -- do not modify it except to change the relevant twig file!

..  _RapidPro_integration_type:

RapidPro Integration Types
=======================================
RapidPro

The purpose of this integration is to provide a channel to collect data.


RapidPro Wave Configuration
------------------------

Go through each screen of the Wave Form or Wizard for a RapidPro Wave

RapidPro Basic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `basic Tab in the RapidPro Wave
<http://behattest.stagingsurvos.com/waves/dummy/RapidPro#basic>`_.

.. figure::  /images/modules/stay_RapidPro_basic.png

   Rendered Form RapidPro Wave Tab basic

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    Protocol                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    description                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    integrationTypeCode                </th>
                <td>
                                            <b>Type</b>: string(16)                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Survey Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    How will the survey happen?                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Dedicated Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Deactivate previous waves using this channel                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    scheduleType                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Trigger                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Key word to trigger self-initiated survey                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Prompt Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    How will the prompting happen?  Leave empty if same as survey                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Response Channel                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Channel for response, if different than primary channel (e.g. API)                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    marking                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Schedule                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    help_block_schedule_configuration                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Scheduling Conditions                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Only schedule when these conditions are met, e.g. dayOfWeek in ['Mon','Wed','Fri'] and dayOfMonth != 22
                                Fields: dayOfWeek (.e.g Mon), month (e.g. Jan), dayOfMonth (e.g. 15)                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Start Date                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Starting date of the protocol, when surveys are scheduled / accepted.                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Relative To Start Date                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: Yes<br>
                                                                                    </td>
                <td>
                    +1 for starting the next day                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Specific Start Date                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Only if type is set to specific, otherwise calculated                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Completion Threshold                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Minimum completed prompt percentage to mark as Complete                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Notes                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Allow in Observe                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Send link to web-based survey                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Publish Conditions                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    In addition to the Source Channel Filter                </td>
            </tr>
                    </tbody>
    </table>
    </div>


RapidPro Enrollment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `enrollment Tab in the RapidPro Wave
<http://behattest.stagingsurvos.com/waves/dummy/RapidPro#enrollment>`_.

.. figure::  /images/modules/stay_RapidPro_enrollment.png

   Rendered Form RapidPro Wave Tab enrollment

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                    </tbody>
    </table>
    </div>


RapidPro Task
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `task Tab in the RapidPro Wave
<http://behattest.stagingsurvos.com/waves/dummy/RapidPro#task>`_.

.. figure::  /images/modules/stay_RapidPro_task.png

   Rendered Form RapidPro Wave Tab task

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    Task Title                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Public title                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Description                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Public description of this task                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Deployment Keywords                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Keywords make searching for jobs easier                </td>
            </tr>
                    </tbody>
    </table>
    </div>


RapidPro Expiration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `expiration Tab in the RapidPro Wave
<http://behattest.stagingsurvos.com/waves/dummy/RapidPro#expiration>`_.

.. figure::  /images/modules/stay_RapidPro_expiration.png

   Rendered Form RapidPro Wave Tab expiration

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    Time before expiration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                                    </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Number of Reminders before Expiration                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    If 0, no reminders                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Maximum response time                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Time allowed after first response before marking as abandoned (eg, 5m, 3h, 2d)                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    Number of warnings                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Once responding, number of warnings before marking as abandoned                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    Minimum Time Between Same Surveys                </th>
                <td>
                                            <b>Type</b>: integer                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Delay surveys if necessary by this amount  (eg, 5m, 3h, 2d)                </td>
            </tr>
                    </tbody>
    </table>
    </div>


RapidPro Messages
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This is the form snippet from `messages Tab in the RapidPro Wave
<http://behattest.stagingsurvos.com/waves/dummy/RapidPro#messages>`_.

.. figure::  /images/modules/stay_RapidPro_messages.png

   Rendered Form RapidPro Wave Tab messages

.. raw:: html

    <div class="wy-table-responsive">
    <table border="1" class="docutils">
        <colgroup>
        <col width="15%">
        <col width="25%">
        <col width="60%">
        </colgroup>
        <thead valign="bottom">
            <tr class="row-odd">
                <th class="head">Field</th>
                <th class="head">Info</th>
                <th class="head">Description</th>
            </tr>
        </thead>
        <tbody valign="top">
                                    <tr class="row-odd">
                <th class="head">
                    welcome                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Welcome!                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    welcome                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    welcome Custom Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    taskEnd                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    The task has ended.                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    taskEnd                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    taskEnd Custom Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    prompt                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    Time to take your survey!                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    prompt                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    prompt Custom Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    end                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    The assignment has ended.                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    end                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    end Custom Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    expiration                </th>
                <td>
                                            <b>Type</b>: boolean                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    The assignment has expired                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    expiration                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    expiration Custom Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    reminder                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    Please start your survey.                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    reminder                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    reminder Custom Message                </td>
            </tr>
                                    <tr class="row-odd">
                <th class="head">
                    warning                </th>
                <td>
                                            <b>Type</b>: mixed
                                    </td>
                <td>
                    You have {{ assignment.remainingTimeDisplay}} remaining.                </td>
            </tr>
                                    <tr class="row-even">
                <th class="head">
                    warning                </th>
                <td>
                                            <b>Type</b>: text                            <br>
                        <b>Required</b>: No<br>
                                                                                    </td>
                <td>
                    warning Custom Message                </td>
            </tr>
                    </tbody>
    </table>
    </div>


