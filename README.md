# Head Inserter

* Date:    August 13, 2014
* Author:  Joey Bomber
* Version: 1.0
* License: http://opensource.org/licenses/MIT

Creates a new Hook called head_inserter, when called this hook inserts the given string just above the closing head tag. If </head> is not found, nothing is inserted

## Usage

~~~ php
	function insert($html) {
		return $html . "\t<meta name=\"robots\" content=\"noindex, nofollow\">\n";
	}

	\Sleepy\Hook::applyFilter('head_inserter', 'insert');
~~~