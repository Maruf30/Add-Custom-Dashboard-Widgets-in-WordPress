# Add-Custom-Dashboard-Widgets-in-WordPress




function my_custom_dashboard_widgets() {
global $wp_meta_boxes;
 
wp_add_dashboard_widget('custom_help_widget', 'Theme Support', 'custom_dashboard_help');
}
 
function custom_dashboard_help() {
echo '<p>Here write custom widget data which show on widget if use the custom widget.</p>';
}
add_action('wp_dashboard_setup', 'my_custom_dashboard_widgets');
