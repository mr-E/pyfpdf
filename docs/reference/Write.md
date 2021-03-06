## Write ##

```python
write(h: float, txt: str, link)
```

### Description ###

This method prints text from the current position. When the right margin is reached (or the \n character is met) a line break occurs and text continues from the left margin. Upon method exit, the current position is left just at the end of the text.
It is possible to put a link on the text.

### Parameters ###

h:
> Line height.

txt:
> String to print.

link:
> URL or identifier returned by [AddLink](AddLink.md).

### Example ###
```python
# Begin with regular font
pdf.set_font('Arial','',14)
pdf.write(5,'Visit ');
# Then put a blue underlined link
pdf.set_text_color(0,0,255);
pdf.set_font('','U');
pdf.write(5,'www.fpdf.org','http://www.fpdf.org');
```

### See also ###

[SetFont](SetFont.md), [SetTextColor](SetTextColor.md), [AddLink](AddLink.md), [MultiCell](MultiCell.md), [SetAutoPageBreak](SetAutoPageBreak.md), [WriteHTML](WriteHTML.md)
