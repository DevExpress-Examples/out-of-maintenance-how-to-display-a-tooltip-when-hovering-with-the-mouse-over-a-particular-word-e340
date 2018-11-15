<!-- default file list -->
*Files to look at*:

* [Form1.cs](./CS/Form1.cs) (VB: [Form1.vb](./VB/Form1.vb))
* [Program.cs](./CS/Program.cs) (VB: [Program.vb](./VB/Program.vb))
<!-- default file list end -->
# How to display a ToolTip when hovering with the mouse over a particular word


<p>Firstly, you should <a href="http://documentation.devexpress.com/#WindowsForms/CustomDocument6012"><u>Obtain the Document Position under the Mouse Cursor</u></a>. Then, utilize the <a href="http://documentation.devexpress.com/#CoreLibraries/DevExpressXtraRichEditAPINativeSubDocument_GetTexttopic754"><u>SubDocument.GetText Method</u></a> to get a text within specified ranges several times until this text represents a whole word. Note also that it is very important to utilize the <a href="http://documentation.devexpress.com/#CoreLibraries/DevExpressXtraRichEditAPINativeDocumentPosition_BeginUpdateDocumenttopic"><u>DocumentPosition.BeginUpdateDocument Method</u></a>. This allows you to distinguish between different parts of the document, such as header, footer or body.<br><br>Starting with version 16.1, the <a href="https://documentation.devexpress.com/#corelibraries/clsDevExpressXtraRichEditHitTestManagertopic">HitTestManager</a> class is provided. Using this class, it's possible to obtain document layout elements located under the specific point and display information about this element in the ToolTip.<br>Refer to the <a href="https://www.devexpress.com/Support/Center/p/T399401">How to show a ToolTip containing information about the document layout element located under the cursor position</a> example illustrating this approach.</p>

<br/>


