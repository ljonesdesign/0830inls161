# Naming Conventions Notes

Did anyone notice that there is a slight difference in the naming conventions for the tasks and website repositories? Look how using a monospace font and strict alignment reveals the lack of consistency: the inls-161 with the added hypen goes out one character so that the last 1 in 161 does not line up with the last 1 in the 161 just above. This is one reason it is helpful to use monospace fonts in code editors.
```
          |     |
2017-fall-inls161-website  
2017-fall-inls-161-tasks
          |      |
```
This is an unintentional “bug.” It might not be an issue, but there is a chance it might cause a problem. For example, later, when you "build" your site with the console, you will have to "reference" your repository. If your reference is not EXACTLY the same, your "build" will fail. So, since I have already "built" my example site as inls161, without the hyphen, lets make that the naming convention for the tasks repository, just so we can keep things tidy.

Change your tasks repository from
```
2017-fall-inls-161-tasks
```
to
```
2017-fall-inls161-tasks
```
Now we have better consistency up to the point where it is more logical to make a change:
```
          |     |
2017-fall-inls161-website  
2017-fall-inls161-tasks
          |     |
```
This is relevant to database table design as well. Take a look at these field names:
```
tblPublisher_ID
tblPublisher_Name
tblPublisher_City
tblPublisher_State
Tbl-publisher_Zip Code
```
See how all of them are nice and tidy from left to right in all aspects until there needs to be a difference? Well, all except the last line.

How many bugs are in that field name? (Don't answer too quickly!) The answer is on the database table task page.

If you are curious, here is more info on this naming convention, but it's fine to skip for now. We will cover it in the Database section.

While we are on the topic of naming conventions, I will also want you to follow specific naming conventions with your document, spreadsheet, access, and powerpoint files. For example:
```
lastname-firstname-task03-FINAL.docx    #Word document       
lastname-firstname-task04-DRAFT*.xlsx   #Excel document   
lastname-firstname-task05-FINAL.accdb   #Access document
lastname-firstname-task06-FINAL.pptx    #Powerpoint document

Use DRAFT if you need me to look an issue before due date
```
I will know that it is your word document in your repository. But If you name it after your subject, like
```
my-the-brothers-karamazov-ebook.docx    #Not a good choice; it has 96 chapters
```
and everyone else does the same, then when I pull them all down to my computer to grade, I will have 32 different book titles in a folder on my desktop and I have no idea which one belongs to each one of you.
