# Data Dictionary

## Purpose

This data dictionary defines the fields used in the synthetic customer complaint dataset. It provides a consistent interpretation of each field for analysis and reporting.

| Field Name            | Data Type | Description                                                                                  | Example        |
| --------------------- | --------- | -------------------------------------------------------------------------------------------- | -------------- |
| Complaint_ID          | Text      | Unique identifier assigned to each complaint record.                                         | C001           |
| Complaint_Date        | Date      | Date on which the customer complaint was recorded.                                           | 2026-01-05     |
| Category              | Text      | Main category assigned to the customer complaint.                                            | Delivery       |
| Channel               | Text      | Communication channel through which the complaint was received.                              | Email          |
| Priority              | Text      | Business priority assigned to the complaint based on urgency or impact.                      | High           |
| Resolution_Time_Hours | Numeric   | Number of hours required to resolve the complaint.                                           | 48             |
| Repeat_Contact        | Text      | Indicates whether the customer contacted the company more than once regarding the complaint. | Yes            |
| Resolution_Status     | Text      | Current resolution status of the complaint.                                                  | Resolved       |
| Root_Cause            | Text      | Primary suspected operational cause associated with the complaint.                           | Delivery Delay |

## Field Interpretation

### Complaint_ID

A unique identifier used to distinguish individual complaint records.

### Complaint_Date

The date the complaint was recorded. This field can be used for monthly or time-based trend analysis.

### Category

The broad business area associated with the complaint. Categories in this dataset include Delivery, Billing, Product Quality, Refund, and Account.

### Channel

The communication method used by the customer. Channels include Email, Phone, Web, and Chat.

### Priority

Indicates the relative urgency of the complaint:

* **High** — requires greater attention due to potential customer or operational impact.
* **Medium** — requires standard follow-up.
* **Low** — generally lower urgency.

### Resolution_Time_Hours

Measures the elapsed time required to resolve the complaint. This can be used to calculate average resolution time and compare performance across complaint categories.

### Repeat_Contact

Indicates whether the customer contacted the company more than once about the complaint:

* **Yes** — repeat contact occurred.
* **No** — no repeat contact was recorded.

### Resolution_Status

Indicates the current status of the complaint. The current synthetic dataset contains resolved complaints.

### Root_Cause

Represents the primary suspected cause associated with the complaint. Examples include Delivery Delay, Incorrect Invoice, Product Defect, Refund Processing Delay, and Account Information Issue.

## Data Quality Notes

* The dataset is synthetic and created solely for portfolio purposes.
* Complaint IDs are unique within this dataset.
* Dates use the `YYYY-MM-DD` format.
* Resolution time is measured in hours.
* Categorical values use consistent labels to support grouping and analysis.
* The dataset should not be interpreted as actual company or customer data.
