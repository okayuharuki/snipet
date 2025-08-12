# snipet
スニペット登録一覧

{
	// Place your GLOBAL snippets here. Each snippet is defined under a snippet name and has a scope, prefix, body and 
	// description. Add comma separated ids of the languages where the snippet is applicable in the scope field. If scope 
	// is left empty or omitted, the snippet gets applied to all languages. The prefix is what is 
	// used to trigger the snippet and the body will be expanded and inserted. Possible variables are: 
	// $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. 
	// Placeholders with the same ids are connected.
	// Example:
	// "Print to console": {
	// 	"scope": "javascript,typescript",
	// 	"prefix": "log",
	// 	"body": [
	// 		"console.log('$1');",
	// 		"$2"
	// 	],
	// 	"description": "Log output to console"
	// }
	"Var dump": {
		"prefix": "pp-var_dump",
		"body": [
			"<?php echo '<pre>'; ?>",
			"\t<?php var_dump($1); ?>",
			"<?php echo '</pre>'; ?>"
		],
		"description": "整形したvardump"
	},
	"Loop": {
		"prefix": "pp-loop",
		"body": [
			"<?php if ( have_posts() ) : ?>",
			"\t<?php while ( have_posts() ) : ?>",
			"\t\t<?php the_post(); ?>",
			"\t\t<?php the_content(); ?>",
			"\t<?php endwhile; ?>",
			"<?php endif; ?>"
		]
	},
	"PHP if": {
		"prefix": "pp-if",
		"body": [
			"<?php if ($1) : ?>",
			"${3:<?php elseif ($2) : ?>}",
			"${4:<?php else : ?>}",
			"<?php endif; ?>"
		]
	},
	"PHP": {
		"prefix": "pp",
		"body": [
			"<?php $1 ?>"
		]
	},
	"PHP_fget": {
		"prefix": "pp_fget",
		"body": [
			"$$1 = fget(STDIN);"
		]
	},
	"PHP_img": {
		"prefix": "pp-img",
		"body": [
			"<?php echo get_template_directory_uri(); ?>"
		]
	},
	"Home_Url": {
		"prefix": "pp-home_url",
		"body": [
			"<?php echo esc_url( home_url( '/$1' ) ); ?>"
		]
	},
	"The_Time": {
		"prefix": "pp-the_time",
		"body": [
			"<time class=\"$1\" datetime=\"<?php the_time( 'c' ); ?>\"><?php the_time( 'Y,m,d' ); ?></time>"
		]
	},
	"The_modified_Time": {
		"prefix": "pp-the_modified_time",
		"body": [
			"<?php if (get_the_modified_time('c') !== get_the_time('c')) : ?>",
			"\t<time class=\"$1\" datetime='<?php the_modified_time('c'); ?>'>最終更新日 <?php the_modified_time('Y/n/j'); ?></time>",
			"<?php endif; ?>"
		],
		"description": "最終更新日"
	},
	"The_title": {
		"prefix": "pp-the_title",
		"body": [
			"<?php the_title($1); ?>"
		]
	},
	"The_Content": {
		"prefix": "pp-the_content",
		"body": [
			"<?php the_content($1); ?>"
		]
	},
	"The_Permalink": {
		"prefix": "pp-the_permalink",
		"body": [
			"${1:<?php the_permalink($2); ?>}"
		]
	},
	"The_Excerpt": {
		"prefix": "pp-the_excerpt",
		"body": [
			"<?php the_excerpt($1); ?>"
		],
		"description": "抜粋文"
	},
	"Get_template_Parts": {
		"prefix": "pp-get_template_part",
		"body": [
			"<?php get_template_part( 'template-parts/$1' ); ?>"
		]
	},
	"Get_Header": {
		"prefix": "pp-get_header",
		"body": [
			"<?php get_header($1); ?>"
		]
	},
	"Get_Footer": {
		"prefix": "pp-get_footer",
		"body": [
			"<?php get_footer($1); ?>"
		]
	},
	"Get_Archives": {
		"prefix": "pp-get_archives",
		"body": [
			"<?php wp_get_archives(); ?>"
		],
		"description": "アーカイブを取得"
	},
	"Get_Category": {
		"prefix": "pp-get_category",
		"body": [
			"<?php",
			"\\$category = get_the_category();",
			"if (\\$category[0]): ?>",
			"\t<div class=''>",
			"\t\t<a href='<?php echo get_category_link(\\$category[0]->term_id); ?>'>",
			"\t\t\t<?php echo \\$category[0]->cat_name; ?>",
			"\t\t</a>",
			"\t</div>",
			"<?php endif; ?>"
		]
	},
	"Get_Tag": {
		"prefix": "pp-get_tag",
		"body": [
			"<?php \\$post_tags = get_the_tags(); ?>",
			"<div class=\"$1\">",
			"\t<?php if (\\$post_tags) : ?>",
			"\t\t<?php foreach (\\$post_tags as \\$tag) : ?>",
			"\t\t\t<div class=\"$1\"><a href='<?php echo get_tag_link(\\$tag->term_id); ?>'><?php echo \\$tag->name; ?></a></div><!-- /entry-tag-item -->",
			"\t\t<?php endforeach; ?>",
			"\t<?php endif; ?>",
			"</div>"
		]
	},
	"Get_Template_Directory": {
		"prefix": "pp-get_template_directory",
		"body": [
			"${1:<?php echo esc_url( get_template_directory_uri() ); ?>}"
		]
	},
	"Get_Stylesheet_Directory": {
		"prefix": "pp-get_stylesheet_directory",
		"body": [
			"${1:<?php echo esc_url( get_stylesheet_directory_uri() ); ?>}"
		]
	},
	"has_post_thumbnail": {
		"prefix": "pp-has_post_thumbnail",
		"body": [
			"<?php if(has_post_thumbnail()): ?>",
			"<?php the_post_thumbnail(); ?>",
			"<?php  else: ?>",
			"\t<img src=\"<?php echo get_template_directory_uri(); ?>/img$1\" alt=\"\">",
			"<?php endif; ?>",
		],
		"description": "サムネイル画像を呼び出す"
	},
	"paginate_links": {
		"prefix": "pp-paginate_links",
		"body": [
			"<?php if(paginate_links()) : //ページが1ページ以上あれば以下を表示 ?>",
			"<!-- pagination -->",
			"<div class=\"pagination\">",
			"\t<?php",
			"\techo paginate_links(",
			"\t\tarray(",
			"\t\t'end_size' => 1,",
			"\t\t'mid_size' => 1,",
			"\t\t'prev_next' => true,",
			"\t\t'prev_text' => '<i class=\"fas fa-angle-left\"></i>',",
			"\t\t'next_text' => '<i class=\"fas fa-angle-right\"></i>',",
			"\t\t)",
			"\t);",
			"\t)?>",
			"</div><!-- /pagination -->",
			"<?php endif; ?>",
		],
		"description": "次のページに移動"
	},
	"sub-loop": {
		"prefix": "pp-sub-loop",
		"body": [
			"<?php \\$pickup_query = new WP_Query(",
			"\tarray(",
			"\t\t'post_type' => 'post',",
			"\t\t'tag' => 'pickup',",
			"\t\t'posts_per_page' => 3",
			"\t)",
			");",
			"//pickupタグを用意して呼び出す ?>",
			"<?php if ( \\$news_query->have_posts() ) : ?>",
			"<?php while ( \\$news_query->have_posts() ) : ?>",
			"<?php \\$news_query->the_post(); ?>",
			"\t<p>処理内容</p>",
			"<?php endwhile; ?>",
			"<?php endif; ?>",
			"<?php wp_reset_postdata(); ?>",
		],
		"description": "サブループ"
	},
	"my_setup": {
		"prefix": "pp-script-setup_thumbnails",
		"body": [
			"function my_setup(){",
			"\tadd_theme_support('post-thumbnails');",
			"\tadd_theme_support('automatic-feed-links');",
			"\tadd_theme_support('title-tag');",
			"\tadd_theme_support('html5', array('comment-list', 'comment-form', 'search-form', 'gallery', 'caption', 'style', 'script'));",
			"}",
			"add_action(\"after_setup_theme\", \"my_setup\");",
		],
		"description": "function.phpに記述サムネイルを有効にする(wordpressの機能追加)"
	},
}
