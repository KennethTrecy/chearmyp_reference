# Syntax Overview
There are four general kinds of nodes that exist in Chearmyp. Take note that Chearmyp still have
unstable syntax.

1. *Comment*. These nodes may be used for documentation purposes. It has two subkinds: *line*
	comments and *block* comments.
	- *Line* comment. These are comments that only exist in one line and have a pound sign (`#`)
		prefix.
		```
		# This is a line comment.
		```
	- *Block* comment. These comments may have one or more lines. They have three pound signs (`###`)
		as their prefix and suffix.
		```
		###
		This is a block comment.
		###

		# Below is an indented block comment.
			###
				This is an indented block comment.
		### These pound signs will not terminate the comment.
				### This one too.
			Only the pound signs below will end the block comment.
			###
		```

2. *Edon*. These nodes can be thought of as basic concepts that other concepts can use or
	include. They are the main nodes that may act as instructions, structure, or data.
	```
	language	# This is an example of edon. Use tabs to separate comment.
		number
			0	# An edon can be a number.
			1
			2
			...	# An edon can be punctuations too.
			9
		noun
			common
			proper
				Kenneth Trecy	# An edon may contain spaces too.
		verb
			types
				regular
				irregular
			tenses
				past
				present
				future
		adjective
		punctuations
			.	# An edon can be anything as long as it does not start with a pound sign.
			,
	```

3. *Attacher*. These nodes are pair of concepts may be attached to an *edon*. These
	concepts may be a metadata, adjective, reference, and others. They are written indented below the
	*edon* they are attaching to. These nodes can be used to describe the whole file
	if these are on the root (hence, not attached to any *edon*). *Attachers* must
	have a colon (`:`) and followed tab(s) or spaces(s) between the pairs namely label and content.
	```
	books
		book_a|
			price: $1			# Attaches book a's price.
			title: Title A		# Attaches book a's title.
			author: Author A	# Attaches book a's author.

		book_b|
			price:	$2			# Attaches book b's price.
			title:	Title B	# Attaches book b's title.
			author:	Author B	# Attaches book b's author.

		# Attachers can be written in one line.
		book_c|
			price: $3	title: Title C	author: Author C

		name: Book set A	# Attaches book set's name.
	```

5. *Othertongue*. These nodes contain a different language from the rest of the document. Their
	syntax is  similar to *comments*. Due to the variety of languages, there are concepts also, that
	have no direct translation to the current concept. However, *othertongues* must be contained to a
	*complex*.
	- *Line* othertongue. These othertongues are similar to *line* comments. Their containment must
		be expressed by indention using tab(s) or in one line after the *complex*.
		```
		numbers
			0|
				= zero
			1|
				= one
				= ...

		attacher
			= a pair of concepts that attach to other complex or simplex
		```
	- *Block* othertongue. These othertongues are similar to *block* comments. Instead of pound
		signs, they are identified using three equal signs(`===`).
		```
		languages
			natural
				English
					===
					Good morning!
					===
				Filipino
					===
					Magandang umaga!
					===
				Kapampangan
					===
					Mayap na abak!
					===
			programming
				===
				print "Good morning!"
				===
		```
