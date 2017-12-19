```
function js_async_attr($tag){
 # Add async to all remaining scripts
 return str_replace( ' src', ' async="async" src', $tag );
}
add_filter( 'script_loader_tag', 'js_async_attr', 10 );

define('WP_POST_REVISIONS', false );
