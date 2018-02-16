# jekyll2dayone

bash script for converting Jekyll entries to Day One entries

I cobbled this together through copying the bash yaml parser from [jasperes](https://github.com/jasperes/bash-yaml).

You'll want to customize it to fit your needs.

Line 49 indicates where you want the script to look for your Jekyll files

Line 58 determines how many lines of YAML should be ignored when the entry is written to Day One. Just adjust the "+5" to whatever you need (basically, +5 ignores the first 5 (or 6? I'm not sure if it starts from 0) lines).

Line 60 determines the options for writing to Day One. You can delete the --journal flag or change "Work" to match your journal. If your jekyll entries don't have a "title" in the YAML field, or you don't want it written into the Day One entries, then delete "$title". Same with the date flag. Same with the tags flag. 

I really don't know much of anything about bash scripting. I got this to work for my needs, but if it doesn't work for you, I'm not sure I'll be too useful.
