# Guide to using LUA to Access Codex Model Members

## Shared Members

These members are shared by all elements that are accessable using LUA.

**Properties**

- Name: ```local elementName = element.Name;```
- Parent: ```local parent = element.Parent```
- ReferenceString: ```local ref = element.ReferenceString;```
- Style: 
  - ```element.Style.ForegroundColor = color.blue;```
  - ```element.Style.MarginLeft = 0.5;```
  - ```element.Style.Bold = true;```

## Button

**Properties**

- AlternateText: 
  - ```local altText = myButton.AlternateText;```
  - ```myButton.AlternateText = "This is a button.";```
- ImageSource
  - ```local image = myButton.ImageSource;```
  - ```myButton.ImageSource = "images\image1.png";```
- Text
  - ```local butText = myButton.Text;```
  - ```myButton.Text = "Button";```

**Methods**

- Click: ```myButton.Click();```

**Events**

- OnAlternateTextChanged
- OnClick: ```myButton.OnClick = "myButton.Text = string.format("Updated...");```
- OnImageSourceChanged
- OnTextChanged

##Document

**Properties**

- Title: 
  - ```myDocument.Title = "This is the name of the docuent";```
  - ```local docTitle = myDocument.Title;```

##Footer

**Properties**

- Level: ```local footLevel = myFooter.Level;```
- Title: 
  - ```theFooter.Title = "This is the footer";```
  - ```local footTitle = theFooter.Title;```

##Header

**Properties**

- Level: ```local headLevel = myHeader.Level;```
- Title: 
  - ```theHeader.Title = "This is the header";```
  - ```local headTitle = theHeader.Title;```

**Fields**

- References: ```local refs = theHeader.References;```

##Image

**Properties**

- AlternateText: 
  - ```local altText = myImage.AlternateText;```
  - ```myImage.AlternateText = "This is an image.";```
- ImageSource
  - ```local image = myImage.ImageSource;```
  - ```myImage.ImageSource = "images\image1.png";```

**Methods**

- Tap: ```myImage.Tap();```

**Events**

- OnAlternateTextChanged
- OnImageSourceChanged
- OnTap

##Page

