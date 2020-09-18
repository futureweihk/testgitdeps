<html xmlns:o="urn:schemas-microsoft-com:office:office"
      xmlns:x="urn:schemas-microsoft-com:office:excel"
      xmlns="http://www.w3.org/TR/REC-html40">
    <head>
        <title>PCL ServiceDesk</title>
        <style type="text/css">
         table {
             mso-displayed-decimal-separator:"\.";
             mso-displayed-thousand-separator:"\,";
         }
         body
         {
             margin: 0px;
             font-size: 12px;
             font-family: Arial, sans-serif;
             color:black;
         }

        </style>
        <META HTTP-EQUIV="Content-Type" Content="application/vnd.ms-excel; charset=UTF-8">
        <!-- JRA-7598 - ensure fields (e.g. description) occupy only one cell - even fields containing newlines. -->
        <!--
             Vertical align all cells to the top, in order to align all issue rows of issuetable to the top,
             since Excel does not use or save the css files it is hardcoded here.
           -->
        <style>
         @page
         {
             mso-page-orientation:landscape;
             margin:.25in .25in .5in .25in;
             mso-header-margin:.5in;
             mso-footer-margin:.25in;
             mso-footer-data:"&R&P of &N";
             mso-horizontal-page-align:center;
             mso-vertical-page-align:center;
         }

         td.issuekey,
         td.issuetype,
         td.status {
             mso-style-parent: "";
             mso-number-format: \@;
             text-align: left;
         }
         br
         {
             mso-data-placement:same-cell;
         }

         td
         {
             vertical-align: top;
         }
        </style>

        <!--[if gte mso 9]><xml>
            <x:ExcelWorkbook>
            <x:ExcelWorksheets>
            <x:ExcelWorksheet>
            <x:Name>general_report</x:Name>
            <x:WorksheetOptions>
            <x:Print>
            <x:ValidPrinterInfo/>
            </x:Print>
            </x:WorksheetOptions>
            </x:ExcelWorksheet>
            </x:ExcelWorksheets>
            </x:ExcelWorkbook>
            </xml><![endif]-->
    </head>
    <body>

        <table border="1">
            <tr bgcolor="#0747a6" height="30">
                <td colspan="300">
                    <img src="http://10.9.17.104:8080/images/jira-generic.png" width="57" height="30" border="0" alt="PCL ServiceDesk">
                </td>
            </tr>
            <tr>
                <td colspan="300">
                    <a href="http://10.9.17.104:8080/issues/?jql=status+%3D+Done+order+by+lastViewed+DESC">PCL ServiceDesk</a>
                </td>
            </tr>
            <tr>
                <td colspan="300">
                    Displaying <strong>214</strong> issues at <strong>18/Sep/2020 11:36 AM</strong>.
                </td>
            </tr>
        </table>

        


                            <issuetable-web-component>
                <table id="issuetable"  border="1" cellpadding="3" cellspacing="1" width="100%">
                        <thead>
        <tr class="rowHeader">
            
                                                            <th class="colHeaderLink headerrow-project" data-id="project">
                            Project
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-issuekey" data-id="issuekey">
                            Key
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-summary" data-id="summary">
                            Summary
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-issuetype" data-id="issuetype">
                            Issue Type
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-status" data-id="status">
                            Status
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-priority" data-id="priority">
                            Priority
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-resolution" data-id="resolution">
                            Resolution
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-assignee" data-id="assignee">
                            Assignee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-reporter" data-id="reporter">
                            Reporter
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-creator" data-id="creator">
                            Creator
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-created" data-id="created">
                            Created
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-lastViewed" data-id="lastViewed">
                            Last Viewed
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-updated" data-id="updated">
                            Updated
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-resolutiondate" data-id="resolutiondate">
                            Resolved
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-versions" data-id="versions">
                            Affects Version/s
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-fixVersions" data-id="fixVersions">
                            Fix Version/s
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-components" data-id="components">
                            Component/s
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-duedate" data-id="duedate">
                            Due Date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-thumbnail" data-id="thumbnail">
                            Images
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-timeoriginalestimate" data-id="timeoriginalestimate">
                            Original Estimate
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-timeestimate" data-id="timeestimate">
                            Remaining Estimate
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-timespent" data-id="timespent">
                            Time Spent
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-workratio" data-id="workratio">
                            Work Ratio
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-subtasks" data-id="subtasks">
                            Sub-Tasks
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-issuelinks" data-id="issuelinks">
                            Linked Issues
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-environment" data-id="environment">
                            Environment
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-description" data-id="description">
                            Description
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-security" data-id="security">
                            Security Level
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-progress" data-id="progress">
                            Progress
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-aggregateprogress" data-id="aggregateprogress">
                            Σ Progress
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-aggregatetimespent" data-id="aggregatetimespent">
                            Σ Time Spent
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-aggregatetimeestimate" data-id="aggregatetimeestimate">
                            Σ Remaining Estimate
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-aggregatetimeoriginalestimate" data-id="aggregatetimeoriginalestimate">
                            Σ Original Estimate
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-labels" data-id="labels">
                            Labels
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11040" data-id="customfield_11040">
                            Excel Delivery Method (OSW Regenerate ATM PIN)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11041" data-id="customfield_11041">
                            Excel Remark (OSW Regenerate ATM PIN)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11042" data-id="customfield_11042">
                            Excel Action (Octopus)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11043" data-id="customfield_11043">
                            Excel Check digit (Octopus)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11044" data-id="customfield_11044">
                            Excel Octopus number (Octopus)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10990" data-id="customfield_10990">
                            Excel Annual Fee Remark
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11045" data-id="customfield_11045">
                            Excel Reload amount (Octopus)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11046" data-id="customfield_11046">
                            Excel Remark (Octopus)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11047" data-id="customfield_11047">
                            Excel Action code (Direct Debit Authorization)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10992" data-id="customfield_10992">
                            Excel Card Replacement Fee Remark
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11048" data-id="customfield_11048">
                            Excel Change to (Direct Debit Authorization)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11049" data-id="customfield_11049">
                            Excel Remark (Direct Debit Authorization)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10994" data-id="customfield_10994">
                            Excel Reprint Statement Fee Remark
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10510" data-id="customfield_10510">
                            Product categorization
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11039" data-id="customfield_11039">
                            Excel Action code (OSW Regenerate ATM PIN)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10984" data-id="customfield_10984">
                            Excel Overlimit Fee Remark1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10500" data-id="customfield_10500">
                            Pending reason
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10985" data-id="customfield_10985">
                            Excel Overlimit Fee Remark2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10501" data-id="customfield_10501">
                            Impact
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10502" data-id="customfield_10502">
                            Change type
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10986" data-id="customfield_10986">
                            Excel Overlimit Fee Remark3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10503" data-id="customfield_10503">
                            Change risk
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10504" data-id="customfield_10504">
                            Change reason
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10988" data-id="customfield_10988">
                            Excel Absorb Odd Dollars Remark
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10505" data-id="customfield_10505">
                            Change start date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10506" data-id="customfield_10506">
                            Change completion date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10507" data-id="customfield_10507">
                            Urgency
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10508" data-id="customfield_10508">
                            Change managers
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10509" data-id="customfield_10509">
                            CAB
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11030" data-id="customfield_11030">
                            Excel Delivery Method (Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11031" data-id="customfield_11031">
                            Excel Remark (Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11032" data-id="customfield_11032">
                            Excel Waive Handling (Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11033" data-id="customfield_11033">
                            Excel Waive Handling Fee (Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11034" data-id="customfield_11034">
                            Excel Action (OSW Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10980" data-id="customfield_10980">
                            Excel Autopay Reject Fee Remark3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11035" data-id="customfield_11035">
                            Excel Delivery Method (OSW Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11036" data-id="customfield_11036">
                            Excel Remark (OSW Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11037" data-id="customfield_11037">
                            Excel Waive Handling (OSW Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11038" data-id="customfield_11038">
                            Excel Waive Handling Fee (OSW Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11028" data-id="customfield_11028">
                            Excel Action (Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10973" data-id="customfield_10973">
                            Excel Finance Charge Remark2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11029" data-id="customfield_11029">
                            Excel Action code (Card Replacement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10974" data-id="customfield_10974">
                            Excel Finance Charge Remark3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10978" data-id="customfield_10978">
                            Excel Autopay Reject Fee Remark1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10979" data-id="customfield_10979">
                            Excel Autopay Reject Fee Remark2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11020" data-id="customfield_11020">
                            Excel Delivery Method (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11021" data-id="customfield_11021">
                            Excel Level (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11022" data-id="customfield_11022">
                            Excel Remark (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11023" data-id="customfield_11023">
                            Excel Waive Handling (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11024" data-id="customfield_11024">
                            Excel Waive Handling Fee (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11025" data-id="customfield_11025">
                            Excel Cardholder Name
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10970" data-id="customfield_10970">
                            Excel Late Charge Remark2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11026" data-id="customfield_11026">
                            Card Maintenance Service
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10971" data-id="customfield_10971">
                            Excel Late Charge Remark3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10972" data-id="customfield_10972">
                            Excel Finance Charge Remark1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11027" data-id="customfield_11027">
                            Fee Maintenance Service
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11017" data-id="customfield_11017">
                            Excel Bank Account (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10962" data-id="customfield_10962">
                            cb_Other
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11018" data-id="customfield_11018">
                            Excel Block Code (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10600" data-id="customfield_10600">
                            System Team
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10963" data-id="customfield_10963">
                            cb_OverseasTransactionActivation
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11019" data-id="customfield_11019">
                            Excel Credit Balance Refund (Credit Balance Refund)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10964" data-id="customfield_10964">
                            cb_ReprintStatement
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10602" data-id="customfield_10602">
                            Involved Category
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10965" data-id="customfield_10965">
                            Org
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10603" data-id="customfield_10603">
                            Post Checker
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10969" data-id="customfield_10969">
                            Excel Late Charge Remark1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11010" data-id="customfield_11010">
                            Excel Late Charge1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11011" data-id="customfield_11011">
                            Excel Late Charge2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11012" data-id="customfield_11012">
                            Excel Late Charge3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11013" data-id="customfield_11013">
                            Excel Overlimit Fee1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11014" data-id="customfield_11014">
                            Excel Overlimit Fee2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11015" data-id="customfield_11015">
                            Excel Overlimit Fee3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10960" data-id="customfield_10960">
                            cb_OptIn
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11016" data-id="customfield_11016">
                            Excel Reprint Statement Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10961" data-id="customfield_10961">
                            cb_OptOut
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11006" data-id="customfield_11006">
                            Excel Cash Back
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10951" data-id="customfield_10951">
                            Other
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11007" data-id="customfield_11007">
                            Excel Finance Charge1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10952" data-id="customfield_10952">
                            Overseas Transaction Activation
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11008" data-id="customfield_11008">
                            Excel Finance Charge2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10953" data-id="customfield_10953">
                            Reprint Statement
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11009" data-id="customfield_11009">
                            Excel Finance Charge3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10954" data-id="customfield_10954">
                            cb_CardCancellation
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10955" data-id="customfield_10955">
                            cb_CardReplacement
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10956" data-id="customfield_10956">
                            cb_CreditBalanceRefund
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10957" data-id="customfield_10957">
                            cb_DirectDebitAuthorization
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10958" data-id="customfield_10958">
                            cb_OSWCardReplacement
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10959" data-id="customfield_10959">
                            cb_OSWRegenerateATM_PIN
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11000" data-id="customfield_11000">
                            Excel Absorb Odd Dollars
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11001" data-id="customfield_11001">
                            Excel Annual Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11002" data-id="customfield_11002">
                            Excel Autopay Reject Fee1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11003" data-id="customfield_11003">
                            Excel Autopay Reject Fee2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11004" data-id="customfield_11004">
                            Excel Autopay Reject Fee3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11005" data-id="customfield_11005">
                            Excel Card Replacement Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10950" data-id="customfield_10950">
                            Opt Out
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10940" data-id="customfield_10940">
                            checkers
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10941" data-id="customfield_10941">
                            Task Summary
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10942" data-id="customfield_10942">
                            Task IT Manager
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10943" data-id="customfield_10943">
                            Card Cancellation
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10944" data-id="customfield_10944">
                            Card Replacement
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10945" data-id="customfield_10945">
                            Credit Balance Refund
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10946" data-id="customfield_10946">
                            Direct Debit Authorization
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10947" data-id="customfield_10947">
                            OSW Card Replacement
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10948" data-id="customfield_10948">
                            OSW Regenerate ATM PIN
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10949" data-id="customfield_10949">
                            Opt In
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10930" data-id="customfield_10930">
                            Annual Fee Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10931" data-id="customfield_10931">
                            Cash Back Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10810" data-id="customfield_10810">
                            Related System
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10932" data-id="customfield_10932">
                            Absorb Odd Dollars Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10811" data-id="customfield_10811">
                            Prod Owners
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10933" data-id="customfield_10933">
                            Card Replacement Fee Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10813" data-id="customfield_10813">
                            New Equipment
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10934" data-id="customfield_10934">
                            Reprint Statement Fee Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10815" data-id="customfield_10815">
                            Others Detail
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10816" data-id="customfield_10816">
                            Sample
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10938" data-id="customfield_10938">
                            cb_Octopus
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10939" data-id="customfield_10939">
                            Octopus
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11100" data-id="customfield_11100">
                            Task Involved Category
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11101" data-id="customfield_11101">
                            General Info
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10920" data-id="customfield_10920">
                            Cardholder information
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10800" data-id="customfield_10800">
                            User authentication
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10921" data-id="customfield_10921">
                            single-approver
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10801" data-id="customfield_10801">
                            Access Control
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10922" data-id="customfield_10922">
                            multi-approver
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10802" data-id="customfield_10802">
                            Backup&amp;Recovery
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10923" data-id="customfield_10923">
                            Logo
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10803" data-id="customfield_10803">
                            System Monitoring
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10804" data-id="customfield_10804">
                            Target Date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10925" data-id="customfield_10925">
                            cb_AbsorbOddDollars
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10926" data-id="customfield_10926">
                            Late Charge Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10805" data-id="customfield_10805">
                            Reasons for High Priority Case
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10806" data-id="customfield_10806">
                            Branch/Department
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10927" data-id="customfield_10927">
                            Finance Charge Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10807" data-id="customfield_10807">
                            Need Create GL Code
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10928" data-id="customfield_10928">
                            Overlimit Fee Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10929" data-id="customfield_10929">
                            Autopay Reject Fee Total
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10808" data-id="customfield_10808">
                            New GL Code
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10809" data-id="customfield_10809">
                            CFO
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10000" data-id="customfield_10000">
                            Request participants
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10001" data-id="customfield_10001">
                            Customer Request Type
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10002" data-id="customfield_10002">
                            Organizations
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10910" data-id="customfield_10910">
                            Reprint Statement Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10911" data-id="customfield_10911">
                            cb_LateCharge
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10912" data-id="customfield_10912">
                            cb_FinanceCharge
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10913" data-id="customfield_10913">
                            cb_Overlimit
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10914" data-id="customfield_10914">
                            cb_AutopayReject
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10915" data-id="customfield_10915">
                            cb_Annual
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10916" data-id="customfield_10916">
                            cb_CashBack
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10917" data-id="customfield_10917">
                            cb_CardReplacementFee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10918" data-id="customfield_10918">
                            cb_ReprintStatementFee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10919" data-id="customfield_10919">
                            cb_Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11200" data-id="customfield_11200">
                            Others(Detail)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11201" data-id="customfield_11201">
                            Additional Info
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10104" data-id="customfield_10104">
                            Time to resolution
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10105" data-id="customfield_10105">
                            Time to first response
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10900" data-id="customfield_10900">
                            Target User
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10902" data-id="customfield_10902">
                            Late Charge
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10903" data-id="customfield_10903">
                            Finance Charge
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10904" data-id="customfield_10904">
                            Overlimit Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10905" data-id="customfield_10905">
                            Autopay Reject Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10906" data-id="customfield_10906">
                            Annual Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10907" data-id="customfield_10907">
                            Cash Back
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10908" data-id="customfield_10908">
                            Absorb odd dollars
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10909" data-id="customfield_10909">
                            Card Replacement Fee
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10101" data-id="customfield_10101">
                            Satisfaction
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10103" data-id="customfield_10103">
                            Approvers
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10330" data-id="customfield_10330">
                            Password Owner
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10331" data-id="customfield_10331">
                            Change completion date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11300" data-id="customfield_11300">
                            IT Admin
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10332" data-id="customfield_10332">
                            Time to approve normal change
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10333" data-id="customfield_10333">
                            Time to close after resolution
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10324" data-id="customfield_10324">
                            Workaround
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10325" data-id="customfield_10325">
                            Change risk
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10326" data-id="customfield_10326">
                            Change managers
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10205" data-id="customfield_10205">
                            Rank
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10206" data-id="customfield_10206">
                            Development
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10327" data-id="customfield_10327">
                            Prod Owner
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10328" data-id="customfield_10328">
                            Dept Head
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10329" data-id="customfield_10329">
                            PO&amp;Special Approver
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10320" data-id="customfield_10320">
                            Urgency
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10321" data-id="customfield_10321">
                            Change reason
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10200" data-id="customfield_10200">
                            Sprint
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10322" data-id="customfield_10322">
                            Deploy Operator
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10201" data-id="customfield_10201">
                            Epic Link
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10323" data-id="customfield_10323">
                            New or Change
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10313" data-id="customfield_10313">
                            Future-UserPicker2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10314" data-id="customfield_10314">
                            Change start date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10315" data-id="customfield_10315">
                            CTO
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10316" data-id="customfield_10316">
                            Future: single user select-manager
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10317" data-id="customfield_10317">
                            Product categorization
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10318" data-id="customfield_10318">
                            CAB
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11406" data-id="customfield_11406">
                            Gitlab comment count
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10319" data-id="customfield_10319">
                            Root cause
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11080" data-id="customfield_11080">
                            Excel Attachment Filename3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11081" data-id="customfield_11081">
                            Excel Attachment Link1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11082" data-id="customfield_11082">
                            Excel Attachment Link2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11083" data-id="customfield_11083">
                            Excel Attachment Link3
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11084" data-id="customfield_11084">
                            Excel Approver
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11085" data-id="customfield_11085">
                            Excel Approval Date
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11086" data-id="customfield_11086">
                            System Enhance
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11087" data-id="customfield_11087">
                            Cardholder Date information
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10310" data-id="customfield_10310">
                            Source
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10311" data-id="customfield_10311">
                            Security Manager
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10312" data-id="customfield_10312">
                            Investigation reason
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10302" data-id="customfield_10302">
                            Impact
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10303" data-id="customfield_10303">
                            IT Manager
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10304" data-id="customfield_10304">
                            Operational categorization
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10305" data-id="customfield_10305">
                            Pending reason
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10306" data-id="customfield_10306">
                            System Owner
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10307" data-id="customfield_10307">
                            Change type
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10308" data-id="customfield_10308">
                            IT Head
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10309" data-id="customfield_10309">
                            Future-UserPicker
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11070" data-id="customfield_11070">
                            Excel Remark (Reprint Statement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11071" data-id="customfield_11071">
                            Excel Reprint Period from (Reprint Statement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11072" data-id="customfield_11072">
                            Excel Reprint Period to (Reprint Statement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11073" data-id="customfield_11073">
                            Excel Waive Handling (Reprint Statement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11074" data-id="customfield_11074">
                            Excel Waive Handling Fee (Reprint Statement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11075" data-id="customfield_11075">
                            Excel Other (Other)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11076" data-id="customfield_11076">
                            test attachment form
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11077" data-id="customfield_11077">
                            New Staff
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11078" data-id="customfield_11078">
                            Excel Attachment Filename1
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11079" data-id="customfield_11079">
                            Excel Attachment Filename2
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10300" data-id="customfield_10300">
                            Source Review
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10301" data-id="customfield_10301">
                            Need Apply Password
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11060" data-id="customfield_11060">
                            Excel Reason (Card Cancellation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11061" data-id="customfield_11061">
                            Excel Remark (Card Cancellation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11062" data-id="customfield_11062">
                            Excel Virtual card (Card Cancellation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11063" data-id="customfield_11063">
                            Excel Whole Account Level (Card Cancellation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11064" data-id="customfield_11064">
                            Excel Action code (Overseas Transaction Activation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11065" data-id="customfield_11065">
                            Excel Daily available Limit (Overseas Transaction Activation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11066" data-id="customfield_11066">
                            Excel Duration From (Overseas Transaction Activation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11067" data-id="customfield_11067">
                            Excel Duration To (Overseas Transaction Activation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11068" data-id="customfield_11068">
                            Excel Remark (Overseas Transaction Activation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11069" data-id="customfield_11069">
                            Excel Action code (Reprint Statement)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10401" data-id="customfield_10401">
                            Account Type
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10404" data-id="customfield_10404">
                            Engineer
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11050" data-id="customfield_11050">
                            Excel Action code (Opt In)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11051" data-id="customfield_11051">
                            Excel Opt In (Opt In)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11052" data-id="customfield_11052">
                            Excel Other (Opt In)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11053" data-id="customfield_11053">
                            Excel Remark (Opt In)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11054" data-id="customfield_11054">
                            Excel Action code (Opt out)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11055" data-id="customfield_11055">
                            Excel Opt out (Opt out)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11056" data-id="customfield_11056">
                            Excel Other (Opt out)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11057" data-id="customfield_11057">
                            Excel Remark (Opt out)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11058" data-id="customfield_11058">
                            Excel Action Code (Card Cancellation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11059" data-id="customfield_11059">
                            Excel Level (Card Cancellation)
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10511" data-id="customfield_10511">
                            Operational categorization
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10996" data-id="customfield_10996">
                            Excel Cash Back Remark
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10512" data-id="customfield_10512">
                            Source
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10513" data-id="customfield_10513">
                            Investigation reason
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10514" data-id="customfield_10514">
                            Root cause
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10515" data-id="customfield_10515">
                            Workaround
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10516" data-id="customfield_10516">
                            Software Type
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10518" data-id="customfield_10518">
                            System Category
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10203" data-id="customfield_10203">
                            Epic Name
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10204" data-id="customfield_10204">
                            Epic Color
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10207" data-id="customfield_10207">
                            Story Points
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10202" data-id="customfield_10202">
                            Epic Status
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11403" data-id="customfield_11403">
                            Severity
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11402" data-id="customfield_11402">
                            Additional information
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11405" data-id="customfield_11405">
                            External issue ID
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11404" data-id="customfield_11404">
                            Priority
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11401" data-id="customfield_11401">
                            Steps to reproduce
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_11400" data-id="customfield_11400">
                            External issue URL
                                                    </th>
                                                
                                                            <th class="colHeaderLink headerrow-customfield_10403" data-id="customfield_10403">
                            Special Approver
                                                    </th>
                                                                    </tr>
    </thead>
    <tbody>
                    

                <tr id="issuerow12901" rel="12901" data-issuekey="ITJR-1092" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1092" href="http://10.9.17.104:8080/browse/ITJR-1092">ITJR-1092</a>
</td>
                                            <td class="summary"><p>
                Apply a new monitor, 2k, 28&quot;
    </p>
</td>
                                            <td class="issuetype">    Purchase Equipment
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           High
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 03/Aug/2020 10:28 PM </td>
                                            <td class="lastViewed"> 16/Sep/2020 6:33 PM </td>
                                            <td class="updated"> 04/Aug/2020 2:21 PM </td>
                                            <td class="resolutiondate"> 04/Aug/2020 2:21 PM </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description">      My monitor currently in use does not work well, I need a new monitor for article editing. 
  </td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>Summary</th></tr><tr><td>Apply a new monitor, 2k, 28&quot;</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-08-07T00:00:00.000Z</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="07/Aug/2020"><time datetime="2020-08-07">07/Aug/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805">      Cannot work without monitor. 
  </td>
                                            <td class="customfield_10806">    Business Intelligence
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/c944566a-e8a7-431e-ac3c-c662840459fe" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;Computer Equipment&quot;,&quot;rtIconId&quot;:10512}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10512" />
                                        Computer Equipment
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1092&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1092&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1092&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1092&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00ar3:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            future.wei
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12901" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403">            pro.special_aprv1
    </td>
                    </tr>


                <tr id="issuerow12902" rel="12902" data-issuekey="ITJR-1093" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1093" href="http://10.9.17.104:8080/browse/ITJR-1093">ITJR-1093</a>
</td>
                                            <td class="summary"><p>
                Apply a monitor, 2k, 28&#39;&#39;
    </p>
</td>
                                            <td class="issuetype">    Purchase Equipment
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           High
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 04/Aug/2020 4:43 PM </td>
                                            <td class="lastViewed"> 05/Aug/2020 5:59 PM </td>
                                            <td class="updated"> 04/Aug/2020 5:32 PM </td>
                                            <td class="resolutiondate"> 04/Aug/2020 5:32 PM </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description">      My monitor is broken, please help. 
  </td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>Summary</th></tr><tr><td>Apply a monitor, 2k, 28&#x27;&#x27;</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-08-07T00:00:00.000Z</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="07/Aug/2020"><time datetime="2020-08-07">07/Aug/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805">      Cannot work without monitor. 
  </td>
                                            <td class="customfield_10806">    Business Intelligence
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/c944566a-e8a7-431e-ac3c-c662840459fe" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;Computer Equipment&quot;,&quot;rtIconId&quot;:10512}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10512" />
                                        Computer Equipment
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1093&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1093&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1093&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1093&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00arb:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12902" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403">            pro.special_aprv1
    </td>
                    </tr>


                <tr id="issuerow12803" rel="12803" data-issuekey="SOFT-413" class="issuerow">
                                            <td class="project">    Software
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="SOFT-413" href="http://10.9.17.104:8080/browse/SOFT-413">SOFT-413</a>
</td>
                                            <td class="summary"><p>
                Task #1 Deployment
    </p>
</td>
                                            <td class="issuetype">    Deploy Task
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution">    <em>Unresolved</em>
</td>
                                            <td class="assignee">            pro.prod_owner1
    </td>
                                            <td class="reporter">            pro.it_developer2
    </td>
                                            <td class="creator">            pro.it_developer2
    </td>
                                            <td class="created"> 09/Jun/2020 11:11 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 10/Jun/2020 12:48 AM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components">    &nbsp;
</td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                                        SOFT-410                        </td>
                                            <td class="environment"></td>
                                            <td class="description">      Deployment Task #1 Description
  </td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels">    </td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603">            pro.it_manager2
    </td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804"></td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806"></td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"></td>
                                            <td class="customfield_10001"></td>
                                            <td class="customfield_10002"></td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-413&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-413&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330">            pro.prod_owner1
    </td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300"></td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-413&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-413&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00aqn:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328"></td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322">            pro.it_developer1
    </td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311">            pro.security_manager1
    </td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306">            pro.it_manager1
    </td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12803" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Done
</td>
                                            <td class="customfield_10301">    Yes
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404"></td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12800" rel="12800" data-issuekey="SOFT-410" class="issuerow">
                                            <td class="project">    Software
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="SOFT-410" href="http://10.9.17.104:8080/browse/SOFT-410">SOFT-410</a>
</td>
                                            <td class="summary"><p>
                Task - Test Task #1 Summary | Multiple Tasks | System Enhancement
    </p>
</td>
                                            <td class="issuetype">    System Enhancement Task
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution">    <em>Unresolved</em>
</td>
                                            <td class="assignee">            pro.it_developer2
    </td>
                                            <td class="reporter">            IT-Service Desk
    </td>
                                            <td class="creator">            IT-Service Desk
    </td>
                                            <td class="created"> 09/Jun/2020 4:10 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 10/Jun/2020 12:48 AM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components">    &nbsp;
</td>
                                            <td class="duedate">    11/Jun/2020
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                                        ITJR-1088,                                                SOFT-413                        </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels">    </td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804"></td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806"></td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"></td>
                                            <td class="customfield_10001"></td>
                                            <td class="customfield_10002"></td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-410&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-410&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300"></td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-410&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-410&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00apz:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327"></td>
                                            <td class="customfield_10328"></td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308"></td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12800" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer2
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12780" rel="12780" data-issuekey="ITJR-1088" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1088" href="http://10.9.17.104:8080/browse/ITJR-1088">ITJR-1088</a>
</td>
                                            <td class="summary"><p>
                Test Task #1 Summary | Multiple Tasks | System Enhancement
    </p>
</td>
                                            <td class="issuetype">    Task
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution">    <em>Unresolved</em>
</td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            IT-Service Desk
    </td>
                                            <td class="created"> 09/Jun/2020 3:44 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 10/Jun/2020 12:48 AM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components">    &nbsp;
</td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                                        SOFT-410                        </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels">    </td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


    <div class="shorten" id="customfield_10602-field">
        							<span>Loan</span>,			        							<span>STA</span>,			        							<span>GL</span>			            </div>
</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804"></td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806"></td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/d1efa1d6-e90b-4d68-8375-7e4fa27326f3" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;Task&quot;,&quot;rtIconId&quot;:10530}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10530" />
                                        Task
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1088&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1088&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300"></td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1088&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1088&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00apb:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327"></td>
                                            <td class="customfield_10328"></td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201">
            Parent Epic Link
    </td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303">            pro.it_manager2
    </td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308"></td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12780" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404"></td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12775" rel="12775" data-issuekey="SOFT-409" class="issuerow">
                                            <td class="project">    Software
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="SOFT-409" href="http://10.9.17.104:8080/browse/SOFT-409">SOFT-409</a>
</td>
                                            <td class="summary"><p>
                Single Task - Enhance Loan Application System
    </p>
</td>
                                            <td class="issuetype">    Single Task
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution">    <em>Unresolved</em>
</td>
                                            <td class="assignee">            pro.it_developer2
    </td>
                                            <td class="reporter">            pro.it_manager1
    </td>
                                            <td class="creator">            IT-Service Desk
    </td>
                                            <td class="created"> 09/Jun/2020 11:47 AM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 09/Jun/2020 12:35 PM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components">    &nbsp;
</td>
                                            <td class="duedate">    10/Jun/2020
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                                        ITJR-1085                        </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels">    </td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804"></td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806"></td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"></td>
                                            <td class="customfield_10001"></td>
                                            <td class="customfield_10002"></td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-409&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-409&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300"></td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-409&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;SOFT-409&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00ao7:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327"></td>
                                            <td class="customfield_10328"></td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311">            pro.security_manager1
    </td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12775" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer2
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12774" rel="12774" data-issuekey="ITJR-1085" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1085" href="http://10.9.17.104:8080/browse/ITJR-1085">ITJR-1085</a>
</td>
                                            <td class="summary"><p>
                Enhance Loan Application System
    </p>
</td>
                                            <td class="issuetype">    Epic
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.it_manager1
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 08/Jun/2020 9:56 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 09/Jun/2020 1:33 PM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                                        SOFT-409                        </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800">    Yes
</td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801">    Yes
</td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802">    Yes
</td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803">    Yes
</td>
                                            <td class="customfield_10804">          <span title="09/Jun/2020"><time datetime="2020-06-09">09/Jun/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805">      Too old
  </td>
                                            <td class="customfield_10806">    Aberdeen-231
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/93c43eae-6599-45ad-b730-5414d89f57a5" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;System Enhancement&quot;,&quot;rtIconId&quot;:10500}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10500" />
                                        System Enhancement
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1085&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1085&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1085&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1085&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00anz:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"><div class="shorten" id="customfield_10329-field">
                        pro.special_aprv1            </div>
</td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315">            pro.ceo1
    </td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>Summary</th></tr><tr><td>Enhance Loan Application System</td></tr></div><div><tr><th>New GL Code</th></tr><tr><td>000</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-06-09T00:00:00.000Z</td></tr></div><div><tr><th>Description</th></tr><tr><td>Test Description for System Enhancement</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311">            pro.security_manager1
    </td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303">            pro.it_manager1
    </td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12774" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404"></td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518">    Loan System
             - product data (e.g. loan amount,tenor,yield,etc.) and customer data of Local loan/credit card/auto loan/mortgage loan
    </td>
                                            <td class="customfield_10203">      Parent Epic Link
  </td>
                                            <td class="customfield_10204">      ghx-label-3
  </td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202">    To Do
</td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12773" rel="12773" data-issuekey="ITJR-1084" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1084" href="http://10.9.17.104:8080/browse/ITJR-1084">ITJR-1084</a>
</td>
                                            <td class="summary"><p>
                New Staff Request
    </p>
</td>
                                            <td class="issuetype">    System Account
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 08/Jun/2020 11:56 AM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 08/Jun/2020 5:01 PM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


    <div class="shorten" id="customfield_10810-field">
        							<span>Loan</span>,			        							<span>CIC</span>,			        							<span>Email</span>,			        							<span>Computer Login</span>,			        							<span>Mobile Mail</span>,			        							<span>VPN</span>,			        							<span>Credit Card</span>,			        							<span>Sales App</span>,			        							<span>Mobile App CMS</span>,			        							<span>Website CMS</span>,			        							<span>Data Warehouse</span>,			        							<span>SunSystem</span>,			        							<span>OPEL</span>			            </div>
</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"><div class="shorten" id="customfield_10811-field">
                        Alfred Chan,                                 Bernie Yip,                                 Bryant Leung,                                 Tommy Au            </div>
</td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


    <div class="shorten" id="customfield_10813-field">
        							<span>Computer</span>,			        							<span>Telephone</span>,			        							<span>Others</span>			            </div>
</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="09/Jun/2020"><time datetime="2020-06-09">09/Jun/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806">    Aberdeen-231
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/f170342b-1e00-4fb5-8691-7869331162ec" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;New Staff Setup&quot;,&quot;rtIconId&quot;:10531}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10531" />
                                        New Staff Setup
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200">      Mac Book Specially Request
  </td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1084&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1084&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1084&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1084&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00anr:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12773" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>New Equipment</th></tr><tr><td>Computer, Telephone, Others</td></tr></div><div><tr><th>If tick &quot;Others&quot;, please specify</th></tr><tr><td>Mac Book Specially Request</td></tr></div><div><tr><th>Summary</th></tr><tr><td>New Staff Request</td></tr></div><div><tr><th>Additional Info</th></tr><tr><td></td></tr></div><div><tr><th>Related System</th></tr><tr><td>Loan, CIC, Email, Computer Login, Mobile Mail</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-06-09T00:00:00.000Z</td></tr></div><div><tr><th></th></tr><tr><td>VPN, Credit Card, Sales App, Mobile App CMS</td></tr></div><div><tr><th></th></tr><tr><td>Website CMS, Data Warehouse, SunSystem, OPEL</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403">            pro.special_aprv1
    </td>
                    </tr>


                <tr id="issuerow12772" rel="12772" data-issuekey="ITJR-1083" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1083" href="http://10.9.17.104:8080/browse/ITJR-1083">ITJR-1083</a>
</td>
                                            <td class="summary"><p>
                Problem in Email Account
    </p>
</td>
                                            <td class="issuetype">    General
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 07/Jun/2020 11:00 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 08/Jun/2020 11:36 AM </td>
                                            <td class="resolutiondate"> 08/Jun/2020 11:36 AM </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>Summary</th></tr><tr><td>Problem in Email Account</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-06-08T00:00:00.000Z</td></tr></div><div><tr><th>Description </th></tr><tr><td>Error</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="08/Jun/2020"><time datetime="2020-06-08">08/Jun/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805">      Test Reason
  </td>
                                            <td class="customfield_10806">    Aberdeen-231
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/6de43487-f344-457e-93b2-0bd39df879ed" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;Get IT Help&quot;,&quot;rtIconId&quot;:10530}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10530" />
                                        Get IT Help
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1083&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1083&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1083&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1083&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00anj:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12772" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403">            pro.special_aprv1
    </td>
                    </tr>


                <tr id="issuerow12771" rel="12771" data-issuekey="ITJR-1082" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1082" href="http://10.9.17.104:8080/browse/ITJR-1082">ITJR-1082</a>
</td>
                                            <td class="summary"><p>
                Notebook
    </p>
</td>
                                            <td class="issuetype">    Purchase Equipment
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 05/Jun/2020 4:59 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 07/Jun/2020 9:58 PM </td>
                                            <td class="resolutiondate"> 07/Jun/2020 9:58 PM </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>Summary</th></tr><tr><td>Notebook</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-06-06T00:00:00.000Z</td></tr></div><div><tr><th>Description </th></tr><tr><td>For Testing Notebook</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="06/Jun/2020"><time datetime="2020-06-06">06/Jun/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806">    Aberdeen-231
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/c944566a-e8a7-431e-ac3c-c662840459fe" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;Computer Equipment&quot;,&quot;rtIconId&quot;:10512}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10512" />
                                        Computer Equipment
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1082&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1082&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1082&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1082&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00anb:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12771" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403">            pro.special_aprv1
    </td>
                    </tr>


                <tr id="issuerow12769" rel="12769" data-issuekey="ITJR-1080" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1080" href="http://10.9.17.104:8080/browse/ITJR-1080">ITJR-1080</a>
</td>
                                            <td class="summary"><p>
                test new staff setup
    </p>
</td>
                                            <td class="issuetype">    System Account
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 04/Jun/2020 2:56 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 04/Jun/2020 3:17 PM </td>
                                            <td class="resolutiondate"> &nbsp; </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


    <div class="shorten" id="customfield_10810-field">
        							<span>Loan</span>,			        							<span>CIC</span>,			        							<span>Email</span>,			        							<span>Computer Login</span>,			        							<span>Mobile Mail</span>,			        							<span>VPN</span>,			        							<span>Credit Card</span>,			        							<span>Sales App</span>,			        							<span>Mobile App CMS</span>,			        							<span>Website CMS</span>,			        							<span>Data Warehouse</span>,			        							<span>SunSystem</span>,			        							<span>OPEL</span>			            </div>
</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"><div class="shorten" id="customfield_10811-field">
                        Alfred Chan,                                 Bernie Yip,                                 Bryant Leung,                                 Tommy Au            </div>
</td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


    <div class="shorten" id="customfield_10813-field">
        							<span>Computer</span>,			        							<span>Others</span>			            </div>
</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="05/Jun/2020"><time datetime="2020-06-05">05/Jun/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805"></td>
                                            <td class="customfield_10806">    Aberdeen-231
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/f170342b-1e00-4fb5-8691-7869331162ec" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;New Staff Setup&quot;,&quot;rtIconId&quot;:10531}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10531" />
                                        New Staff Setup
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200">      test equipment
  </td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1080&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1080&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1080&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1080&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00amv:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12769" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>New Equipment</th></tr><tr><td>Computer, Others</td></tr></div><div><tr><th>If tick &quot;Others&quot;, please specify</th></tr><tr><td>test equipment</td></tr></div><div><tr><th>Summary</th></tr><tr><td>test new staff setup</td></tr></div><div><tr><th>Additional Info</th></tr><tr><td></td></tr></div><div><tr><th>Related System</th></tr><tr><td>Loan, CIC, Email, Computer Login, Mobile Mail</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-06-05T00:00:00.000Z</td></tr></div><div><tr><th></th></tr><tr><td>VPN, Credit Card, Sales App, Mobile App CMS</td></tr></div><div><tr><th></th></tr><tr><td>Website CMS, Data Warehouse, SunSystem, OPEL</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12768" rel="12768" data-issuekey="ITJR-1079" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1079" href="http://10.9.17.104:8080/browse/ITJR-1079">ITJR-1079</a>
</td>
                                            <td class="summary"><p>
                Test IT Support
    </p>
</td>
                                            <td class="issuetype">    General
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 04/Jun/2020 2:18 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 04/Jun/2020 2:53 PM </td>
                                            <td class="resolutiondate"> 04/Jun/2020 2:53 PM </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


</td>
                                            <td class="customfield_11016"></td>
                                            <td class="customfield_10961">


</td>
                                            <td class="customfield_11006"></td>
                                            <td class="customfield_10951">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11154" customFieldId="10951"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11007"></td>
                                            <td class="customfield_10952">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11155" customFieldId="10952"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11008"></td>
                                            <td class="customfield_10953">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11156" customFieldId="10953"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11009"></td>
                                            <td class="customfield_10954">


</td>
                                            <td class="customfield_10955">


</td>
                                            <td class="customfield_10956">


</td>
                                            <td class="customfield_10957">


</td>
                                            <td class="customfield_10958">


</td>
                                            <td class="customfield_10959">


</td>
                                            <td class="customfield_11000"></td>
                                            <td class="customfield_11001"></td>
                                            <td class="customfield_11002"></td>
                                            <td class="customfield_11003"></td>
                                            <td class="customfield_11004"></td>
                                            <td class="customfield_11005"></td>
                                            <td class="customfield_10950">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11153" customFieldId="10950"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10940"></td>
                                            <td class="customfield_10941"></td>
                                            <td class="customfield_10942"></td>
                                            <td class="customfield_10943">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11146" customFieldId="10943"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10944">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11147" customFieldId="10944"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10945">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11148" customFieldId="10945"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10946">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11149" customFieldId="10946"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10947">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11150" customFieldId="10947"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10948">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11151" customFieldId="10948"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10949">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11152" customFieldId="10949"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10930"></td>
                                            <td class="customfield_10931"></td>
                                            <td class="customfield_10810">


</td>
                                            <td class="customfield_10932"></td>
                                            <td class="customfield_10811"></td>
                                            <td class="customfield_10933"></td>
                                            <td class="customfield_10813">


</td>
                                            <td class="customfield_10934"></td>
                                            <td class="customfield_10815"></td>
                                            <td class="customfield_10816">


</td>
                                            <td class="customfield_10938">


</td>
                                            <td class="customfield_10939">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11142" customFieldId="10939"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11100">


</td>
                                            <td class="customfield_11101">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11301" customFieldId="11101"></div>
    <div class="jsd-bundled-fields-static-table">
        <div><style>td, th { padding: 5px }</style><table><div><tr><th>Summary</th></tr><tr><td>Test IT Support</td></tr></div><div><tr><th>Target Date</th></tr><tr><td>2020-06-05T00:00:00.000Z</td></tr></div><div><tr><th>Description </th></tr><tr><td>Test IT Support Description</td></tr></div></table></div>
    </div>
</div>
</td>
                                            <td class="customfield_10920">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11123" customFieldId="10920"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10800"></td>
                                            <td class="customfield_10921"></td>
                                            <td class="customfield_10801"></td>
                                            <td class="customfield_10922"></td>
                                            <td class="customfield_10802"></td>
                                            <td class="customfield_10923"></td>
                                            <td class="customfield_10803"></td>
                                            <td class="customfield_10804">          <span title="05/Jun/2020"><time datetime="2020-06-05">05/Jun/2020</time></span>
    </td>
                                            <td class="customfield_10925">


</td>
                                            <td class="customfield_10926"></td>
                                            <td class="customfield_10805">      test IT support description 
  </td>
                                            <td class="customfield_10806">    Aberdeen-231
</td>
                                            <td class="customfield_10927"></td>
                                            <td class="customfield_10807"></td>
                                            <td class="customfield_10928"></td>
                                            <td class="customfield_10929"></td>
                                            <td class="customfield_10808"></td>
                                            <td class="customfield_10809">            Bernie Yip
    </td>
                                            <td class="customfield_10000"><div class="shorten" id="customfield_10000-field">
    </div>
</td>
                                            <td class="customfield_10001">    <div class="sd-customer-request-type-customfield-root" data-value="pros/6de43487-f344-457e-93b2-0bd39df879ed" "Customer Request Type" "com.atlassian.servicedesk.internal.customfields.origin.VpOriginCFType@7700e100" data-payload="{&quot;rtName&quot;:&quot;Get IT Help&quot;,&quot;rtIconId&quot;:10530}" data-is-column-view="true">
                <span style="white-space: nowrap;">
                                            <img aria-hidden="true"
                             style="width: 24px;height: 24px;vertical-align: middle;padding: 5px;box-sizing: border-box;"
                             src="/secure/viewavatar?avatarType=SD_REQTYPE&amp;avatarId=10530" />
                                        Get IT Help
        </span>
    </div>
</td>
                                            <td class="customfield_10002"><div class="shorten" id="customfield_10002-field">
    </div>
</td>
                                            <td class="customfield_10910">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11113" customFieldId="10910"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10911">


</td>
                                            <td class="customfield_10912">


</td>
                                            <td class="customfield_10913">


</td>
                                            <td class="customfield_10914">


</td>
                                            <td class="customfield_10915">


</td>
                                            <td class="customfield_10916">


</td>
                                            <td class="customfield_10917">


</td>
                                            <td class="customfield_10918">


</td>
                                            <td class="customfield_10919">


</td>
                                            <td class="customfield_11200"></td>
                                            <td class="customfield_11201"></td>
                                            <td class="customfield_10104"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1079&quot;}">
            
    </div></td>
                                            <td class="customfield_10105"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1079&quot;}">
            
    </div></td>
                                            <td class="customfield_10900"></td>
                                            <td class="customfield_10902">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11105" customFieldId="10902"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10903">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11106" customFieldId="10903"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10904">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11107" customFieldId="10904"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10905">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11108" customFieldId="10905"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10906">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11109" customFieldId="10906"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10907">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11110" customFieldId="10907"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10908">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11111" customFieldId="10908"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10909">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11112" customFieldId="10909"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10101"><div class="sd-request-feedback-customfield-root" data-payload="{&quot;canView&quot;:true}">
    <div style="white-space: nowrap;">
                    </div>
</div></td>
                                            <td class="customfield_10103"></td>
                                            <td class="customfield_10330"></td>
                                            <td class="customfield_10331"></td>
                                            <td class="customfield_11300">            pro.it_admin1
    </td>
                                            <td class="customfield_10332"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1079&quot;}">
            
    </div></td>
                                            <td class="customfield_10333"><div class="sd-sla-field-customfield-root" data-payload="{&quot;isAgent&quot;:true,&quot;issueKey&quot;:&quot;ITJR-1079&quot;}">
            
    </div></td>
                                            <td class="customfield_10324"></td>
                                            <td class="customfield_10325"></td>
                                            <td class="customfield_10326"></td>
                                            <td class="customfield_10205">      0|i00amn:
  </td>
                                            <td class="customfield_10206">    <div class='dev-status-column-view-wrapper'></div>
</td>
                                            <td class="customfield_10327">            Alfred Chan
    </td>
                                            <td class="customfield_10328">            pro.dep_head1
    </td>
                                            <td class="customfield_10329"></td>
                                            <td class="customfield_10320"></td>
                                            <td class="customfield_10321"></td>
                                            <td class="customfield_10200"></td>
                                            <td class="customfield_10322"></td>
                                            <td class="customfield_10201"></td>
                                            <td class="customfield_10323">    New
</td>
                                            <td class="customfield_10313"></td>
                                            <td class="customfield_10314"></td>
                                            <td class="customfield_10315"></td>
                                            <td class="customfield_10316">            pro.it_manager1
    </td>
                                            <td class="customfield_10317"></td>
                                            <td class="customfield_10318"></td>
                                            <td class="customfield_11406"></td>
                                            <td class="customfield_10319"></td>
                                            <td class="customfield_11080"></td>
                                            <td class="customfield_11081"></td>
                                            <td class="customfield_11082"></td>
                                            <td class="customfield_11083"></td>
                                            <td class="customfield_11084"></td>
                                            <td class="customfield_11085"></td>
                                            <td class="customfield_11086">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11286" customFieldId="11086"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11087">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11287" customFieldId="11087"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10310"></td>
                                            <td class="customfield_10311"></td>
                                            <td class="customfield_10312"></td>
                                            <td class="customfield_10302"></td>
                                            <td class="customfield_10303"></td>
                                            <td class="customfield_10304"></td>
                                            <td class="customfield_10305"></td>
                                            <td class="customfield_10306"></td>
                                            <td class="customfield_10307"></td>
                                            <td class="customfield_10308">            pro.it_head1
    </td>
                                            <td class="customfield_10309"></td>
                                            <td class="customfield_11070"></td>
                                            <td class="customfield_11071"></td>
                                            <td class="customfield_11072"></td>
                                            <td class="customfield_11073"></td>
                                            <td class="customfield_11074"></td>
                                            <td class="customfield_11075"></td>
                                            <td class="customfield_11076">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11276" customFieldId="11076"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11077">
<div>
    <div class="jsd-bundled-fields-view" issueId="12768" contextId="11277" customFieldId="11077"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11078"></td>
                                            <td class="customfield_11079"></td>
                                            <td class="customfield_10300">    Not Yet
</td>
                                            <td class="customfield_10301">    Not Confirmed
</td>
                                            <td class="customfield_11060"></td>
                                            <td class="customfield_11061"></td>
                                            <td class="customfield_11062"></td>
                                            <td class="customfield_11063"></td>
                                            <td class="customfield_11064"></td>
                                            <td class="customfield_11065"></td>
                                            <td class="customfield_11066"></td>
                                            <td class="customfield_11067"></td>
                                            <td class="customfield_11068"></td>
                                            <td class="customfield_11069"></td>
                                            <td class="customfield_10401"></td>
                                            <td class="customfield_10404">            pro.it_developer1
    </td>
                                            <td class="customfield_11050"></td>
                                            <td class="customfield_11051"></td>
                                            <td class="customfield_11052"></td>
                                            <td class="customfield_11053"></td>
                                            <td class="customfield_11054"></td>
                                            <td class="customfield_11055"></td>
                                            <td class="customfield_11056"></td>
                                            <td class="customfield_11057"></td>
                                            <td class="customfield_11058"></td>
                                            <td class="customfield_11059"></td>
                                            <td class="customfield_10511"></td>
                                            <td class="customfield_10996"></td>
                                            <td class="customfield_10512"></td>
                                            <td class="customfield_10513"></td>
                                            <td class="customfield_10514"></td>
                                            <td class="customfield_10515"></td>
                                            <td class="customfield_10516"></td>
                                            <td class="customfield_10518"></td>
                                            <td class="customfield_10203"></td>
                                            <td class="customfield_10204"></td>
                                            <td class="customfield_10207"></td>
                                            <td class="customfield_10202"></td>
                                            <td class="customfield_11403"></td>
                                            <td class="customfield_11402"></td>
                                            <td class="customfield_11405"></td>
                                            <td class="customfield_11404"></td>
                                            <td class="customfield_11401"></td>
                                            <td class="customfield_11400"></td>
                                            <td class="customfield_10403"></td>
                    </tr>


                <tr id="issuerow12767" rel="12767" data-issuekey="ITJR-1078" class="issuerow">
                                            <td class="project">    Information Technology Dept
</td>
                                            <td class="issuekey">

    <a class="issue-link" data-issue-key="ITJR-1078" href="http://10.9.17.104:8080/browse/ITJR-1078">ITJR-1078</a>
</td>
                                            <td class="summary"><p>
                0
    </p>
</td>
                                            <td class="issuetype">    Purchase Equipment
</td>
                                            <td class="status">
                <span class=" jira-issue-status-lozenge aui-lozenge jira-issue-status-lozenge-green jira-issue-status-lozenge-done aui-lozenge-subtle jira-issue-status-lozenge-max-width-medium" data-tooltip="&lt;span class=&quot;jira-issue-status-tooltip-title&quot;&gt;Done&lt;/span&gt;&lt;br&gt;&lt;span class=&quot;jira-issue-status-tooltip-desc&quot;&gt;This was auto-generated by Jira Service Desk during workflow import&lt;/span&gt;">Done</span>    </td>
                                            <td class="priority">           Medium
    </td>
                                            <td class="resolution"></td>
                                            <td class="assignee">            pro.digital_marketing_team
    </td>
                                            <td class="reporter">            pro.digital_marketing_team
    </td>
                                            <td class="creator">            pro.digital_marketing_team
    </td>
                                            <td class="created"> 04/Jun/2020 1:40 PM </td>
                                            <td class="lastViewed"> &nbsp; </td>
                                            <td class="updated"> 04/Jun/2020 2:11 PM </td>
                                            <td class="resolutiondate"> 04/Jun/2020 2:11 PM </td>
                                            <td class="versions">    &nbsp;
</td>
                                            <td class="fixVersions">    &nbsp;
</td>
                                            <td class="components"></td>
                                            <td class="duedate">    &nbsp;
</td>
                                            <td class="thumbnail"></td>
                                            <td class="timeoriginalestimate"></td>
                                            <td class="timeestimate"></td>
                                            <td class="timespent"></td>
                                            <td class="workratio">&nbsp;
</td>
                                            <td class="subtasks">                </td>
                                            <td class="issuelinks">                </td>
                                            <td class="environment"></td>
                                            <td class="description"></td>
                                            <td class="security"></td>
                                            <td class="progress">     
</td>
                                            <td class="aggregateprogress">     
</td>
                                            <td class="aggregatetimespent"></td>
                                            <td class="aggregatetimeestimate"></td>
                                            <td class="aggregatetimeoriginalestimate"></td>
                                            <td class="labels"></td>
                                            <td class="customfield_11040"></td>
                                            <td class="customfield_11041"></td>
                                            <td class="customfield_11042"></td>
                                            <td class="customfield_11043"></td>
                                            <td class="customfield_11044"></td>
                                            <td class="customfield_10990"></td>
                                            <td class="customfield_11045"></td>
                                            <td class="customfield_11046"></td>
                                            <td class="customfield_11047"></td>
                                            <td class="customfield_10992"></td>
                                            <td class="customfield_11048"></td>
                                            <td class="customfield_11049"></td>
                                            <td class="customfield_10994"></td>
                                            <td class="customfield_10510"></td>
                                            <td class="customfield_11039"></td>
                                            <td class="customfield_10984"></td>
                                            <td class="customfield_10500"></td>
                                            <td class="customfield_10985"></td>
                                            <td class="customfield_10501"></td>
                                            <td class="customfield_10502"></td>
                                            <td class="customfield_10986"></td>
                                            <td class="customfield_10503"></td>
                                            <td class="customfield_10504"></td>
                                            <td class="customfield_10988"></td>
                                            <td class="customfield_10505"></td>
                                            <td class="customfield_10506"></td>
                                            <td class="customfield_10507"></td>
                                            <td class="customfield_10508"></td>
                                            <td class="customfield_10509"></td>
                                            <td class="customfield_11030"></td>
                                            <td class="customfield_11031"></td>
                                            <td class="customfield_11032"></td>
                                            <td class="customfield_11033"></td>
                                            <td class="customfield_11034"></td>
                                            <td class="customfield_10980"></td>
                                            <td class="customfield_11035"></td>
                                            <td class="customfield_11036"></td>
                                            <td class="customfield_11037"></td>
                                            <td class="customfield_11038"></td>
                                            <td class="customfield_11028"></td>
                                            <td class="customfield_10973"></td>
                                            <td class="customfield_11029"></td>
                                            <td class="customfield_10974"></td>
                                            <td class="customfield_10978"></td>
                                            <td class="customfield_10979"></td>
                                            <td class="customfield_11020"></td>
                                            <td class="customfield_11021"></td>
                                            <td class="customfield_11022"></td>
                                            <td class="customfield_11023"></td>
                                            <td class="customfield_11024"></td>
                                            <td class="customfield_11025"></td>
                                            <td class="customfield_10970"></td>
                                            <td class="customfield_11026">
<div>
    <div class="jsd-bundled-fields-view" issueId="12767" contextId="11226" customFieldId="11026"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_10971"></td>
                                            <td class="customfield_10972"></td>
                                            <td class="customfield_11027">
<div>
    <div class="jsd-bundled-fields-view" issueId="12767" contextId="11227" customFieldId="11027"></div>
    <div class="jsd-bundled-fields-static-table">
        
    </div>
</div>
</td>
                                            <td class="customfield_11017"></td>
                                            <td class="customfield_10962">


</td>
                                            <td class="customfield_11018"></td>
                                            <td class="customfield_10600"></td>
                                            <td class="customfield_10963">


</td>
                                            <td class="customfield_11019"></td>
                                            <td class="customfield_10964">


</td>
                                            <td class="customfield_10602">


</td>
                                            <td class="customfield_10965"></td>
                                            <td class="customfield_10603"></td>
                                            <td class="customfield_10969"></td>
                                            <td class="customfield_11010"></td>
                                            <td class="customfield_11011"></td>
                                            <td class="customfield_11012"></td>
                                            <td class="customfield_11013"></td>
                                            <td class="customfield_11014"></td>
                                            <td class="customfield_11015"></td>
                                            <td class="customfield_10960">


