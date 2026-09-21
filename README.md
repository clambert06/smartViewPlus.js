# smartViewPlus.js
WARNING: NOT FOR PROFESSIONAL USE

Section 1 - Command Description
smartViewPlus.js is a custom Node.js command-line tool that extends basic file-viewing functionality. It reads a text file, displays the first 10 lines, the last 10 lines, searches for a keyword, counts matches, and writes all results to a log file. The tool combines the behavior of commands like cat, head, tail, and grep into a single "fancy" command.

How to Run It
From the terminal:
node smartViewPlus.js <filename> <keyword>
Example: node smartViewPlus.js sample.txt error

What the Tool Does
  Reads the specified file
  Prints the first 10 lines
  Prints the last 10 lines
  Searches for lines containing the keyword
  Displays all matching lines
  Shows the total match count
  Creates a log file (smartview.log) with all results

This combines the functionality of:
  head - first 10 lines
  tail - last 10 lines
  grep - keyword search
  cat - file viewing
  All inside one Node.js script.

Section 2 - AI-Assisted Programming
I used AI to help me understand how to structure the command, how to read files in Node.js, and how to slice and filter arrays to get the first and last 10 lines and keyword matches. I asked AI questions about debugging, especially when my script wasn’t printing anything, and it helped me realize the issue was with my test file rather than the code itself. AI also helped identify important edge cases, like what should happen when the keyword doesn’t appear at all or when the file has fewer than 10 lines.

Even though AI helped with explanations and troubleshooting, I still had to think independently about how to integrate each feature into one tool, how to test different scenarios, and how to update my code based on the assignment requirements. I also had to make decisions about how to format the output and how to structure the log file. AI didn’t always know what was wrong at first - for example, it assumed my code was broken when the real issue was that my sample.txt file was empty - so I had to verify the behavior myself and adjust my testing approach.

Section 3 - Testing Reflection
During testing, I discovered that some outputs weren’t appearing, which made me think the logic was broken. The real issue was that my test file didn’t have enough lines, and in one case it was completely empty, so the first and last 10 lines and keyword matches didn’t show anything. After adding more realistic content to sample.txt, both test scenarios worked correctly, including the case where the keyword wasn’t found and the match count was 0. AI helped me identify missing edge cases, confirm that the script logic was correct, and understand that the problem was with my test data rather than the code.
