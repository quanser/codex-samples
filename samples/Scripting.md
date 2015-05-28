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

- AlternateText
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

- Title
  - ```myDocument.Title = "This is the name of the docuent";```
  - ```local docTitle = myDocument.Title;```

##Footer

**Properties**

- Level: ```local footLevel = theFooter.Level;```
- Title
  - ```theFooter.Title = "This is the footer";```
  - ```local footTitle = theFooter.Title;```

##Header

**Properties**

- Level: ```local headLevel = theHeader.Level;```
- Title
  - ```theHeader.Title = "This is the header";```
  - ```local headTitle = theHeader.Title;```

**Fields**

- References: ```local refs = theHeader.References;```

##Image

**Properties**

- AlternateText
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

Shares Properties with all elements

##Section

**Properties**

- Level: ```local secLevel = theSection.Level;```
- Title
  - ```theSection.Title = "This is a section";```
  - ```local secTitle = theSection.Title;```

##Slider

**Properties**

- InitialValue
  - ```mySlider.InitialValue = 5;```
  - ```local initVal = mySlider.InitialValue;```
- MaxValue
  - ```mySlider.MaxValue = 10;```
  - ```local maxVal = mySlider.MaxValue;```
- MinValue
  - ```mySlider.MinValue = 0;```
  - ```local minVal = mySlider.MinValue;```
- Value
  - ```mySlider.Value = 3;```
  - ```local slideVal = mySlider.Value;```

**Fields**

- DefaultMaxValue: ```local defaultMax = mySlider.DefaultMaxValue;```
- DefaultMinValue: ```local defaultMin = mySlider.DefaultMinValue;```
- DefaultValue: ```local defaultVal = mySlider.DefaultValue;```

**Events**

- OnMaxValueChanged
- OnMinValueChanged
- OnValueChanged

##Stack Layout

**Properties**

- Orientation
  - ```myStack.Orientation = "horizontal"```;
  - ```local stackOrient = myStack.Orientation;```

**Events**

- OnOrientationChanged

##Switch

**Properties**

- InitialValue
  - ```mySwitch.InitialValue = true;```
  - ```local initVal = mySwitch.InitialValue;```
- Value
  - ```mySwitch.Value = false;```
  - ```local switchVal = mySwitch.Value;```
  
**Fields**

- DefaultValue: ```local defaultVal = mySwitch.DefaultValue;```

**Events**

- OnValueChanged

##Table

**Properties**

- ColumnWidths
  - ```myTable.ColumnWidths = 0.5;```
  - ```local colWidth = myTable.ColumnWidths;```
- GridLines
  - ```myTable.GridLines = true;```
  - ```local gridLines = myTable.GridLines;```
- HasHeaderRow: ```local myTable.HasHeaderRow;```

##TableData

**Properties**

- ColumnSpan
  - ```myTable.ColumnSpan = 2;```
  - ```local colSpan = myTable.ColumnSpan;```
- RowSpan
  - ```myTable.RowSpan = 3;```
  - ```local rowSpan = myTable.RowSpan;```
