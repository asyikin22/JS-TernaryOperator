This script creates a simple website with a dropdown menu that enables you to change the background color and text color of the entire web page.                                                          

	1. Initializing Variables:
		○ Select the dropdown menu element with ID "color" using document.querySelector("select");
		○ Select the html element which represents the whole HTML document using 
		document.querySelector("html");
		
	2. Define a function named update for background color and text color:
		○ The function takes two arguments, bgColor and textColor
		○ Update the background color of entire HTML using bgColor
		html.style.backgroundColor = bgColor;
		○ Update the text color  of entire HTML using textColor
		html.style.color = textColor;
		
	3. Attach Event Listener
		○ This attaches event listener to dropdown menu that triggers every time the selection changes: select.addEventListener ("change", () => ... );
			§ Checks if the selected value is blue: 
			select.value === "blue"
			§ If condition is true, it calls the update function with arguments "blue" for background color and "yellow" for text
			? update ("blue", "yellow")
			§ If condition is false, it calls the update function with argument "yellow" and "blue" respectively. 
			: update ("yellow", "blue")
