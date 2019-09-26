# Print-ticket-as-page
 
This change brings back the feature to print an single ticket as a Word document.
A Print button on the view ticket page will be visible. 

![Example](/example.png)

Tested against Mantisbt 2.21

1) in your main mantis config dir create a new file named 'custom_strings_inc.php' and add following lines to it
'''
<?php
switch( $g_active_language ) {
	default:
	# Default language, as defined in config/config_inc.php
	# ($g_default_language, English in this case)
	# Mantis grafieken

    $s_print_bug_page = 'Print Ticket';

	break;
}
'''

2) implement the code