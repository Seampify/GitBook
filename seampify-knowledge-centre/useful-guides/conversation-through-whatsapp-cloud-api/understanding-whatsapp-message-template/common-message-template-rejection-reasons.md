---
icon: message-exclamation
---

# Common Message Template Rejection Reasons

## Common Rejection Reasons <a href="#common-rejection-reasons" id="common-rejection-reasons"></a>

Submissions are commonly rejected for the following reasons, so make sure you avoid these mistakes.

* Variable parameters are missing or have mismatched curly braces. The correct format is `{{1}}`.
* Variable parameters contain special characters such as a `#`, `$`, or `%`.
* Variable parameters are not sequential. For example, `{{1}}`, `{{2}}`, `{{4}}`, `{{5}}` are defined but `{{3}}` does not exist.
* Template contains too many variable parameters relative to the message length. You need to decrease the number of variable parameters or increase the message length.
* The message template cannot end with a parameter.
* The message template contains content that violates WhatsApp’s Commerce Policy: When you offer goods or services for sale, we consider all messages and media related to your goods or services, including any descriptions, prices, fees, taxes and/or any required legal disclosures, to constitute transactions. Transactions must comply with the [WhatsApp Commerce Policy](https://www.whatsapp.com/legal/commerce-policy/?fbclid=IwZXh0bgNhZW0CMTEAAR3p9bHswvypTJnCKUprFfRUJPt0bIP1GAUWdEhDkaxFZziqtv6tNWkRAuI_aem_TNe3ienZ3WQbncmpN9vf9g).
* The message template contains content that violates the [WhatsApps Business Policy](https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.whatsapp.com%2Flegal%2Fbusiness-policy%2F%3Ffbclid%3DIwZXh0bgNhZW0CMTEAAR1RaauLVyBw-NNjIADM9AbvYltDog0LlFz6zL8e5gXCmIPQdgMXjZ0DF2U_aem_VBj92d3TcaPgmJaWWxNfHw\&h=AT19DwX-0sR3jHXL7ouTkPZ1WJh_HyfBT4INewPHghK8_iGwM7vNHRVegBbLRPYbhuQ0ZPwNJTmOwlnl9tq1ZCGqegmPdFwP6q5i6BTuFrzRSM26YjhjZojV5xbFFc_VhMRQ9Uc6o0274EHwBVb9Ahh7): Do not request sensitive identifiers from users. For example, do not ask people to share full length individual payment card numbers, financial account numbers, National Identification numbers, or other sensitive identifiers. This also includes not requesting documents from users that might contain sensitive identifiers. Requesting partial identifiers (ex: last 4 digits of their Social Security number) is OK.
* The content contains potentially abusive or threatening content, such as threatening a customer with legal action or threatening to publicly shame them.
* The message template is a duplicate of an existing template. If a template is submitted with the same wording in the body and footer of an existing template, the duplicate template will be rejected.
* The message template contains a URL shortener for your links.

A rejection notification that includes the rejection reason will appear in [Business Support Home](https://business.facebook.com/business-support-home). You can view rejections in the **Business Support Home** by navigating to **Account Overview** > **View my accounts** (button) > (your Meta Business Account) > (your WABA) > **Rejected message templates**. Rejection info will also be sent via email.

You can refer to the **Business Support Home** notification to see the name and language of the existing template with the same content as the rejected duplicate template. You may also choose to edit the template and resubmit.

This check does not apply to templates categorized as [`AUTHENTICATION`](./#types-of-message-template).



## Troubleshooting a rejected message template&#x20;

You can edit a template at the [Manage Templates](../../../seampifys-modules/settings/more-settings/channels/manage-templates/) page. Note that if you edit a message template and resubmit it for approval, its status will be set to **Pending** and it can't be sent to customers until its status has been set to **Approved**.



## Quality Rating <a href="#quality-rating" id="quality-rating"></a>

Every message template has a quality rating based on usage, customer feedback and engagement. A message template's rating will appear in the WhatsApp Manager whenever it has an **Active** status, and will be displayed after a hyphen in the message template's status:

* Active - **Quality pending** (highlighted in green)
* Active - **High quality** (highlighted in green)
* Active - **Medium quality** (highlighted in yellow)
* Active - **Low quality** (highlighted in red)

Approved message templates start out with a **Quality pending** rating. If a message template continuously receives negative feedback or low engagement, it will eventually cause a change in the template status. As long as a message template has an **Active** status, regardless of the quality rating, it can be sent to customers. However, once a message template's status changes to any other status, it cannot be sent to customers until it becomes active again.

<br>
