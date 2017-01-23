<body ondragover="return false" class="light_theme"><div id="coachmark_bg" class="hidden"></div>

<div id="drop-zone">
	<div class="instructions">
		<div class="instructions_icons"></div>
		<h1>Drop to upload to Slack</h1>
		
		<p class="drop_tip">Hold down <span class="keyboard">Shift</span> while dropping to upload immediately.</p>
		<p class="drop_tip">For more shortcuts and keyboard commands, press <span id="drag_drop_mac_key" class="keyboard">Control</span><span class="keyboard">?</span></p>
			</div>
</div>


<script type="text/javascript">

setTimeout(function() {
	if (document.getElementById('self_help_link_div')) {
		document.getElementById('self_help_link_div').style.opacity = 1;
	}
}, 30000);
// Only log 10% of all events
if (window.TSMeasureAndBeacon) {
	window.TSMeasureAndBeacon('loading_screen_rendered', 'start_nav');
}

</script>

<div id="client-ui" class="container-fluid flexbox_client feature_shrinkwrap_menus flexpane_redesign sidebar_theme_default whats_new_showing flex_pane_showing">

	
<div id="banner" class="hidden">

	<div id="notifications_banner" class="banner mustard_yellow_bg hidden">
		Slack needs your permission to <a>enable desktop notifications</a>.		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss"></a>
	</div>

	<div id="notifications_dismiss_banner" class="banner seafoam_green_bg hidden">
		We strongly recommend enabling desktop notifications if you’ll be using Slack on this computer.		<span class="inline_block no_wrap">
			<a onclick="TS.ui.banner.close(); TS.ui.banner.growlsPermissionPrompt();">Enable notifications</a> •
			<a onclick="TS.ui.banner.close()">Ask me next time</a> •
			<a onclick="TS.ui.banner.closeNagAndSetCookie()">Never ask again on this computer</a>
		</span>
	</div>

	<div id="macssb1_banner" class="banner blue_fill_bg hidden">
		<a class="apps_page_link" href="/downloads" target="_new" onclick="TS.ui.banner.onClickedMacSSB1Link(this, true)">Download the Slack Mac app</a> for greater control over your notifications. Easier if you’re on multiple teams,&nbsp;too!		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss"></a>
	</div>

	<div id="macssb1_dismiss_banner" class="banner blue_fill_bg hidden">
					Are you sure? You can install it from the <a href="" target="_new" onclick="TS.ui.banner.onClickedMacSSB1Link(this)">Mac App Store</a> or&nbsp;by&nbsp;<a href="/ssb/download-osx" target="_new" onclick="TS.ui.banner.onClickedMacSSB1Link(this)">direct&nbsp;download</a>.				<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" onclick="TS.ui.banner.onClickedMacSSB1Link(this, true)" aria-label="Dismiss"></a>
	</div>

	<div id="macssb2_banner" class="banner blue_fill_bg hidden">
		A shiny new version of Slack is available! <a class="apps_page_link" href="/downloads" target="_new" onclick="TS.ui.banner.onClickedMacSSB2Link(true)">Upgrade now</a>		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss"></a>
	</div>

	<div id="winssb1_banner" class="banner blue_fill_bg hidden">
		<a class="apps_page_link" href="/downloads" target="_new" onclick="TS.ui.banner.onClickedWinSSB1Link(this, true)">Download the Slack Windows app</a> for greater control over your notifications. Easier if you’re on multiple teams, too!		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss"></a>
	</div>

	<div id="winssb1_dismiss_banner" class="banner blue_fill_bg hidden">
		Are you sure? You can <a href="https://slack.com/ssb/download-win" target="_new" onclick="TS.ui.banner.onClickedWinSSB1Link(this)">download</a> it now.		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" onclick="TS.ui.banner.onClickedWinSSB1Link(this, true)" aria-label="Dismiss"></a>
	</div>

	<div id="macssb_osx_deprecated_banner" class="banner mustard_yellow_bg hidden">
		Your version of OS X won’t be supported for much longer. <a target="_blank" href="https://get.slack.help/hc/articles/207677868">Learn more</a> to keep using Slack.		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss"></a>
	</div>

	
	<div id="macelectron1_banner" class="banner seafoam_green_bg hidden">
		<img class="banner_emoji" src="https://cdx.slack-edge.com/f5d6f/img/emoji_2016_06_08/apple/1f44b.png" alt="">
		We have a new Mac app! It’s faster than ever, with built-in notifications so you never miss a beat. <a class="mac_downloads_page_link" href="/downloads/osx" target="_new" onclick="TS.ui.banner.onClickedMacElectronLink(this, true)">Download now</a>		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss" onclick="TS.ui.banner.onDismissedMacElectronLink(this)"></a>
	</div>

	<div id="macelectron2_banner" class="banner seafoam_green_bg hidden">
		<img class="banner_emoji very_small_right_margin" src="https://cdx.slack-edge.com/66f9/img/emoji/1f68c.png" alt="">
		Beep! Our new Mac app has a fresh coat of paint and runs faster than ever. <a class="update_link" href="/downloads/osx" onclick="TS.ui.banner.onClickedMacElectronLink(this, true)">Download now</a> to get the latest.		<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss" onclick="TS.ui.banner.onDismissedMacElectronLink(this)"></a>
	</div>

			<div id="allow_popups_banner" class="banner mustard_yellow_bg hidden">
			Please allow pop-ups in <span id="allow_popups_banner_browser">your browser</span>. You can <a href="http://my.slack.com/help/requests/new">contact Slack</a> if you need help.			<a class="banner_dismiss ts_icon ts_icon_times_circle" data-action="dismiss_banner" aria-label="Dismiss"></a>
		</div>
	
</div>
			<div class="client_container">
			
<div class="client_channels_list_container">
	<div id="col_channels_bg" style="z-index: 0;"></div>
	<div id="col_channels_overlay" class="onboarding_overlay hidden">
		<div class="overlay_mock_text forty_percent_width"></div>
		<div class="overlay_mock_text fifty_percent_width"></div>
		<div class="overlay_mock_text thirty_five_percent_width"></div>
	</div>

	
<div id="team_menu" data-qa="team_menu_selector" class="">
	<div class="placeholder_shimmer_clipper">
	<div class="placeholder_shimmer_bg_wrapper">
		<div class="placeholder_shimmer_bg"></div>
	</div>
</div>	<button class="notifications_menu_btn ts_icon ts_tip ts_tip_bottom ts_tip_float btn_unstyle ts_icon_snooze_outline" aria-label="Notifications Menu">
		<span class="notifications_menu_tip ts_tip_tip">Notifications</span>
	</button>
	<div class="team_name_container top_margin">
		<button class="ts_icon ts_icon_chevron_down team_name_caret btn_unstyle" aria-label="Team Menu" aria-haspopup="true"></button>
		<span id="team_name" class="overflow_ellipsis">MIC</span>
	</div>
	<div id="team_menu_overlay" class="onboarding_overlay hidden">
		<div class="overlay_mock_text seventy_percent_width"></div>
	</div>
	<div id="team_menu_user">
		<div id="presence_container" class="no_wrap ts_tip ts_tip_bottom ts_tip_left">
			<i id="presence" class="ts_icon ts_icon_presence active dnd" style="opacity: 1;"></i>
			<span class="ts_tip_tip">active</span>
		</div>
					<span id="team_menu_user_name" class="overflow_ellipsis current_user_name">vanhakobyan</span>
			</div>
</div>
	<div id="col_channels" class="channels_list_holder no_unread_msgs_badges default_sort feature_message_replies_threads_view">

		<div class="placeholder_shimmer_clipper">
	<div class="placeholder_shimmer_bg_wrapper">
		<div class="placeholder_shimmer_bg"></div>
	</div>
</div>
		<div id="channels_nav" class="section_holder">
					</div>

		<div id="channels_scroller" class="show_which_channel_is_active" style="visibility: visible; height: 537px;">

			<ul id="all-unreads-list">
				<li data-action="show_unread_view" class="channels_nav_unread show_in_list_even_though_no_unreads unread_link all_unreads hidden">
					<a class="overflow_ellipsis channel_name" aria-label="Unread conversations">
						<ts-icon class="ts_icon_list"></ts-icon>
						All unreads					</a>
				</li>
			</ul>
							<ul id="all_threads_nav">
					<li data-action="show_threads_view" class="show_in_list_even_though_no_unreads all_threads">
						<a class="overflow_ellipsis channel_name" aria-label="Threads">
							<ts-icon class="ts_icon_small_reply"></ts-icon>
							<span class="unread_highlights hidden"></span>
							<span class="all_threads_label">All Threads</span><span class="new_threads_label">New Threads</span>
						</a>
					</li>
				</ul>
			
			<div id="unread" role="navigation" class="section_holder hidden" aria-label="Unreads">
				<h2 id="unread_section_header" class="overflow_ellipsis">
					<ts-icon class="ts_icon_channel_list ts_icon_inherit" aria-hidden="true"></ts-icon>
					<span id="unread_msgs" class="hidden">Unread Messages</span>
					<span id="unread_mntns" class="hidden">Unread Mentions</span>
				</h2>
				<ul id="unread-list"></ul>
			</div>

			<div id="starred_div" role="navigation" class="section_holder hidden" aria-label="Starred conversations">
				<h2 id="starred_section_header" class="overflow_ellipsis">
					<ts-icon class="ts_icon_star" aria-hidden="true"></ts-icon>					Starred				</h2>
				<ul id="starred-list"></ul>
			</div>

			<div id="channels" role="navigation" class="section_holder" aria-label="Channels">
				<button class="new_channel_btn ts_icon ts_icon_plus_circle channels_list_new_btn btn_unstyle" data-toggle="tooltip" data-action="create_channel" title="" aria-label="Create new channel" data-original-title="Create new channel"></button>

				<h2 id="channels_header" class="hoverable">
																		<button class="channel_list_header_label btn_unstyle" data-qa="channel_list_header_label" data-toggle="tooltip" title="" aria-label="Browse all 1 channels" data-original-title="Browse all channels">
								Channels								<span class="header_count">(<span id="channel_header_count">3</span>)</span>
							</button>
															</h2>

				<ul id="channel-list" aria-label="channels">	<li class="group_G3B6Z0Y81 group active  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_G3B6Z0Y81"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
		<a href="/archives/betconstruct_backend" target="new_1485198992132" class="group_name" data-group-id="G3B6Z0Y81" aria-label="betconstruct_backend, channel">
					<ts-icon class="ts_icon_lock prefix" aria-hidden="true"></ts-icon>
			<span class="unread_msg_G3B6Z0Y81 unread_msgs hidden">0</span>
			<span class="unread_highlight_G3B6Z0Y81 unread_highlights 
			             hidden
			             ">
				0</span>
			<span class="display_flex">
				<span class="overflow_ellipsis">
					betconstruct_backend
				</span>

				
			</span>
		</a>
	</li>
	<li class="channel_C0U54BA95 channel ">
		<div class="hotness_icon hidden" id="hotness_C0U54BA95"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
		<a href="/archives/general" target="new_1485198992132" class="channel_name" data-channel-id="C0U54BA95" aria-label="general, channel">
					<ts-icon class="ts_icon_channel_pane_hash prefix" aria-hidden="true"></ts-icon>
							<span class="unread_msg_C0U54BA95 unread_msgs hidden">
				0
			</span>
			<span class="unread_highlight_C0U54BA95 unread_highlights hidden">
				0
			</span>
			<span class="display_flex">
				<span class="overflow_ellipsis">
					general
				</span>

				
			</span>
		</a>
	</li>
	<li class="channel_C0U54C6SH channel ">
		<div class="hotness_icon hidden" id="hotness_C0U54C6SH"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
		<a href="/archives/random" target="new_1485198992132" class="channel_name" data-channel-id="C0U54C6SH" aria-label="random, channel">
					<ts-icon class="ts_icon_channel_pane_hash prefix" aria-hidden="true"></ts-icon>
							<span class="unread_msg_C0U54C6SH unread_msgs hidden">
				0
			</span>
			<span class="unread_highlight_C0U54C6SH unread_highlights hidden">
				0
			</span>
			<span class="display_flex">
				<span class="overflow_ellipsis">
					random
				</span>

				
			</span>
		</a>
	</li>
</ul>
				<div class="clear_both"></div>
			</div>

			<div id="direct_messages" role="navigation" class="section_holder no_bottom_margin" aria-label="Direct Messages">
				<button class="new_dm_btn ts_icon ts_icon_plus_circle channels_list_new_btn btn_unstyle" data-toggle="tooltip" title="" aria-label="Open a Direct Message" data-qa="new_dm_btn" data-original-title="Open a Direct Message"></button>

				<h2 id="direct_messages_header" class="hoverable" data-toggle="tooltip" title="" aria-label="Direct Messages" data-original-title="Open a Direct Message">Direct Messages</h2>
				<ul id="im-list">

	<li class="member_USLACKBOT member  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3CFSSG22"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/slackbot" target="new_1485198992132" class="im_name nuc color_USLACKBOT color_757575" data-member-id="USLACKBOT" aria-label="slackbot, direct message, active">
				<span class="unread_highlight_USLACKBOT unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<i class="ts_icon ts_icon_heart slackbot_icon"></i>
						slackbot
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with slackbot" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3B5F2125 member  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3BTW5D6H"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/vanhakobyan" target="new_1485198992132" class="im_name nuc color_U3B5F2125 color_d58247" data-member-id="U3B5F2125" aria-label="">
				<span class="unread_highlight_U3B5F2125 unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3B5F2125" class="presence member_presence_U3B5F2125 active dnd" title="active"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						vanhakobyan
						 (you)
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with vanhakobyan" data-qa="im_close"></button>
	</li>
 

	<li class="member_U0U59721F member away  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3BRB6C0J"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/aghasi.lorsabyan" target="new_1485198992132" class="im_name nuc color_U0U59721F color_9f69e7" data-member-id="U0U59721F" aria-label="">
				<span class="unread_highlight_U0U59721F unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U0U59721F" class="presence member_presence_U0U59721F away dnd" title="away"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						aghasi.lorsabyan
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with aghasi.lorsabyan" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3CD6J85V member away  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3ET8TNKX"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/aramjam" target="new_1485198992132" class="im_name nuc color_U3CD6J85V color_e0a729" data-member-id="U3CD6J85V" aria-label="">
				<span class="unread_highlight_U3CD6J85V unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3CD6J85V" class="presence member_presence_U3CD6J85V away dnd" title="away"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						aramjam
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with aramjam" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3BR8V9PE member  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3RQXTU2F"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/hayk.harutyunyan" target="new_1485198992132" class="im_name nuc color_U3BR8V9PE color_2b6836" data-member-id="U3BR8V9PE" aria-label="hayk.harutyunyan, direct message, active">
				<span class="unread_highlight_U3BR8V9PE unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3BR8V9PE" class="presence active member_presence_U3BR8V9PE" title="active"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						hayk.harutyunyan
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with hayk.harutyunyan" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3BTJ0H5K member  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3CG4KGUF"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/hovo" target="new_1485198992132" class="im_name nuc color_U3BTJ0H5K color_4cc091" data-member-id="U3BTJ0H5K" aria-label="">
				<span class="unread_highlight_U3BTJ0H5K unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3BTJ0H5K" class="presence member_presence_U3BTJ0H5K active dnd" title="active"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						hovo
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with hovo" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3BSURBNW member  cursor_pointer away">
		<div class="hotness_icon hidden" id="hotness_D3R9A3X61"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/lusine" target="new_1485198992132" class="im_name nuc color_U3BSURBNW color_235e5b" data-member-id="U3BSURBNW" aria-label="">
				<span class="unread_highlight_U3BSURBNW unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3BSURBNW" class="presence member_presence_U3BSURBNW away" title="away"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						lusine
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with lusine" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3BNFSYSF member away  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3BRB6E5Q"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/meri" target="new_1485198992132" class="im_name nuc color_U3BNFSYSF color_99a949" data-member-id="U3BNFSYSF" aria-label="">
				<span class="unread_highlight_U3BNFSYSF unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3BNFSYSF" class="presence member_presence_U3BNFSYSF away dnd" title="away"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						meri
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with meri" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3BEMJGFK member  cursor_pointer away">
		<div class="hotness_icon hidden" id="hotness_D3QGVHYUB"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/shtigran" target="new_1485198992132" class="im_name nuc color_U3BEMJGFK color_50a0cf" data-member-id="U3BEMJGFK" aria-label="">
				<span class="unread_highlight_U3BEMJGFK unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3BEMJGFK" class="presence member_presence_U3BEMJGFK away dnd" title="away"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						shtigran
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with shtigran" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3B45EY1E member  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3BRB6DDY"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/suren" target="new_1485198992132" class="im_name nuc color_U3B45EY1E color_df3dc0" data-member-id="U3B45EY1E" aria-label="">
				<span class="unread_highlight_U3B45EY1E unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3B45EY1E" class="presence member_presence_U3B45EY1E active dnd" title="active"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						suren
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with suren" data-qa="im_close"></button>
	</li>
 

	<li class="member_U3BS7F6H0 member away  cursor_pointer">
		<div class="hotness_icon hidden" id="hotness_D3UM6SQS0"><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:57.5% 65%;background-size:4100%"></span></div>
		
		
		
			<a href="/team/tigran" target="new_1485198992132" class="im_name nuc color_U3BS7F6H0 color_db3150" data-member-id="U3BS7F6H0" aria-label="tigran, direct message, away">
				<span class="unread_highlight_U3BS7F6H0 unread_highlights hidden">0</span>
				<span class="typing_indicator"></span>
				<span class="overflow_ellipsis member_name">
							<span data-member-presence="U3BS7F6H0" class="presence away member_presence_U3BS7F6H0" title="away"><i aria-hidden="true" class="ts_icon ts_icon_presence presence_icon"></i></span>
						tigran
						
				</span>
			</a>
			<button class="ts_icon ts_icon_times_circle im_close btn_unstyle" aria-label="Close Direct Message with tigran" data-qa="im_close"></button>
	</li>
 </ul>
				<div class="clear_both"></div>
			</div>

			<button id="channel_list_invites_link" class="channel_list_add_link btn_unstyle dim" data-action="admin_invites_modal" aria-label="Invite people" data-clog-click="true" data-clog-event="INVITEMODAL_ACTION" data-clog-params="action=open_modal,trigger=click_channel_list_invite_btn"><i class="ts_icon ts_icon_plus_small float_left"></i> Invite people</button>

			<div id="everything" role="navigation" class="section_holder hidden" aria-label="Everything else">
				<h2 id="everything_section_header" class="overflow_ellipsis">
					<ts-icon class="ts_icon_channel_list ts_icon_inherit" aria-hidden="true"></ts-icon>
					<span id="everything_else" class="hidden">Everything Else</span>
					<span id="everything_at_top" class="hidden">Everything</span>
				</h2>
				<ul id="everything-list"></ul>
			</div>

		</div>

		<a id="channel_scroll_up" class="hidden" onclick="TS.client.ui.scrollSoTopUnseenChannelIsInView(this); return false" style="top: 0px;"><span>more unreads</span> <i class="ts_icon ts_icon_arrow_up"></i></a>
		<a id="channel_scroll_down" class="hidden" onclick="TS.client.ui.scrollSoBottomUnseenChannelIsInView(this); return false"><span>more unreads</span> <i class="ts_icon ts_icon_arrow_down"></i></a>

		<div id="col_channels_footer">
											<div id="quick_switcher_btn"><i class="ts_icon ts_icon_filter"></i><span id="quick_switcher_label" class="quick_switcher_label_windows_alignment">Quick Switcher</span><span id="quick_switcher_shortcut">Ctrl+K</span></div>
					</div>
	</div>
</div>
			<div class="client_main_container">
	
<header id="client_header">

	<div id="active_channel_name_overlay" class="onboarding_overlay hidden"></div>

	
		<div class="channel_header">
		<div class="messages_header">

<div class="channel_title">
		<h2 id="channel_name_container" class="channel_name_container">
			<span id="channel_name" class="channel_name" data-qa="channel_name">
					<span id="channel_title"><i class="ts_icon ts_icon_lock"></i>betconstruct_backend</span>
</span><div class="channel_actions_container"><a id="mute_container" class="mute_container ts_tip ts_tip_bottom"></a></div>
		</h2>

		<div id="channel_header_info" class="channel_header_info">
			
			<div id="star_container" class="channel_header_info_item star_container"><button data-group-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_bottom star_group ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this channel">
		Star this channel
	</span>
</button></div><span id="channel_members_toggle_count" class="channel_header_info_item blue_on_hover ts_tip ts_tip_bottom ts_tip_multiline"><ts-icon class="ts_icon_user ts_icon_inherit channel_members_icon"></ts-icon>
					<span id="channel_members_toggle_count_count">19</span><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">
						View member list
					</span></span></span><span id="pinned_item_count" class="channel_header_info_item blue_on_hover ts_tip ts_tip_bottom ts_tip_multiline"><ts-icon class="ts_icon_thumb_tack ts_icon_inherit ts_icon_align_bottom pinned_count_icon"></ts-icon><span id="pinned_item_count_count">4</span><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">
					View Pinned Items<br><span class="subtle_silver pin_count_new_pin_message"></span>
				</span></span></span><span class="channel_header_info_item" role="presentation"></span><span id="topic_inline_edit" class="channel_topic inline_edit inline_edit_editable inline_edit_hover"><span class="inline_edit_inner" data-instructions-text="Enter to submit, Esc to cancel"><span id="channel_topic_text" class="inline_edit_input no_jumbomoji" data-placeholder="Add a topic"></span></span></span></div>
	</div>

<div class="channel_title_info">
		<!-- calls button -->
		<div id="channel_calls_container" class="channel_calls_container">	<button class="channel_header_icon channel_calls_button voice_call btn_unstyle ts_tip ts_tip_bottom ts_tip_multiline ts_tip_delay_300 blue_on_hover">
		<span class="ts_tip_tip"><span class="ts_tip_multiline_inner">
			Only paid teams can start calls from channels.
		</span></span>
		<ts-icon class="call_icon call_window_offline ts_icon_phone" aria-hidden="true"></ts-icon>
	</button>
</div><button id="channel_actions_toggle" class="btn_unstyle blue_on_hover channel_actions_toggle channel_header_icon ts_tip ts_tip_bottom">
			<span class="ts_tip_tip">Channel Settings</span>
						<ts-icon class="ts_icon_cog_o" aria-hidden="true"></ts-icon>
		</button><button id="details_toggle" class="channel_header_icon btn_unstyle blue_on_hover channel_details_toggle ts_tip ts_tip_bottom ">
				<span class="ts_tip_tip">Show Channel Details</span>
							<ts-icon class="ts_icon_side_panel" aria-hidden="true"></ts-icon>
		</button>
			</div>
</div>
		<div class="flex_header">
						<div id="search_container">
				<form role="search" method="get" action="/search" id="header_search_form" class="search_form no_bottom_margin">
										<div class="icon_search_wrapper"><ts-icon class="ts_icon_search icon_search" aria-hidden="true"></ts-icon></div>
					<div class="search_input_wrapper"><input type="text" id="search_terms" name="q" class="search_input" placeholder="Search" autocomplete="off" maxlength="250" aria-label="Search"></div>
					<div class="search_clear_icon_wrapper"><button type="button" id="search_clear" class="btn_unstyle search_clear_icon" aria-label="Clear search field"><ts-icon class="ts_icon_times_circle" aria-hidden="true"></ts-icon></button></div>
				</form>
			</div><button id="recent_mentions_toggle" class="channel_header_icon btn_unstyle ts_tip ts_tip_bottom">
				<span class="ts_tip_tip">Show Activity</span>
				<ts-icon class="ts_icon_mentions" aria-hidden="true"></ts-icon>			</button><button id="stars_toggle" class="channel_header_icon btn_unstyle ts_tip ts_tip_bottom ts_tip_rightish">
				<span class="ts_tip_tip">Show Starred Items</span>
				<ts-icon class="ts_icon_star_o" aria-hidden="true"></ts-icon>			</button><button id="flex_menu_toggle" class="channel_header_icon blue_on_hover btn_unstyle ts_tip ts_tip_bottom ts_tip_right normal">
				<span class="ts_tip_tip">More Items</span>
				<div id="whats_new_burst" class="all_read"></div>
				<ts-icon class="ts_icon_vertical_ellipsis" aria-hidden="true"></ts-icon>				<span class="help_icon_icon" id="help_icon_circle_count">0</span>
				<div class="flex_menu_download_circle"></div>
			</button><button id="whats_new_toggle" class="channel_header_icon btn_unstyle ts_tip ts_tip_bottom ts_tip_right candy_red_bg neutral_white small_left_margin">
				<span class="ts_tip_tip">What's New</span>
				<ts-icon class="ts_icon_emoji_celebration" aria-hidden="true"></ts-icon>			</button>
		<div id="rxn_toast_div" class="hidden ts_tip ts_tip_bottom"></div></div>
	</div>
</header> <!-- client header -->


		
	
		<div id="client_body">

		<div id="col_messages">

						
							
<div id="footer">
	<div id="footer_overlay" class="onboarding_overlay hidden"></div>
	<div id="footer_msgs">
				<div id="msg_preview" class="hidden lato_regular">
			<div id="msg_preview_msg" class="message"></div>
		</div>

				<form id="msg_form" class="offline" onsubmit="TS.view.submit(); return false;" data-qa="message_form">
										<textarea id="msg_input" aria-label="Message input for Private Channel betconstruct_backend" data-qa="message_input" style="overflow-y: hidden; height: 43px;" placeholder="Message betconstruct_backend" autocorrect="off" autocomplete="off" spellcheck="true"></textarea>
			
			<a id="primary_file_button" data-js="primary_file_button" class="file_upload_btn" aria-label="File menu" onclick="return false;">
				<i class="ts_icon ts_icon_plus_thick"></i>
			</a>
			<input type="file" id="file_upload" class="offscreen" multiple="multiple" aria-hidden="true" data-qa="file_upload">

			<a id="main_emo_menu" class="emo_menu" aria-label="Emoji menu">
				<i class="ts_icon ts_icon_circle_fill"></i>
				<i class="ts_icon ts_icon_smile_o"></i>
				<i class="ts_icon ts_icon_happy_smile"></i>
			</a>

			<div id="msg_input_message"><span></span></div>

			
		</form>
		<div id="notification_bar" class="">
			<div id="typing_text" class="overflow_ellipsis" role="status" aria-live="polite" aria-atomic="true"></div>
			<div id="special_formatting_text" class="special_formatting_tips" aria-hidden="true"><b>*bold*</b> <i>_italics_</i> ~strike~ <code>`code`</code> <code class="preformatted">```preformatted```</code> <span class="quote">&gt;quote</span></div>
			<div id="snippet_prompt" class="hidden">
				<div class="warning">
					Text is too long!					<a class="snippet_link ts_tip ts_tip_top ts_tip_multiline" onclick="TS.client.msg_input.createSnippetFromPrompt()">
						<span class="ts_tip_tip">
							<span class="ts_tip_multiline_inner">
								A snippet is a text file that can be much longer than a normal message.							</span>
						</span>
						Make this a snippet
					</a>
					instead?				</div>
			</div>
		</div>
	</div>
	<div id="footer_archives" class="hidden">
		<div id="footer_archives_table">
			<div id="footer_archives_left"><span id="footer_archives_text"></span></div>
			<div id="footer_archives_right"><a class="btn btn_outline btn_small" id="footer_archives_action_button"></a><br><span id="footer_archives_action_tip"></span></div>
		</div>
	</div>
</div>			
				
								<div id="messages_container" role="main" class="">

					<div id="unread_msgs_scroller_div"></div>

											<div id="threads_msgs_scroller_div" class="loading" data-loading-text="Loading messages..." data-slow-loading-text="Still loading... sorry for the long wait!" data-empty-text="No threads yet" data-empty-instructions="No one has replied to your message yet. You can also follow threads and stay up‑to‑date here."></div>
					
					<div id="archive_msgs_scroller_div" class="hidden">
						<div id="archives_top_div" class="msgs_holder hidden mini italic"></div>
						<div id="archives_msgs_div" class="msgs_holder"></div>
						<div id="archives_bottom_div" class="msgs_holder hidden mini italic"></div>
					</div>

					<div id="msgs_scroller_div" tabindex="-1" style="height: 544px;">

						<div id="end_div" class="relative mini help" style="height: 115px;">
							<div id="end_display_onboarding" class="hidden onboarding">
								<div id="onboarding_header">
									<div id="onboarding_fade_out_mask" class="hidden"></div>
									<span id="onboarding_welcome_text" class="lato_light">Welcome!</span>
									<span id="onboarding_welcome_message" class="align_center lato_bold">Slack is a messaging app for teams.</span>
									<div id="onboarding_video" class="display_flex align_items_center justify_content_center align_center hidden" style="background: url('/img/newxp/newxp_video_preview_2x.png') 50% 50% no-repeat;background-size:contain; width:398px; height:224px; margin-top:15px;">
										<button id="onboarding_video_play" class="tour_btn btn pill_btn btn_large btn_info ts_icon ts_icon_play" style="box-shadow:0 5px 10px 5px rgba(0,0,0,.24);">Watch the Tour</button>
									</div>
									<div id="in_skip_messaging" class="align_center hidden">Got the hang of Slack already? <a role="button" class="skip_tutorial_link">Skip the tutorial.</a></div>
									<div id="unskip_messaging" class="align_center hidden">I changed my mind. <a role="button" class="take_tutorial_link">Take the tutorial.</a></div>
								</div>
								<div id="onboarding_footer">
									<div id="explore_btn_container" class="align_center">
										<a role="button" class="btn">Explore Slack</a>
									</div>
									<div id="pre_skip_messaging" class="align_center">Not your first Slack team? <a role="button" class="skip_tutorial_link">Skip the tutorial.</a></div>
								</div>
							</div>
							<div id="end_display_div" class="relative">
								<div id="end_display_padder" style="height: 16px;"></div>
								<div id="end_display_meta" class="hidden">
									<div id="channel_meta" class="hidden">
										<h1 class="small_bottom_margin channel_meta_name"></h1>
										<p class="small_bottom_margin">
											
											<span id="channel_creator_name" class=""></span> created this channel
											<span class="channel_meta_shared_info dusty_springfield_grey hidden"></span>
											<span id="channel_create_date"></span>.
																						
											<span class="not_limited_copy">This is the very beginning of the </span>
											<span class="is_limited_copy hidden">This is the </span>
											<span class="channel_meta_name"></span> channel.
																						<span id="channel_meta_purpose_container">
												Purpose: <span id="channel_meta_purpose" class="italic no_jumbomoji"></span> (<a role="button" class="end_action_purpose">edit</a>)											</span>
										</p>
										<ul class="end_display_actions">
											<li><a role="button" class="end_action_purpose"><ts-icon class="ts_icon_pencil ts_icon_inherit" aria-hidden="true"></ts-icon> Set a purpose</a></li>											<li><a role="button" class="end_action_integration" href="" target="new"><ts-icon class="ts_icon_plus ts_icon_inherit" aria-hidden="true"></ts-icon>												Add an app or custom integration											</a></li>
											<li><a class="end_action_invite"><i class="ts_icon ts_icon_user ts_icon_inherit"></i> Invite others to this channel</a></li>
											<li class="hidden"><span class="end_action_slack_invite blue_link" data-clog-click="true" data-clog-event="INVITEMODAL_ACTION" data-clog-params="action=open_modal,trigger=click_general_channel_invite_btn"></span></li>
										</ul>
									</div>
									<div id="group_meta" class="hidden">
										<h1 class="small_bottom_margin group_meta_name"></h1>
										<p class="small_bottom_margin">
											
											<span id="group_creator_name"></span> created this private channel
											<span class="group_meta_shared_info dusty_springfield_grey hidden"></span>
											<span id="group_create_date"></span>.											
											<span class="not_limited_copy">This is the very beginning of the </span>
											<span class="is_limited_copy hidden">This is the </span>
											<span class="group_meta_name bold"></span> private channel.
																						<span id="group_meta_purpose_container">
												Purpose: <span id="group_meta_purpose" class="no_jumbomoji italic"></span> (<a role="button" class="end_action_purpose">edit</a>)											</span>
											<span id="group_meta_archived_parent">
												It was created from the now archived private channel <a role="button" id="group_meta_archived_parent_link" href="" target="_blank"></a>.											</span>
										</p>
										<ul class="end_display_actions">
											<li><a role="button" class="end_action_purpose"><ts-icon class="ts_icon_pencil ts_icon_inherit" aria-hidden="true"></ts-icon> Set a purpose</a></li>											<li><a role="button" class="end_action_integration" href="" target="new"><ts-icon class="ts_icon_plus ts_icon_inherit" aria-hidden="true"></ts-icon>												Add an app or custom integration											</a></li>
											<li><a role="button" class="end_action_invite"><ts-icon class="ts_icon_user ts_icon_inherit" aria-hidden="true"></ts-icon> Invite others to this private channel</a></li>
										</ul>
									</div>
									<div id="slackbot_meta" class="hidden">
										This is Slackbot display
									</div>
									<div id="im_meta" class="hidden">
										This is Direct Message display
									</div>

									<div class="is_limited_div is_limited_copy hidden mini">
										<ts-icon class="ts_icon_comment_o " aria-hidden="true"></ts-icon> Your team has more than 10,000 messages in its archive, so although there are older messages than are shown below, you can't see them. <a href="/pricing" target="_blank" class="bold">Find out more about upgrading your team.</a>
									</div>
								</div>
								<div id="end_display_status" class="" aria-live="polite" aria-atomic="true"><a onclick="TS.client.ui.doLoadScrollBackHistory(true)">And more...</a></div>
							</div>
						</div>
						<div id="msgs_div" class="msgs_holder"><div class="day_container"><div class="day_divider" id="day_divider_1484750285_000022" data-date="January 18th, 2017" data-ts="1484750285.000022"><i class="copy_only"><br>----- </i><div class="day_divider_label" aria-label="January eighteenth, twenty seventeen">January 18th</div><i class="copy_only">  -----</i></div>
<div class="day_msgs" data-date="January 18th, 2017" data-ts="1484750285.000022">

<ts-message id="msg_1484750285_000022" data-ts="1484750285.000022" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BNFSYSF" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484750285000022">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484750285000022" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/meri" target="/team/meri" class=" member_preview_link member_image thumb_36" data-member-id="U3BNFSYSF" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BNFSYSF-c475b1c2e374-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484750285000022" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:38 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 18th at 6:38:05 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484750285.000022" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/meri" target="/team/meri" class="message_sender color_U3BNFSYSF color_99a949 member member_preview_link " data-member-id="U3BNFSYSF">meri</a>
				<a href="/archives/betconstruct_backend/p1484750285000022" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:38 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 18th at 6:38:05 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484750285.000022" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>DirectoryTree<br><a href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;]" data-referer-original-href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" rel="noreferrer" target="_blank">https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;]" data-referer-original-href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" rel="noreferrer" target="_blank">
						marysahakyan/UsefulExamples</a>
						
					</div>

						Contribute to UsefulExamples development by creating an account on GitHub.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;]" data-referer-original-href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24479739%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24479739%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="edited ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Jan 18th at 6:38 PM"> (edited)</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484750285_000022-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484750285_000022_label" class="message_aria_label hidden">
			<strong>meri</strong>.
			DirectoryTree<br><a href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fmarysahakyan%2FUsefulExamples%2Ftree%2Fmaster%2FDirectoryTree&quot;]" data-referer-original-href="https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree" rel="noreferrer" target="_blank">https://github.com/marysahakyan/UsefulExamples/tree/master/DirectoryTree</a>.
			NaN replies
			six thirty-eight PM. Edited.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484766484_000029" data-ts="1484766484.000029" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/vanhakobyan/F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484766484000029" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:08 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 18th at 11:08:04 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3TV5J66A" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484766484000029" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:08 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 18th at 11:08:04 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3TV5J66A" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3TV5J66A" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" data-file-id="F3TV5J66A">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Does not work finlly</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 320px;">

	<a data-file-id="F3TV5J66A" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3TV5J66A-73098d87cd/pasted_image_at_2017_01_18_11_07_pm_360.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" target="https://files.slack.com/files-pri/T0U4V6GA0-F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" style="width: 320px;" class="file_body image_body image_png
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3TV5J66A-73098d87cd/pasted_image_at_2017_01_18_11_07_pm_360.png" style="
					padding-top: -webkit-calc( 320 / 320 * 100%); padding-top: -moz-calc( 320 / 320 * 100%); padding-top: calc( 320 / 320 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3TV5J66A-73098d87cd/pasted_image_at_2017_01_18_11_07_pm_360.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3TV5J66A" href="https://files.slack.com/files-pri/T0U4V6GA0-F3TV5J66A/download/pasted_image_at_2017_01_18_11_07_pm.png" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3TV5J66A" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" data-file-id="F3TV5J66A" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3TV5J66A-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							<a href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/stackOverFlowException" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FstackOverFlowException&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FstackOverFlowException&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/stackOverFlowException" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/ProjectsGroup/tree/master/stackOverFlowException</a>
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484766484_000029_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> uploaded a file: <a href="https://micarmenia.slack.com/files/vanhakobyan/F3TV5J66A/pasted_image_at_2017_01_18_11_07_pm.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3TV5J66A">Does not work finlly</a> and commented: <a href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/stackOverFlowException" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FstackOverFlowException&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FstackOverFlowException&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/stackOverFlowException" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/ProjectsGroup/tree/master/stackOverFlowException</a>.
			NaN replies
			eleven oh-eight PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484767822_000030" data-ts="1484767822.000030" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/tigran/F3TC58NMB/unnesfiles.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484767822000030" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:30 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 18th at 11:30:22 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3TC58NMB" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1484767822000030" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:30 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 18th at 11:30:22 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3TC58NMB" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3TC58NMB" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/tigran/F3TC58NMB/unnesfiles.gif" target="https://micarmenia.slack.com/files/tigran/F3TC58NMB/unnesfiles.gif" data-file-id="F3TC58NMB">
						
						
						

							uploaded this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Unnesfiles.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3TC58NMB" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3TC58NMB-bda4d997d6/unnesfiles_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3TC58NMB/unnesfiles.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3TC58NMB/unnesfiles.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3TC58NMB/unnesfiles.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3TC58NMB-bda4d997d6/unnesfiles_360.gif" style="
					padding-top: -webkit-calc( 173 / 360 * 100%); padding-top: -moz-calc( 173 / 360 * 100%); padding-top: calc( 173 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3TC58NMB-bda4d997d6/unnesfiles_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3TC58NMB" href="https://files.slack.com/files-pri/T0U4V6GA0-F3TC58NMB/download/unnesfiles.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3TC58NMB" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/tigran/F3TC58NMB/unnesfiles.gif" target="https://micarmenia.slack.com/files/tigran/F3TC58NMB/unnesfiles.gif" data-file-id="F3TC58NMB" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>Add Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3TC58NMB-"></div>





		<i class="copy_only"><br></i>


		<span id="msg_1484767822_000030_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/tigran/F3TC58NMB/unnesfiles.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3TC58NMB">Unnesfiles.gif</a>.
			NaN replies
			eleven thirty PM.
		</span>

	</div>

</ts-message>
 </div></div><div class="day_container"><div class="day_divider" id="day_divider_1484769808_000031" data-date="January 19th, 2017" data-ts="1484769808.000031"><i class="copy_only"><br>----- </i><div class="day_divider_label" aria-label="January nineteenth, twenty seventeen">January 19th</div><i class="copy_only">  -----</i></div>
<div class="day_msgs" data-date="January 19th, 2017" data-ts="1484769808.000031">

<ts-message id="msg_1484769808_000031" data-ts="1484769808.000031" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B1NMZK2" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484769808000031">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/khachik" target="/team/khachik" class=" member_preview_link member_image thumb_36" data-member-id="U3B1NMZK2" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B1NMZK2-64649df3e28a-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484769808000031" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:03 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:03:28 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484769808.000031" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/khachik" target="/team/khachik" class="message_sender color_U3B1NMZK2 color_684b6c member member_preview_link " data-member-id="U3B1NMZK2">khachik</a>
				<a href="/archives/betconstruct_backend/p1484769808000031" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:03 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:03:28 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484769808.000031" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp; &nbsp; <a href="https://github.com/KhachikSukiasyan/Inheritance-example" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Inheritance-example" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/Inheritance-example</a><br><a href="https://github.com/KhachikSukiasyan/Fibonacci-number" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Fibonacci-number" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/Fibonacci-number</a><br><a href="https://github.com/KhachikSukiasyan/Vectors" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Vectors" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/Vectors</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/KhachikSukiasyan/Inheritance-example">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/KhachikSukiasyan/Inheritance-example" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Inheritance-example" rel="noreferrer" target="_blank">
						KhachikSukiasyan/Inheritance-example</a>
						
					</div>

						Inheritance-example - Inheritance example
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/KhachikSukiasyan/Inheritance-example" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Inheritance-example" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 

<div class="inline_attachment standalone has_thumb" data-attachment-id="2" data-real-src="https://github.com/KhachikSukiasyan/Fibonacci-number">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/KhachikSukiasyan/Fibonacci-number" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Fibonacci-number" rel="noreferrer" target="_blank">
						KhachikSukiasyan/Fibonacci-number</a>
						
					</div>

						Fibonacci-number - Indexer example in C#
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/KhachikSukiasyan/Fibonacci-number" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Fibonacci-number" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 

<div class="inline_attachment standalone has_thumb" data-attachment-id="3" data-real-src="https://github.com/KhachikSukiasyan/Vectors">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/KhachikSukiasyan/Vectors" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Vectors" rel="noreferrer" target="_blank">
						KhachikSukiasyan/Vectors</a>
						
					</div>

						Vectors - Operator overloading example in C#
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/KhachikSukiasyan/Vectors" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Vectors" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484769808_000031-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484769808_000031_label" class="message_aria_label hidden">
			<strong>khachik</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp; &nbsp; <a href="https://github.com/KhachikSukiasyan/Inheritance-example" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FInheritance-example&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Inheritance-example" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/Inheritance-example</a><br><a href="https://github.com/KhachikSukiasyan/Fibonacci-number" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFibonacci-number&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Fibonacci-number" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/Fibonacci-number</a><br><a href="https://github.com/KhachikSukiasyan/Vectors" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FVectors&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/Vectors" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/Vectors</a>.
			NaN replies
			twelve oh-three AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484770566_000033" data-ts="1484770566.000033" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484770566000033" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:16 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:16:06 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3U191PN3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484770566000033" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:16 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:16:06 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3U191PN3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3U191PN3" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" target="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" data-file-id="F3U191PN3">
						
						
						

							uploaded this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Test.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3U191PN3" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3U191PN3-d63ce590e1/test_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3U191PN3/test.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3U191PN3/test.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3U191PN3/test.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3U191PN3-d63ce590e1/test_360.gif" style="
					padding-top: -webkit-calc( 248 / 360 * 100%); padding-top: -moz-calc( 248 / 360 * 100%); padding-top: calc( 248 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3U191PN3-d63ce590e1/test_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3U191PN3" href="https://files.slack.com/files-pri/T0U4V6GA0-F3U191PN3/download/test.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3U191PN3" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" target="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" data-file-id="F3U191PN3" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3U191PN3-"></div>





		<i class="copy_only"><br></i>


		<span id="msg_1484770566_000033_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3U191PN3">Test.gif</a>.
			NaN replies
			twelve sixteen AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484770588_000034" data-ts="1484770588.000034" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484770588000034">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484770588000034" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:16 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:16:28 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484770588.000034" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484770588000034" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:16 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:16:28 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484770588.000034" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;]" data-referer-original-href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" rel="noreferrer" target="_blank">https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;]" data-referer-original-href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" rel="noreferrer" target="_blank">
						shtigran/ArmenianTranslitOfEnglishTranslator</a>
						
					</div>

						ArmenianTranslitOfEnglishTranslator - Armenian Translit Of English Translator, Armenian translit, translit
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;]" data-referer-original-href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484770588_000034-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484770588_000034_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FArmenianTranslitOfEnglishTranslator&quot;]" data-referer-original-href="https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator" rel="noreferrer" target="_blank">https://github.com/shtigran/ArmenianTranslitOfEnglishTranslator</a>.
			NaN replies
			twelve sixteen AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484770869_000036" data-ts="1484770869.000036" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first file_reference file_share first" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484770869000036">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484770869000036" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:21 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:21:09 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-comment-id="Fc3U110LGN" data-file-id="F3U191PN3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484770869000036" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:21 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:21:09 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-comment-id="Fc3U110LGN" data-file-id="F3U191PN3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
					
			</div>
				
		</div>


					<span class="meta meta_feature_fix_files message_body no_jumbomoji">
							commented on
						<a href="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" target="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" data-file-id="F3U191PN3" class="file_preview_link file_force_flexpane file_name">Test.gif</a>
							<a href="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" target="new_1485198992132" data-toggle="tooltip" title="Open file in a new tab" aria-label="Open file in a new tab" data-file-id="F3U191PN3" class="file_new_window_link">
						<i class="ts_icon ts_icon_external_link file_inline_icon"></i></a>
					</span>






					<div class="comment">
						Սպասում եմ Ձեր &nbsp;bug-երին <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>
					</div>
					<div class="rxn_panel rxns_key_file_comment-Fc3U110LGN-"></div>



		<i class="copy_only"><br></i>


		<span id="msg_1484770869_000036_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a> commented on <a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a>’s file <a href="https://micarmenia.slack.com/files/shtigran/F3U191PN3/test.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3U191PN3">Test.gif</a>: Սպասում եմ Ձեր &nbsp;bug-երին <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			twelve twenty-one AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484813459_000004" data-ts="1484813459.000004" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/tigran/F3SRP48G0/workwithfile.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484813459000004" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:10 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:10:59 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3SRP48G0" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1484813459000004" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:10 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:10:59 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3SRP48G0" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3SRP48G0" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/tigran/F3SRP48G0/workwithfile.gif" target="https://micarmenia.slack.com/files/tigran/F3SRP48G0/workwithfile.gif" data-file-id="F3SRP48G0">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Workwithfile.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3SRP48G0" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3SRP48G0-92143915fe/workwithfile_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3SRP48G0/workwithfile.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3SRP48G0/workwithfile.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3SRP48G0/workwithfile.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3SRP48G0-92143915fe/workwithfile_360.gif" style="
					padding-top: -webkit-calc( 203 / 360 * 100%); padding-top: -moz-calc( 203 / 360 * 100%); padding-top: calc( 203 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3SRP48G0-92143915fe/workwithfile_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3SRP48G0" href="https://files.slack.com/files-pri/T0U4V6GA0-F3SRP48G0/download/workwithfile.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3SRP48G0" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/tigran/F3SRP48G0/workwithfile.gif" target="https://micarmenia.slack.com/files/tigran/F3SRP48G0/workwithfile.gif" data-file-id="F3SRP48G0" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3SRP48G0-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							In this project about 52% of code is for exeption handling
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484813459_000004_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/tigran/F3SRP48G0/workwithfile.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3SRP48G0">Workwithfile.gif</a> and commented: In this project about 52% of code is for exeption handling.
			NaN replies
			zero ten PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484813486_000005" data-ts="1484813486.000005" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484813486000005">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484813486000005" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:11 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:11:26 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484813486.000005" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1484813486000005" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:11 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:11:26 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484813486.000005" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> <a href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" rel="noreferrer" target="_blank">https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" rel="noreferrer" target="_blank">
						tigranv/Useful-examples</a>
						
					</div>

						Useful-examples - In this repository, I gathered a lot of useful examples of code that I create while studying programming
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24522089%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24522089%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484813486_000005-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484813486_000005_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> <a href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FWorkWithFiles&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles" rel="noreferrer" target="_blank">https://github.com/tigranv/Useful-examples/tree/master/WorkWithFiles</a>.
			NaN replies
			zero eleven PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484816022_000007" data-ts="1484816022.000007" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BTJ0H5K" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484816022000007">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hovo" target="/team/hovo" class=" member_preview_link member_image thumb_36" data-member-id="U3BTJ0H5K" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BTJ0H5K-7c76331c1e87-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484816022000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:53:42 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484816022.000007" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hovo" target="/team/hovo" class="message_sender color_U3BTJ0H5K color_4cc091 member member_preview_link " data-member-id="U3BTJ0H5K">hovo</a>
				<a href="/archives/betconstruct_backend/p1484816022000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 12:53:42 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484816022.000007" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>Hi guys<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484816022_000007-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484816022_000007_label" class="message_aria_label hidden">
			<strong>hovo</strong>.
			Hi guys.
			NaN replies
			zero fifty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484817182_000008" data-ts="1484817182.000008" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/tigran/F3TKXBYFN/lattoarmtrans.png">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484817182000008" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:13 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 1:13:02 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3TKXBYFN" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1484817182000008" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:13 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 1:13:02 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3TKXBYFN" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3TKXBYFN" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/tigran/F3TKXBYFN/lattoarmtrans.png" target="https://micarmenia.slack.com/files/tigran/F3TKXBYFN/lattoarmtrans.png" data-file-id="F3TKXBYFN">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">lattoarmtrans.PNG</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3TKXBYFN" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3TKXBYFN-7c2429bdf6/lattoarmtrans_720.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3TKXBYFN/lattoarmtrans.png" target="https://files.slack.com/files-pri/T0U4V6GA0-F3TKXBYFN/lattoarmtrans.png" style="width: 360px;" class="file_body image_body image_png
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3TKXBYFN/lattoarmtrans.png" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3TKXBYFN-7c2429bdf6/lattoarmtrans_720.png" style="
					padding-top: -webkit-calc( 36 / 360 * 100%); padding-top: -moz-calc( 36 / 360 * 100%); padding-top: calc( 36 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3TKXBYFN-7c2429bdf6/lattoarmtrans_720.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions  overflow_preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3TKXBYFN" href="https://files.slack.com/files-pri/T0U4V6GA0-F3TKXBYFN/download/lattoarmtrans.png" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3TKXBYFN" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/tigran/F3TKXBYFN/lattoarmtrans.png" target="https://micarmenia.slack.com/files/tigran/F3TKXBYFN/lattoarmtrans.png" data-file-id="F3TKXBYFN" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3TKXBYFN-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							Ավելի գրագետ
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484817182_000008_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/tigran/F3TKXBYFN/lattoarmtrans.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3TKXBYFN">lattoarmtrans.PNG</a> and commented: Ավելի գրագետ.
			NaN replies
			one thirteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484818455_000009" data-ts="1484818455.000009" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B45EY1E" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484818455000009">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/suren" target="/team/suren" class=" member_preview_link member_image thumb_36" data-member-id="U3B45EY1E" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B45EY1E-3e93cfe1e3db-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484818455000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:34 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 1:34:15 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484818455.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/suren" target="/team/suren" class="message_sender color_U3B45EY1E color_df3dc0 member member_preview_link " data-member-id="U3B45EY1E">suren</a>
				<a href="/archives/betconstruct_backend/p1484818455000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:34 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 1:34:15 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484818455.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/SurenKhachatryan/PasswordGenerator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;]" data-referer-original-href="https://github.com/SurenKhachatryan/PasswordGenerator" rel="noreferrer" target="_blank">https://github.com/SurenKhachatryan/PasswordGenerator</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/SurenKhachatryan/PasswordGenerator">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/SurenKhachatryan/PasswordGenerator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;]" data-referer-original-href="https://github.com/SurenKhachatryan/PasswordGenerator" rel="noreferrer" target="_blank">
						SurenKhachatryan/PasswordGenerator</a>
						
					</div>

						PasswordGenerator - Password Generator in C#
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/SurenKhachatryan/PasswordGenerator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;]" data-referer-original-href="https://github.com/SurenKhachatryan/PasswordGenerator" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars3.githubusercontent.com%2Fu%2F24530125%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars3.githubusercontent.com%2Fu%2F24530125%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484818455_000009-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484818455_000009_label" class="message_aria_label hidden">
			<strong>suren</strong>.
			<a href="https://github.com/SurenKhachatryan/PasswordGenerator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FSurenKhachatryan%2FPasswordGenerator&quot;]" data-referer-original-href="https://github.com/SurenKhachatryan/PasswordGenerator" rel="noreferrer" target="_blank">https://github.com/SurenKhachatryan/PasswordGenerator</a>.
			NaN replies
			one thirty-four PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484818547_000011" data-ts="1484818547.000011" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BTJ0H5K" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484818547000011">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hovo" target="/team/hovo" class=" member_preview_link member_image thumb_36" data-member-id="U3BTJ0H5K" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BTJ0H5K-7c76331c1e87-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484818547000011" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:35 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 1:35:47 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484818547.000011" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hovo" target="/team/hovo" class="message_sender color_U3BTJ0H5K color_4cc091 member member_preview_link " data-member-id="U3BTJ0H5K">hovo</a>
				<a href="/archives/betconstruct_backend/p1484818547000011" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:35 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 1:35:47 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484818547.000011" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/HovoNalbandyan/Delete-Temps" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;]" data-referer-original-href="https://github.com/HovoNalbandyan/Delete-Temps" rel="noreferrer" target="_blank">https://github.com/HovoNalbandyan/Delete-Temps</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/HovoNalbandyan/Delete-Temps">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/HovoNalbandyan/Delete-Temps" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;]" data-referer-original-href="https://github.com/HovoNalbandyan/Delete-Temps" rel="noreferrer" target="_blank">
						HovoNalbandyan/Delete-Temps</a>
						
					</div>

						Delete-Temps - The Program Delete Temp Files On Your Computer
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/HovoNalbandyan/Delete-Temps" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;]" data-referer-original-href="https://github.com/HovoNalbandyan/Delete-Temps" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24522046%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24522046%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484818547_000011-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484818547_000011_label" class="message_aria_label hidden">
			<strong>hovo</strong>.
			<a href="https://github.com/HovoNalbandyan/Delete-Temps" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FHovoNalbandyan%2FDelete-Temps&quot;]" data-referer-original-href="https://github.com/HovoNalbandyan/Delete-Temps" rel="noreferrer" target="_blank">https://github.com/HovoNalbandyan/Delete-Temps</a>.
			NaN replies
			one thirty-five PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484822899_000013" data-ts="1484822899.000013" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484822899000013">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484822899000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:48 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 2:48:19 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484822899.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1484822899000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:48 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 2:48:19 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484822899.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/LusineHovs/IO" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;]" data-referer-original-href="https://github.com/LusineHovs/IO" rel="noreferrer" target="_blank">https://github.com/LusineHovs/IO</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/LusineHovs/IO">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/LusineHovs/IO" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;]" data-referer-original-href="https://github.com/LusineHovs/IO" rel="noreferrer" target="_blank">
						LusineHovs/IO</a>
						
					</div>

						IO - Here you will find how to work with Files/Directories
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/LusineHovs/IO" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;]" data-referer-original-href="https://github.com/LusineHovs/IO" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24455176%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24455176%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484822899_000013-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484822899_000013_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			<a href="https://github.com/LusineHovs/IO" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FIO&quot;]" data-referer-original-href="https://github.com/LusineHovs/IO" rel="noreferrer" target="_blank">https://github.com/LusineHovs/IO</a>.
			NaN replies
			two forty-eight PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484823208_000015" data-ts="1484823208.000015" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484823208000015">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484823208000015" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 2:53:28 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484823208.000015" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484823208000015" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 2:53:28 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484823208.000015" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> <a href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" rel="noreferrer" target="_blank">https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" rel="noreferrer" target="_blank">
						harutyunyanhayk/PublicProjects</a>
						
					</div>

						PublicProjects - Random, password, generator
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F19515285%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F19515285%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484823208_000015-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484823208_000015_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> <a href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FPublicProjects%2Ftree%2Fmaster%2FFileManager&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager" rel="noreferrer" target="_blank">https://github.com/harutyunyanhayk/PublicProjects/tree/master/FileManager</a>.
			NaN replies
			two fifty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484824763_000017" data-ts="1484824763.000017" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CDJ064X" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484824763000017">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/gor" target="/team/gor" class=" member_preview_link member_image thumb_36" data-member-id="U3CDJ064X" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CDJ064X-0135b4a52b62-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484824763000017" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 3:19:23 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484824763.000017" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/gor" target="/team/gor" class="message_sender color_U3CDJ064X color_5b89d5 member member_preview_link " data-member-id="U3CDJ064X">gor</a>
				<a href="/archives/betconstruct_backend/p1484824763000017" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 3:19:23 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484824763.000017" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/GorTerGamanyan/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;]" data-referer-original-href="https://github.com/GorTerGamanyan/FileManager" rel="noreferrer" target="_blank">https://github.com/GorTerGamanyan/FileManager</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/GorTerGamanyan/FileManager">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/GorTerGamanyan/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;]" data-referer-original-href="https://github.com/GorTerGamanyan/FileManager" rel="noreferrer" target="_blank">
						GorTerGamanyan/FileManager</a>
						
					</div>

						Contribute to FileManager development by creating an account on GitHub.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/GorTerGamanyan/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;]" data-referer-original-href="https://github.com/GorTerGamanyan/FileManager" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F14791162%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F14791162%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484824763_000017-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484824763_000017_label" class="message_aria_label hidden">
			<strong>gor</strong>.
			<a href="https://github.com/GorTerGamanyan/FileManager" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FGorTerGamanyan%2FFileManager&quot;]" data-referer-original-href="https://github.com/GorTerGamanyan/FileManager" rel="noreferrer" target="_blank">https://github.com/GorTerGamanyan/FileManager</a>.
			NaN replies
			three nineteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484826342_000019" data-ts="1484826342.000019" data-model-ob-id="G3B6Z0Y81" data-member-id="U0U59721F" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484826342000019">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_36" data-member-id="U0U59721F" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484826342000019" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:45 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 3:45:42 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484826342.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class="message_sender color_U0U59721F color_9f69e7 member member_preview_link " data-member-id="U0U59721F">aghasi.lorsabyan</a>
				<a href="/archives/betconstruct_backend/p1484826342000019" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:45 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 3:45:42 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484826342.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://msdn.microsoft.com/en-us/library/d5x73970.aspx" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fmsdn.microsoft.com%2Fen-us%2Flibrary%2Fd5x73970.aspx&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fmsdn.microsoft.com%2Fen-us%2Flibrary%2Fd5x73970.aspx&quot;]" data-referer-original-href="https://msdn.microsoft.com/en-us/library/d5x73970.aspx" rel="noreferrer" target="_blank">https://msdn.microsoft.com/en-us/library/d5x73970.aspx</a><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484826342_000019-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484826342_000019_label" class="message_aria_label hidden">
			<strong>aghasi.lorsabyan</strong>.
			<a href="https://msdn.microsoft.com/en-us/library/d5x73970.aspx" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fmsdn.microsoft.com%2Fen-us%2Flibrary%2Fd5x73970.aspx&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fmsdn.microsoft.com%2Fen-us%2Flibrary%2Fd5x73970.aspx&quot;]" data-referer-original-href="https://msdn.microsoft.com/en-us/library/d5x73970.aspx" rel="noreferrer" target="_blank">https://msdn.microsoft.com/en-us/library/d5x73970.aspx</a>.
			NaN replies
			three forty-five PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484828732_000020" data-ts="1484828732.000020" data-model-ob-id="G3B6Z0Y81" data-member-id="U0U59721F" class="message feature_fix_files is_pinned dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484828732000020">
		</div>

	<span class="is_pinned_holder">

<ts-icon class="ts_icon_thumb_tack_filled ts_icon_inherit ts_icon_align_bottom ts_tip ts_tip_top ts_tip_float ts_tip_multiline">
		<span class="ts_tip_tip">
			<span class="ts_tip_multiline_inner">
					Pinned by aghasi.lorsabyan
			<br>
				<span class="subtle_silver">
						Jan 19th at 4:25 PM
				</span>
			</span>
		</span>
</ts-icon>
			Pinned by aghasi.lorsabyan
 </span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_36" data-member-id="U0U59721F" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484828732000020" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>4:25 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 4:25:32 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484828732.000020" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class="message_sender color_U0U59721F color_9f69e7 member member_preview_link " data-member-id="U0U59721F">aghasi.lorsabyan</a>
				<a href="/archives/betconstruct_backend/p1484828732000020" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>4:25 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 4:25:32 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484828732.000020" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="http://www.introprogramming.info/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fwww.introprogramming.info%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fwww.introprogramming.info%2F&quot;]" data-referer-original-href="http://www.introprogramming.info/" rel="noreferrer" target="_blank">http://www.introprogramming.info/</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone" data-attachment-id="1" data-real-src="http://www.introprogramming.info/">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16.ip&amp;url=http%3A%2F%2Fwww.introprogramming.info%2Fwp-content%2Fthemes%2Fintroprograming_en_abc%2Ffavicon.ico" alt=""></span>

					<span class="attachment_source_name">introprogramming.info</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="http://www.introprogramming.info/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fwww.introprogramming.info%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fwww.introprogramming.info%2F&quot;]" data-referer-original-href="http://www.introprogramming.info/" rel="noreferrer" target="_blank">
						Introduction to Programming with C# / Java Books</a>
						
					</div>

						Fundamentals of Programming with C# and Java books by Svetlin Nakov and his team - official web site
					<span class="media_caret"></span>
			</div>





	</div>

	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484828732_000020-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484828732_000020_label" class="message_aria_label hidden">
			<strong>aghasi.lorsabyan</strong>.
			<a href="http://www.introprogramming.info/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fwww.introprogramming.info%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fwww.introprogramming.info%2F&quot;]" data-referer-original-href="http://www.introprogramming.info/" rel="noreferrer" target="_blank">http://www.introprogramming.info/</a>.
			NaN replies
			four twenty-five PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484838022_000025" data-ts="1484838022.000025" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="comment" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add comment …"></a><a data-action="share_file" data-permalink="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share file …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484838022000025" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:00 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 7:00:22 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3UCSAJ87" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484838022000025" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:00 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 7:00:22 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3UCSAJ87" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3UCSAJ87" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" data-file-id="F3UCSAJ87">
						
						
						

							uploaded this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">notC</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 356px;">

	<a data-file-id="F3UCSAJ87" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UCSAJ87-2880652d70/pasted_image_at_2017_01_19_06_59_pm_360.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" target="https://files.slack.com/files-pri/T0U4V6GA0-F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" style="width: 356px;" class="file_body image_body image_png
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3UCSAJ87-2880652d70/pasted_image_at_2017_01_19_06_59_pm_360.png" style="
					padding-top: -webkit-calc( 126 / 356 * 100%); padding-top: -moz-calc( 126 / 356 * 100%); padding-top: calc( 126 / 356 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UCSAJ87-2880652d70/pasted_image_at_2017_01_19_06_59_pm_360.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3UCSAJ87" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UCSAJ87/download/pasted_image_at_2017_01_19_06_59_pm.png" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3UCSAJ87" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" data-file-id="F3UCSAJ87" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>Add Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3UCSAJ87- " data-rxn-key="file-F3UCSAJ87-"><span data-emoji="muscle::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@aramjam, @shtigran, @gayane, @narekye, and @tigran <span class=&quot;subtle_silver&quot;>reacted with :muscle::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:50% 57.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="5"></span>
</span><span data-emoji="grinning" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 user_reacted" title="You (click to remove) <span class=&quot;subtle_silver&quot;>reacted with :grinning:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 50%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>





		<i class="copy_only"><br></i>


		<span id="msg_1484838022_000025_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> uploaded a file: <a href="https://micarmenia.slack.com/files/vanhakobyan/F3UCSAJ87/pasted_image_at_2017_01_19_06_59_pm.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UCSAJ87">notC</a>.
			NaN replies
			seven o'clock PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484848902_000034" data-ts="1484848902.000034" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="comment" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add comment …"></a><a data-action="share_file" data-permalink="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share file …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484848902000034" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:01 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 10:01:42 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3UFUHNLW" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1484848902000034" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:01 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 10:01:42 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3UFUHNLW" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3UFUHNLW" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif" target="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif" data-file-id="F3UFUHNLW">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">փիղիկներ</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3UFUHNLW" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UFUHNLW-61d3e80f5a/ezgif.com-9a05c6e84e_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UFUHNLW/ezgif.com-9a05c6e84e.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3UFUHNLW/ezgif.com-9a05c6e84e.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3UFUHNLW/ezgif.com-9a05c6e84e.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3UFUHNLW-61d3e80f5a/ezgif.com-9a05c6e84e_360.gif" style="
					padding-top: -webkit-calc( 343 / 360 * 100%); padding-top: -moz-calc( 343 / 360 * 100%); padding-top: calc( 343 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UFUHNLW-61d3e80f5a/ezgif.com-9a05c6e84e_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3UFUHNLW" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UFUHNLW/download/ezgif.com-9a05c6e84e.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3UFUHNLW" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif" target="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif" data-file-id="F3UFUHNLW" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3UFUHNLW- " data-rxn-key="file-F3UFUHNLW-"><span data-emoji="+1" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@shtigran, @gayane, @suren, @khachik, and @meri <span class=&quot;subtle_silver&quot;>reacted with :+1:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 22.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="5"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							checks any changes on the desktop
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484848902_000034_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> uploaded a file: <a href="https://micarmenia.slack.com/files/aramjam/F3UFUHNLW/ezgif.com-9a05c6e84e.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UFUHNLW">փիղիկներ</a> and commented: checks any changes on the desktop.
			NaN replies
			ten oh-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484851728_000037" data-ts="1484851728.000037" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="comment" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add comment …"></a><a data-action="share_file" data-permalink="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share file …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484851728000037" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:48 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 10:48:48 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3T5AREKS" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484851728000037" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:48 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 10:48:48 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3T5AREKS" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3T5AREKS" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif" target="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif" data-file-id="F3T5AREKS">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Tree Creator.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3T5AREKS" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3T5AREKS-e1ef5b3c53/tree_creator_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3T5AREKS/tree_creator.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3T5AREKS/tree_creator.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3T5AREKS/tree_creator.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3T5AREKS-e1ef5b3c53/tree_creator_360.gif" style="
					padding-top: -webkit-calc( 255 / 360 * 100%); padding-top: -moz-calc( 255 / 360 * 100%); padding-top: calc( 255 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3T5AREKS-e1ef5b3c53/tree_creator_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3T5AREKS" href="https://files.slack.com/files-pri/T0U4V6GA0-F3T5AREKS/download/tree_creator.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3T5AREKS" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif" target="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif" data-file-id="F3T5AREKS" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3T5AREKS- " data-rxn-key="file-F3T5AREKS-"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@aramjam, @meri, and @khachik <span class=&quot;subtle_silver&quot;>reacted with :+1::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="3"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							Directory Tree Creator
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484851728_000037_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/shtigran/F3T5AREKS/tree_creator.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3T5AREKS">Tree Creator.gif</a> and commented: Directory Tree Creator.
			NaN replies
			ten forty-eight PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484851733_000038" data-ts="1484851733.000038" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484851733000038">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484851733000038" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:48 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 10:48:53 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484851733.000038" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484851733000038" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:48 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 19th at 10:48:53 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484851733.000038" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/TreeDirectoryCreator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;]" data-referer-original-href="https://github.com/shtigran/TreeDirectoryCreator" rel="noreferrer" target="_blank">https://github.com/shtigran/TreeDirectoryCreator</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/shtigran/TreeDirectoryCreator">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/shtigran/TreeDirectoryCreator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;]" data-referer-original-href="https://github.com/shtigran/TreeDirectoryCreator" rel="noreferrer" target="_blank">
						shtigran/TreeDirectoryCreator</a>
						
					</div>

						Contribute to TreeDirectoryCreator development by creating an account on GitHub.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/shtigran/TreeDirectoryCreator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;]" data-referer-original-href="https://github.com/shtigran/TreeDirectoryCreator" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484851733_000038-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484851733_000038_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/TreeDirectoryCreator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FTreeDirectoryCreator&quot;]" data-referer-original-href="https://github.com/shtigran/TreeDirectoryCreator" rel="noreferrer" target="_blank">https://github.com/shtigran/TreeDirectoryCreator</a>.
			NaN replies
			ten forty-eight PM.
		</span>

	</div>

</ts-message>
 </div></div><div class="day_container"><div class="day_divider" id="day_divider_1484863851_000043" data-date="January 20th, 2017" data-ts="1484863851.000043"><i class="copy_only"><br>----- </i><div class="day_divider_label" aria-label="January twentieth, twenty seventeen">January 20th</div><i class="copy_only">  -----</i></div>
<div class="day_msgs" data-date="January 20th, 2017" data-ts="1484863851.000043">

<ts-message id="msg_1484863851_000043" data-ts="1484863851.000043" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484863851000043" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:10 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 2:10:51 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3U2BURHA" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484863851000043" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:10 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 2:10:51 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3U2BURHA" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3U2BURHA" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" target="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" data-file-id="F3U2BURHA">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Desktop Cleaner.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 359px;">

	<a data-file-id="F3U2BURHA" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3U2BURHA-2177a514b0/desktop_cleaner_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3U2BURHA/desktop_cleaner.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3U2BURHA/desktop_cleaner.gif" style="width: 359px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3U2BURHA/desktop_cleaner.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3U2BURHA-2177a514b0/desktop_cleaner_360.gif" style="
					padding-top: -webkit-calc( 360 / 359 * 100%); padding-top: -moz-calc( 360 / 359 * 100%); padding-top: calc( 360 / 359 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3U2BURHA-2177a514b0/desktop_cleaner_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3U2BURHA" href="https://files.slack.com/files-pri/T0U4V6GA0-F3U2BURHA/download/desktop_cleaner.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3U2BURHA" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" target="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" data-file-id="F3U2BURHA" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>2 Comments</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3U2BURHA-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							Desktop Cleaner
						</div>
						<div class="rxn_panel rxns_key_file_comment-Fc3U2C20J0-"></div>
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484863851_000043_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3U2BURHA">Desktop Cleaner.gif</a> and commented: Desktop Cleaner.
			NaN replies
			two ten AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484863857_000044" data-ts="1484863857.000044" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484863857000044">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484863857000044" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:10 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 2:10:57 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484863857.000044" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484863857000044" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:10 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 2:10:57 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484863857.000044" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/DesktopCleaner" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;]" data-referer-original-href="https://github.com/shtigran/DesktopCleaner" rel="noreferrer" target="_blank">https://github.com/shtigran/DesktopCleaner</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/shtigran/DesktopCleaner">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/shtigran/DesktopCleaner" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;]" data-referer-original-href="https://github.com/shtigran/DesktopCleaner" rel="noreferrer" target="_blank">
						shtigran/DesktopCleaner</a>
						
					</div>

						DesktopCleaner - Desktop Temprory Folders and Files Cleaner
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/shtigran/DesktopCleaner" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;]" data-referer-original-href="https://github.com/shtigran/DesktopCleaner" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484863857_000044-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484863857_000044_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/DesktopCleaner" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FDesktopCleaner&quot;]" data-referer-original-href="https://github.com/shtigran/DesktopCleaner" rel="noreferrer" target="_blank">https://github.com/shtigran/DesktopCleaner</a>.
			NaN replies
			two ten AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484897305_000004" data-ts="1484897305.000004" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first file_reference file_share first" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484897305000004">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484897305000004" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:28 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:28:25 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-comment-id="Fc3U6SQAN8" data-file-id="F3U2BURHA" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1484897305000004" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:28 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:28:25 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-comment-id="Fc3U6SQAN8" data-file-id="F3U2BURHA" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
					
			</div>
				
		</div>


					<span class="meta meta_feature_fix_files message_body no_jumbomoji">
									commented on <a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>’s file
						<a href="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" target="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" data-file-id="F3U2BURHA" class="file_preview_link file_force_flexpane file_name">Desktop Cleaner.gif</a>
							<a href="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" target="new_1485198992132" data-toggle="tooltip" title="Open file in a new tab" aria-label="Open file in a new tab" data-file-id="F3U2BURHA" class="file_new_window_link">
						<i class="ts_icon ts_icon_external_link file_inline_icon"></i></a>
					</span>






					<div class="comment">
						Very nice one :)
					</div>
					<div class="rxn_panel rxns_key_file_comment-Fc3U6SQAN8-"></div>



		<i class="copy_only"><br></i>


		<span id="msg_1484897305_000004_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> commented on <a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a>’s file <a href="https://micarmenia.slack.com/files/shtigran/F3U2BURHA/desktop_cleaner.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3U2BURHA">Desktop Cleaner.gif</a>: Very nice one :).
			NaN replies
			eleven twenty-eight AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484920966_000007" data-ts="1484920966.000007" data-model-ob-id="G3B6Z0Y81" data-member-id="U0U59721F" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1484920966.000007" data-parent-user-id="">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484920966000007">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_36" data-member-id="U0U59721F" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484920966000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:02 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:02:46 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484920966.000007" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class="message_sender color_U0U59721F color_9f69e7 member member_preview_link " data-member-id="U0U59721F">aghasi.lorsabyan</a>
				<a href="/archives/betconstruct_backend/p1484920966000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:02 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:02:46 PM</span></span></span></a>
					
				

					
					<span class="message_star_holder">

<button data-msg-id="1484920966.000007" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><b class="mention">@channel</b> Lets start tomorrow's training at 11:00. Please comment if you can't attend.<span class="constrain_triple_clicks"></span></span>

				





						<div class="rxn_panel rxns_key_message-1484920966_000007-G3B6Z0Y81"></div>
						

<div class="reply_bar">
	<div class="reply_faces">
					<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_24" data-member-id="U3CD6J85V" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-24')" aria-hidden="true"></a>
	
					<a href="/team/tsovinar" target="/team/tsovinar" class=" member_preview_link member_image thumb_24" data-member-id="U3B4Q1S8Y" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B4Q1S8Y-g3ea0086a8a6-24')" aria-hidden="true"></a>
	
					<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_24" data-member-id="U3BEMJGFK" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-24')" aria-hidden="true"></a>
	
						<a href="/team/khachik" target="/team/khachik" class=" member_preview_link member_image thumb_24" data-member-id="U3B1NMZK2" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B1NMZK2-64649df3e28a-24')" aria-hidden="true"></a>
	
	</div>	<div class="reply_summary">
		<a href="/conversation/betconstruct_backend/p1484920966000007" target="_blank" class="reply_count">
			4 replies
		</a>

		<div class="meta_hover_placement">
			<span class="last_reply_at">Last reply 3 days ago</span>
			<span class="view_conv_hover">View thread</span>
		</div>
	</div>
	<ts-icon class="reply_bar_caret ts_icon_chevron_right"></ts-icon>
</div>
 





		<i class="copy_only"><br></i>


		<span id="msg_1484920966_000007_label" class="message_aria_label hidden">
			<strong>aghasi.lorsabyan</strong>.
			<b class="mention">@channel</b> Lets start tomorrow's training at 11:00. Please comment if you can't attend..
						4 replies
			4 replies
			six oh-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484921652_000012" data-ts="1484921652.000012" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484921652000012">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484921652000012" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:14 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:14:12 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484921652.000012" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484921652000012" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:14 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:14:12 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484921652.000012" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>+1<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484921652_000012-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484921652_000012_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			+1.
			NaN replies
			six fourteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484922776_000013" data-ts="1484922776.000013" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484922776000013">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484922776000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:32 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:32:56 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484922776.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484922776000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:32 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:32:56 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484922776.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>+1<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484922776_000013-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484922776_000013_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			+1.
			NaN replies
			six thirty-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484923422_000014" data-ts="1484923422.000014" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B541ABB" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484923422000014">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/gayane" target="/team/gayane" class=" member_preview_link member_image thumb_36" data-member-id="U3B541ABB" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B541ABB-g3583865332e-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484923422000014" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:43 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:43:42 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484923422.000014" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/gayane" target="/team/gayane" class="message_sender color_U3B541ABB color_9b3b45 member member_preview_link " data-member-id="U3B541ABB">gayane</a>
				<a href="/archives/betconstruct_backend/p1484923422000014" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:43 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:43:42 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484923422.000014" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>I &nbsp;can <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484923422_000014-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484923422_000014_label" class="message_aria_label hidden">
			<strong>gayane</strong>.
			I &nbsp;can <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			six forty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484923946_000015" data-ts="1484923946.000015" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BTJ0H5K" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484923946000015">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hovo" target="/team/hovo" class=" member_preview_link member_image thumb_36" data-member-id="U3BTJ0H5K" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BTJ0H5K-7c76331c1e87-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484923946000015" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:52 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:52:26 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484923946.000015" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hovo" target="/team/hovo" class="message_sender color_U3BTJ0H5K color_4cc091 member member_preview_link " data-member-id="U3BTJ0H5K">hovo</a>
				<a href="/archives/betconstruct_backend/p1484923946000015" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:52 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 6:52:26 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484923946.000015" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>its good.i can<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484923946_000015-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484923946_000015_label" class="message_aria_label hidden">
			<strong>hovo</strong>.
			its good.i can.
			NaN replies
			six fifty-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484925599_000016" data-ts="1484925599.000016" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484925599000016">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484925599000016" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 7:19:59 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484925599.000016" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1484925599000016" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 7:19:59 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484925599.000016" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>+1<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484925599_000016-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484925599_000016_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			+1.
			NaN replies
			seven nineteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484927196_000017" data-ts="1484927196.000017" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B1NMZK2" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484927196000017">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/khachik" target="/team/khachik" class=" member_preview_link member_image thumb_36" data-member-id="U3B1NMZK2" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B1NMZK2-64649df3e28a-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484927196000017" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:46 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 7:46:36 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484927196.000017" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/khachik" target="/team/khachik" class="message_sender color_U3B1NMZK2 color_684b6c member member_preview_link " data-member-id="U3B1NMZK2">khachik</a>
				<a href="/archives/betconstruct_backend/p1484927196000017" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:46 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 7:46:36 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484927196.000017" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/KhachikSukiasyan/TranslitToArmenian" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/TranslitToArmenian" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/TranslitToArmenian</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/KhachikSukiasyan/TranslitToArmenian">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/KhachikSukiasyan/TranslitToArmenian" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/TranslitToArmenian" rel="noreferrer" target="_blank">
						KhachikSukiasyan/TranslitToArmenian</a>
						
					</div>

						TranslitToArmenian - Translates translit text to Հայերեն (extension methods example in C#)
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/KhachikSukiasyan/TranslitToArmenian" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/TranslitToArmenian" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484927196_000017-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484927196_000017_label" class="message_aria_label hidden">
			<strong>khachik</strong>.
			<a href="https://github.com/KhachikSukiasyan/TranslitToArmenian" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FTranslitToArmenian&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/TranslitToArmenian" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/TranslitToArmenian</a>.
			NaN replies
			seven forty-six PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484930163_000019" data-ts="1484930163.000019" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1484930163.000019" data-parent-user-id="">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484930163000019">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484930163000019" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:36:03 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484930163.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484930163000019" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:36:03 PM</span></span></span></a>
					
				

					
					<span class="message_star_holder">

<button data-msg-id="1484930163.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>People what program u use for making gif?<span class="constrain_triple_clicks"></span></span>

				





						<div class="rxn_panel rxns_key_message-1484930163_000019-G3B6Z0Y81"></div>
						

<div class="reply_bar">
	<div class="reply_faces">
						<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_24" data-member-id="U3CD6J85V" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-24')" aria-hidden="true"></a>
	
	</div>	<div class="reply_summary">
		<a href="/conversation/betconstruct_backend/p1484930163000019" target="_blank" class="reply_count">
			1 reply
		</a>

		<div class="meta_hover_placement">
			<span class="last_reply_at">3 days ago</span>
			<span class="view_conv_hover">View thread</span>
		</div>
	</div>
	<ts-icon class="reply_bar_caret ts_icon_chevron_right"></ts-icon>
</div>
 





		<i class="copy_only"><br></i>


		<span id="msg_1484930163_000019_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			People what program u use for making gif?.
						1 reply
			1 reply
			eight thirty-six PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484930199_000020" data-ts="1484930199.000020" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484930199000020">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484930199000020" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:36:39 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484930199.000020" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484930199000020" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:36:39 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484930199.000020" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>camgif<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484930199_000020-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484930199_000020_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			camgif.
			NaN replies
			eight thirty-six PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484930217_000023" data-ts="1484930217.000023" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484930217000023">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484930217000023" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:36:57 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484930217.000023" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1484930217000023" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:36:57 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484930217.000023" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>gyazo <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484930217_000023-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484930217_000023_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			gyazo <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			eight thirty-six PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484930230_000024" data-ts="1484930230.000024" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484930230000024">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484930230000024" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:37 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:37:10 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484930230.000024" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484930230000024" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:37 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:37:10 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484930230.000024" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>gyazo? ;-O<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484930230_000024-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484930230_000024_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			gyazo? ;-O.
			NaN replies
			eight thirty-seven PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484930261_000025" data-ts="1484930261.000025" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484930261000025">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484930261000025" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:37 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:37:41 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484930261.000025" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1484930261000025" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:37 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:37:41 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484930261.000025" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>why not? <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484930261_000025-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484930261_000025_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			why not? <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			eight thirty-seven PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484930986_000026" data-ts="1484930986.000026" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484930986000026">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484930986000026" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:49 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:49:46 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484930986.000026" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484930986000026" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:49 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:49:46 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484930986.000026" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>եսիմ <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484930986_000026-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484930986_000026_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			եսիմ <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			eight forty-nine PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931033_000027" data-ts="1484931033.000027" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931033000027">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931033000027" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:50 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:50:33 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931033.000027" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484931033000027" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:50 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:50:33 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931033.000027" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> &nbsp;գյազո անունը վանումա<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931033_000027-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931033_000027_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> &nbsp;գյազո անունը վանումա.
			NaN replies
			eight fifty PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931063_000028" data-ts="1484931063.000028" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931063000028">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931063000028" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:51 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:51:03 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931063.000028" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484931063000028" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:51 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:51:03 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931063.000028" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>aha<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931063_000028-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931063_000028_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			aha.
			NaN replies
			eight fifty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931120_000029" data-ts="1484931120.000029" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931120000029">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931120000029" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:52 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:52:00 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931120.000029" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1484931120000029" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:52 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:52:00 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931120.000029" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" data-member-name="hayk.harutyunyan" data-stringify-text="@U3BR8V9PE" class="internal_member_link">@hayk.harutyunyan</a> <a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> &nbsp;let me disagree with you, i use gyazo and i find gyazo a gyazan program<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931120_000029-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931120_000029_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" data-member-name="hayk.harutyunyan" data-stringify-text="@U3BR8V9PE" class="internal_member_link">@hayk.harutyunyan</a> <a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> &nbsp;let me disagree with you, i use gyazo and i find gyazo a gyazan program.
			NaN replies
			eight fifty-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931215_000030" data-ts="1484931215.000030" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931215000030">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931215000030" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:53:35 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931215.000030" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484931215000030" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:53:35 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931215.000030" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> &nbsp;I fully agree with you.<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931215_000030-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931215_000030_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> &nbsp;I fully agree with you..
			NaN replies
			eight fifty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931229_000031" data-ts="1484931229.000031" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931229000031">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931229000031" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:53:49 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931229.000031" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484931229000031" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:53 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:53:49 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931229.000031" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>I'll try it now<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931229_000031-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931229_000031_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			I'll try it now.
			NaN replies
			eight fifty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931364_000032" data-ts="1484931364.000032" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931364000032">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931364000032" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931364000032" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:56 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:56:04 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931364.000032" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1484931364000032" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:56 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:56:04 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931364.000032" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> did you see how Gyazo's marketing acted <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931364_000032-G3B6Z0Y81 " data-rxn-key="message-1484931364.000032-G3B6Z0Y81"><span data-emoji="writing_hand::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 user_reacted" title="You (click to remove) <span class=&quot;subtle_silver&quot;>reacted with :writing_hand::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:7.5% 70%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931364_000032_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> did you see how Gyazo's marketing acted <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span>.
			NaN replies
			eight fifty-six PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484931550_000034" data-ts="1484931550.000034" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931550000034">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484931550000034" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484931550000034" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:59 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:59:10 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484931550.000034" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1484931550000034" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:59 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 8:59:10 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484931550.000034" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/VanHakobyan/AGA" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;]" data-referer-original-href="https://github.com/VanHakobyan/AGA" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/AGA</a><br>my first repositori in GitHub

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb can_delete" data-attachment-id="1" data-real-src="https://github.com/VanHakobyan/AGA">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/VanHakobyan/AGA" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;]" data-referer-original-href="https://github.com/VanHakobyan/AGA" rel="noreferrer" target="_blank">
						<span class="mention">VanHakobyan</span>/AGA</a>
						
					</div>

						AGA - MOG,ՄՈԳ, Calculator,Average, Qualitative , Appraisal, YSU, University ,
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/VanHakobyan/AGA" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;]" data-referer-original-href="https://github.com/VanHakobyan/AGA" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F23220521%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F23220521%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	

		<div class="delete_attachment_link" data-attachment-id="1"><ts-icon class="ts_icon_times_small"></ts-icon></div>

	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484931550_000034-G3B6Z0Y81 " data-rxn-key="message-1484931550.000034-G3B6Z0Y81"><span data-emoji="+1" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@hovo <span class=&quot;subtle_silver&quot;>reacted with :+1:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 22.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484931550_000034_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="https://github.com/VanHakobyan/AGA" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FAGA&quot;]" data-referer-original-href="https://github.com/VanHakobyan/AGA" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/AGA</a><br>my first repositori in GitHub.
			NaN replies
			eight fifty-nine PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484932235_000038" data-ts="1484932235.000038" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BDBJLDN" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484932235000038">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/satenik" target="/team/satenik" class=" member_preview_link member_image thumb_36" data-member-id="U3BDBJLDN" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BDBJLDN-381a7acb45fa-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484932235000038" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:10 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 9:10:35 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484932235.000038" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/satenik" target="/team/satenik" class="message_sender color_U3BDBJLDN color_5870dd member member_preview_link " data-member-id="U3BDBJLDN">satenik</a>
				<a href="/archives/betconstruct_backend/p1484932235000038" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:10 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 9:10:35 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484932235.000038" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;I can<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484932235_000038-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484932235_000038_label" class="message_aria_label hidden">
			<strong>satenik</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;I can.
			NaN replies
			nine ten PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484932826_000039" data-ts="1484932826.000039" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B7NFX8R" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484932826000039">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/anush" target="/team/anush" class=" member_preview_link member_image thumb_36" data-member-id="U3B7NFX8R" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B7NFX8R-f9dab9170634-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484932826000039" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:20 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 9:20:26 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484932826.000039" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/anush" target="/team/anush" class="message_sender color_U3B7NFX8R color_53b759 member member_preview_link " data-member-id="U3B7NFX8R">anush</a>
				<a href="/archives/betconstruct_backend/p1484932826000039" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:20 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 9:20:26 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484932826.000039" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>It is ok for me<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484932826_000039-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484932826_000039_label" class="message_aria_label hidden">
			<strong>anush</strong>.
			It is ok for me.
			NaN replies
			nine twenty PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484937494_000046" data-ts="1484937494.000046" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B1NMZK2" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484937494000046">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/khachik" target="/team/khachik" class=" member_preview_link member_image thumb_36" data-member-id="U3B1NMZK2" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B1NMZK2-64649df3e28a-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484937494000046" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:38 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 10:38:14 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484937494.000046" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/khachik" target="/team/khachik" class="message_sender color_U3B1NMZK2 color_684b6c member member_preview_link " data-member-id="U3B1NMZK2">khachik</a>
				<a href="/archives/betconstruct_backend/p1484937494000046" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:38 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 10:38:14 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484937494.000046" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>
	<span class="attachment_preamble for_attachment_group">

<span class="meta reply_broadcast_preamble">

		replied to a
		<a data-action="open_conversation" data-thread-ts="1484920966.000007" data-model-ob-id="G3B6Z0Y81" href="/conversation/betconstruct_backend/p1484920966000007" target="/conversation/betconstruct_backend/p1484920966000007">thread</a>

</span>
 </span>

	
	<div class="attachment_group has_link has_container">
		

<div class="inline_attachment standalone clickable message_unfurl reply_broadcast" data-attachment-id="1" data-real-src="https://micarmenia.slack.com/archives/betconstruct_backend/p1484920966000007" data-attachment-ts="1484920966.000007">



	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><a href="https://micarmenia.slack.com/team/aghasi.lorsabyan" target="_blank" class="member_preview_link" data-member-id="U0U59721F"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Favatars.slack-edge.com%2F2016-12-07%2F113051366160_389563add683335d83fa_48.jpg" alt=""></a></span>

					<span class="attachment_source_name"><a href="https://micarmenia.slack.com/team/aghasi.lorsabyan" target="_blank" class="member_preview_link" data-member-id="U0U59721F">aghasi.lorsabyan</a></span>


					<span class="attachment_meta">6:02 PM</span>

				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">

						<b class="mention">@channel</b> Lets start tomorrow's training at 11:00. Please comment if you can't attend.
					
			</div>





	</div>

	


	
		<a href="https://micarmenia.slack.com/archives/betconstruct_backend/p1484920966000007" class="attachment_from_url_link offscreen" target="_blank">https://micarmenia.slack.com/archives/betconstruct_backend/p1484920966000007</a>
	

</div>

 

<span class="attachment_rule reply_broadcast_rule">
	<span class="attachment_rule_inner reply_broadcast_count">

			4 replies

	</span>
</span>
 

<div class="inline_attachment standalone clickable message_unfurl reply_broadcast" data-attachment-id="2" data-real-src="https://micarmenia.slack.com/archives/betconstruct_backend/p1484937494000044?thread_ts=1484920966000007&amp;cid=G3B6Z0Y81" data-attachment-ts="1484937494.000044">



	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><a href="https://micarmenia.slack.com/team/khachik" target="_blank" class="member_preview_link" data-member-id="U3B1NMZK2"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Favatars.slack-edge.com%2F2016-12-08%2F113481524688_64649df3e28aa2680075_48.jpg" alt=""></a></span>

					<span class="attachment_source_name"><a href="https://micarmenia.slack.com/team/khachik" target="_blank" class="member_preview_link" data-member-id="U3B1NMZK2">khachik</a></span>


					<span class="attachment_meta">10:38 PM</span>

				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">

						I can come
					
			</div>





	</div>

	


	
		<a href="https://micarmenia.slack.com/archives/betconstruct_backend/p1484937494000044?thread_ts=1484920966000007&amp;cid=G3B6Z0Y81" class="attachment_from_url_link offscreen" target="_blank">https://micarmenia.slack.com/archives/betconstruct_backend/p1484937494000044?thread_ts=1484920966000007&amp;cid=G3B6Z0Y81</a>
	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484937494_000046-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484937494_000046_label" class="message_aria_label hidden">
			<strong>khachik</strong>.
			.
			NaN replies
			ten thirty-eight PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484937767_000047" data-ts="1484937767.000047" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5S19SM" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484937767000047">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusinekhachatryan" target="/team/lusinekhachatryan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5S19SM" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5S19SM-28a9785116d7-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484937767000047" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:42 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 10:42:47 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484937767.000047" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusinekhachatryan" target="/team/lusinekhachatryan" class="message_sender color_U3B5S19SM color_5a4592 member member_preview_link " data-member-id="U3B5S19SM">lusinekhachatryan</a>
				<a href="/archives/betconstruct_backend/p1484937767000047" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:42 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 10:42:47 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484937767.000047" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>I can<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484937767_000047-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484937767_000047_label" class="message_aria_label hidden">
			<strong>lusinekhachatryan</strong>.
			I can.
			NaN replies
			ten forty-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484940701_000052" data-ts="1484940701.000052" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484940701000052">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484940701000052" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:31 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:31:41 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484940701.000052" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1484940701000052" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:31 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:31:41 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484940701.000052" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>+<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484940701_000052-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484940701_000052_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			+.
			NaN replies
			eleven thirty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484940904_000053" data-ts="1484940904.000053" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files dirty_hover_container" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484940904000053">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484940904000053" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="light_only">11:35</span><span class="dense_only">11:35 PM</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:35:04 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484940904.000053" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1484940904000053" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:35 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:35:04 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484940904.000053" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> make sure the doors will be open<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 57.5%;background-size:4100%" title="smiley">:smiley:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484940904_000053-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484940904_000053_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> make sure the doors will be open<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 57.5%;background-size:4100%" title="smiley">:smiley:</span>.
			NaN replies
			eleven thirty-five PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484941123_000054" data-ts="1484941123.000054" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484941123000054">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484941123000054" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:38 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:38:43 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484941123.000054" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1484941123000054" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:38 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 20th at 11:38:43 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484941123.000054" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> Is 11:00 final?<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484941123_000054-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484941123_000054_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> Is 11:00 final?.
			NaN replies
			eleven thirty-eight PM.
		</span>

	</div>

</ts-message>
 </div></div><div class="day_container"><div class="day_divider" id="day_divider_1484945127_000055" data-date="January 21st, 2017" data-ts="1484945127.000055"><i class="copy_only"><br>----- </i><div class="day_divider_label" aria-label="January twenty-first, twenty seventeen">January 21st</div><i class="copy_only">  -----</i></div>
<div class="day_msgs" data-date="January 21st, 2017" data-ts="1484945127.000055">

<ts-message id="msg_1484945127_000055" data-ts="1484945127.000055" data-model-ob-id="G3B6Z0Y81" data-member-id="U0U59721F" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484945127000055">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_36" data-member-id="U0U59721F" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484945127000055" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:45 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 12:45:27 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484945127.000055" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class="message_sender color_U0U59721F color_9f69e7 member member_preview_link " data-member-id="U0U59721F">aghasi.lorsabyan</a>
				<a href="/archives/betconstruct_backend/p1484945127000055" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:45 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 12:45:27 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484945127.000055" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><b class="mention">@channel</b> the door will be open.<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484945127_000055-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484945127_000055_label" class="message_aria_label hidden">
			<strong>aghasi.lorsabyan</strong>.
			<b class="mention">@channel</b> the door will be open..
			NaN replies
			twelve forty-five AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484946279_000056" data-ts="1484946279.000056" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/tigran/F3V69FFRD/directory_path.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484946279000056" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:04 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 1:04:39 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3V69FFRD" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1484946279000056" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:04 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 1:04:39 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3V69FFRD" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3V69FFRD" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/tigran/F3V69FFRD/directory_path.gif" target="https://micarmenia.slack.com/files/tigran/F3V69FFRD/directory_path.gif" data-file-id="F3V69FFRD">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Directory Path.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3V69FFRD" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3V69FFRD-4f5d132975/directory_path_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3V69FFRD/directory_path.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3V69FFRD/directory_path.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3V69FFRD/directory_path.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3V69FFRD-4f5d132975/directory_path_360.gif" style="
					padding-top: -webkit-calc( 191 / 360 * 100%); padding-top: -moz-calc( 191 / 360 * 100%); padding-top: calc( 191 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3V69FFRD-4f5d132975/directory_path_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3V69FFRD" href="https://files.slack.com/files-pri/T0U4V6GA0-F3V69FFRD/download/directory_path.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3V69FFRD" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/tigran/F3V69FFRD/directory_path.gif" target="https://micarmenia.slack.com/files/tigran/F3V69FFRD/directory_path.gif" data-file-id="F3V69FFRD" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3V69FFRD-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							Այ դիդ իթ
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484946279_000056_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/tigran/F3V69FFRD/directory_path.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3V69FFRD">Directory Path.gif</a> and commented: Այ դիդ իթ.
			NaN replies
			one oh-four AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484947964_000057" data-ts="1484947964.000057" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B1NMZK2" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/khachik/F3UJ1LL6Q/filetest.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/khachik" target="/team/khachik" class=" member_preview_link member_image thumb_36" data-member-id="U3B1NMZK2" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B1NMZK2-64649df3e28a-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484947964000057" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:32 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 1:32:44 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3UJ1LL6Q" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/khachik" target="/team/khachik" class="message_sender color_U3B1NMZK2 color_684b6c member member_preview_link " data-member-id="U3B1NMZK2">khachik</a>
				<a href="/archives/betconstruct_backend/p1484947964000057" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:32 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 1:32:44 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3UJ1LL6Q" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3UJ1LL6Q" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/khachik/F3UJ1LL6Q/filetest.gif" target="https://micarmenia.slack.com/files/khachik/F3UJ1LL6Q/filetest.gif" data-file-id="F3UJ1LL6Q">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">fileTest.gif</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3UJ1LL6Q" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UJ1LL6Q-5e732b45f7/filetest_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UJ1LL6Q/filetest.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3UJ1LL6Q/filetest.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3UJ1LL6Q/filetest.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3UJ1LL6Q-5e732b45f7/filetest_360.gif" style="
					padding-top: -webkit-calc( 275 / 360 * 100%); padding-top: -moz-calc( 275 / 360 * 100%); padding-top: calc( 275 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UJ1LL6Q-5e732b45f7/filetest_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3UJ1LL6Q" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UJ1LL6Q/download/filetest.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3UJ1LL6Q" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/khachik/F3UJ1LL6Q/filetest.gif" target="https://micarmenia.slack.com/files/khachik/F3UJ1LL6Q/filetest.gif" data-file-id="F3UJ1LL6Q" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3UJ1LL6Q-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/KhachikSukiasyan/ContentOfDirectory" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FContentOfDirectory&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FContentOfDirectory&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/ContentOfDirectory" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/ContentOfDirectory</a>
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1484947964_000057_label" class="message_aria_label hidden">
			<strong>khachik</strong>.
			<a href="/team/khachik" target="/team/khachik" data-member-name="khachik" data-stringify-text="@U3B1NMZK2" class="internal_member_link">@khachik</a> uploaded a file: <a href="https://micarmenia.slack.com/files/khachik/F3UJ1LL6Q/filetest.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UJ1LL6Q">fileTest.gif</a> and commented: <a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/KhachikSukiasyan/ContentOfDirectory" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FContentOfDirectory&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FContentOfDirectory&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/ContentOfDirectory" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/ContentOfDirectory</a>.
			NaN replies
			one thirty-two AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484952030_000058" data-ts="1484952030.000058" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B45EY1E" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484952030000058">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/suren" target="/team/suren" class=" member_preview_link member_image thumb_36" data-member-id="U3B45EY1E" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B45EY1E-3e93cfe1e3db-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484952030000058" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:40 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 2:40:30 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484952030.000058" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/suren" target="/team/suren" class="message_sender color_U3B45EY1E color_df3dc0 member member_preview_link " data-member-id="U3B45EY1E">suren</a>
				<a href="/archives/betconstruct_backend/p1484952030000058" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:40 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 2:40:30 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484952030.000058" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>ես համաձայն եմ, հիմա 11:00 &nbsp;վերջնական վորոշումը?<span class="edited ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Jan 21st at 9:19 AM"> (edited)</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484952030_000058-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484952030_000058_label" class="message_aria_label hidden">
			<strong>suren</strong>.
			ես համաձայն եմ, հիմա 11:00 &nbsp;վերջնական վորոշումը?.
			NaN replies
			two forty AM. Edited.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484954161_000059" data-ts="1484954161.000059" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B1NMZK2" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484954161000059">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/khachik" target="/team/khachik" class=" member_preview_link member_image thumb_36" data-member-id="U3B1NMZK2" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B1NMZK2-64649df3e28a-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484954161000059" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:16 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 3:16:01 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484954161.000059" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/khachik" target="/team/khachik" class="message_sender color_U3B1NMZK2 color_684b6c member member_preview_link " data-member-id="U3B1NMZK2">khachik</a>
				<a href="/archives/betconstruct_backend/p1484954161000059" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:16 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 3:16:01 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484954161.000059" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/KhachikSukiasyan/FolderMonitoring" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/FolderMonitoring" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/FolderMonitoring</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/KhachikSukiasyan/FolderMonitoring">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/KhachikSukiasyan/FolderMonitoring" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/FolderMonitoring" rel="noreferrer" target="_blank">
						KhachikSukiasyan/FolderMonitoring</a>
						
					</div>

						FolderMonitoring - Checks changing of given folder
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/KhachikSukiasyan/FolderMonitoring" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/FolderMonitoring" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24527719%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484954161_000059-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484954161_000059_label" class="message_aria_label hidden">
			<strong>khachik</strong>.
			<a href="https://github.com/KhachikSukiasyan/FolderMonitoring" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FKhachikSukiasyan%2FFolderMonitoring&quot;]" data-referer-original-href="https://github.com/KhachikSukiasyan/FolderMonitoring" rel="noreferrer" target="_blank">https://github.com/KhachikSukiasyan/FolderMonitoring</a>.
			NaN replies
			three sixteen AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484982948_000003" data-ts="1484982948.000003" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B7NFX8R" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484982948000003">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/anush" target="/team/anush" class=" member_preview_link member_image thumb_36" data-member-id="U3B7NFX8R" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B7NFX8R-f9dab9170634-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484982948000003" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:15 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 11:15:48 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484982948.000003" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/anush" target="/team/anush" class="message_sender color_U3B7NFX8R color_53b759 member member_preview_link " data-member-id="U3B7NFX8R">anush</a>
				<a href="/archives/betconstruct_backend/p1484982948000003" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:15 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 11:15:48 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484982948.000003" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/AnushMv?tab=repositories" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;]" data-referer-original-href="https://github.com/AnushMv?tab=repositories" rel="noreferrer" target="_blank">https://github.com/AnushMv?tab=repositories</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/AnushMv?tab=repositories">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/AnushMv?tab=repositories" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;]" data-referer-original-href="https://github.com/AnushMv?tab=repositories" rel="noreferrer" target="_blank">
						AnushMv (Anush Movsesyan)</a>
						
					</div>

						AnushMv has 5 repositories available. Follow their code on GitHub.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/AnushMv?tab=repositories" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;]" data-referer-original-href="https://github.com/AnushMv?tab=repositories" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24522072%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24522072%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484982948_000003-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484982948_000003_label" class="message_aria_label hidden">
			<strong>anush</strong>.
			<a href="https://github.com/AnushMv?tab=repositories" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FAnushMv%3Ftab%3Drepositories&quot;]" data-referer-original-href="https://github.com/AnushMv?tab=repositories" rel="noreferrer" target="_blank">https://github.com/AnushMv?tab=repositories</a>.
			NaN replies
			eleven fifteen AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484989425_000009" data-ts="1484989425.000009" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484989425000009">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484989425000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:03 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 1:03:45 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484989425.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1484989425000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:03 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 1:03:45 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484989425.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>delegate double Function(double x);<span class="para_break"><i class="copy_only"><br></i></span> &nbsp; delegate Function Function1(double x, double y, double z);<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484989425_000009-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484989425_000009_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			delegate double Function(double x);<span class="para_break"><i class="copy_only"><br></i></span> &nbsp; delegate Function Function1(double x, double y, double z);.
			NaN replies
			one oh-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1484995757_000010" data-ts="1484995757.000010" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BNFSYSF" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484995757000010">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1484995757000010" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/meri" target="/team/meri" class=" member_preview_link member_image thumb_36" data-member-id="U3BNFSYSF" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BNFSYSF-c475b1c2e374-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1484995757000010" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:49 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 2:49:17 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1484995757.000010" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/meri" target="/team/meri" class="message_sender color_U3BNFSYSF color_99a949 member member_preview_link " data-member-id="U3BNFSYSF">meri</a>
				<a href="/archives/betconstruct_backend/p1484995757000010" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>2:49 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 2:49:17 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1484995757.000010" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>երկար քնելը լավ բան չի փաստորեն <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 55%;background-size:4100%" title="joy">:joy:</span><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 55%;background-size:4100%" title="joy">:joy:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1484995757_000010-G3B6Z0Y81 " data-rxn-key="message-1484995757.000010-G3B6Z0Y81"><span data-emoji="+1" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@tigran and @lusinekhachatryan <span class=&quot;subtle_silver&quot;>reacted with :+1:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 22.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1484995757_000010_label" class="message_aria_label hidden">
			<strong>meri</strong>.
			երկար քնելը լավ բան չի փաստորեն <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 55%;background-size:4100%" title="joy">:joy:</span><span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 55%;background-size:4100%" title="joy">:joy:</span>.
			NaN replies
			two forty-nine PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485000930_000002" data-ts="1485000930.000002" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485000930000002">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485000930000002" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>4:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 4:15:30 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485000930.000002" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1485000930000002" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>4:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 4:15:30 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485000930.000002" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> <a href="https://github.com/shtigran/IenumerableImplementation" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;]" data-referer-original-href="https://github.com/shtigran/IenumerableImplementation" rel="noreferrer" target="_blank">https://github.com/shtigran/IenumerableImplementation</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/shtigran/IenumerableImplementation">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/shtigran/IenumerableImplementation" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;]" data-referer-original-href="https://github.com/shtigran/IenumerableImplementation" rel="noreferrer" target="_blank">
						shtigran/IenumerableImplementation</a>
						
					</div>

						IenumerableImplementation - Ienumerable Implementation for User Class, Ienumerable, IEnumerator, GetEnumerator()
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/shtigran/IenumerableImplementation" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;]" data-referer-original-href="https://github.com/shtigran/IenumerableImplementation" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485000930_000002-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485000930_000002_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> <a href="https://github.com/shtigran/IenumerableImplementation" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FIenumerableImplementation&quot;]" data-referer-original-href="https://github.com/shtigran/IenumerableImplementation" rel="noreferrer" target="_blank">https://github.com/shtigran/IenumerableImplementation</a>.
			NaN replies
			four fifteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485012344_000003" data-ts="1485012344.000003" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485012344000003">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485012344000003" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485012344000003" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:25 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 7:25:44 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485012344.000003" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485012344000003" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:25 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 7:25:44 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485012344.000003" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a> &nbsp;nice idea<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485012344_000003-G3B6Z0Y81 " data-rxn-key="message-1485012344.000003-G3B6Z0Y81"><span data-emoji="wink" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@shtigran <span class=&quot;subtle_silver&quot;>reacted with :wink:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 72.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485012344_000003_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/shtigran" target="/team/shtigran" data-member-name="shtigran" data-stringify-text="@U3BEMJGFK" class="internal_member_link">@shtigran</a> &nbsp;nice idea.
			NaN replies
			seven twenty-five PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485027980_000007" data-ts="1485027980.000007" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485027980000007">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485027980000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:46 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 11:46:20 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485027980.000007" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1485027980000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:46 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Jan 21st at 11:46:20 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485027980.000007" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;is it good idea to use <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">System.Collections(.Generic)</b> everywhere we can, or it could make some problems/abuse (what kind of)??? Example: arrays...<span class="edited ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Jan 21st at 11:58 PM"> (edited)</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485027980_000007-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485027980_000007_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;is it good idea to use <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">System.Collections(.Generic)</b> everywhere we can, or it could make some problems/abuse (what kind of)??? Example: arrays....
			NaN replies
			eleven forty-six PM. Edited.
		</span>

	</div>

</ts-message>
 </div></div><div class="day_container"><div class="day_divider" id="day_divider_1485032934_000009" data-date="January 22nd, 2017" data-ts="1485032934.000009"><i class="copy_only"><br>----- </i><div class="day_divider_label" aria-label="Yesterday">Yesterday</div><i class="copy_only"> January 22nd, 2017 -----</i></div>
<div class="day_msgs" data-date="January 22nd, 2017" data-ts="1485032934.000009">

<ts-message id="msg_1485032934_000009" data-ts="1485032934.000009" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485032934000009">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485032934000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:08 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 1:08:54 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485032934.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1485032934000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:08 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 1:08:54 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485032934.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/VectorsOperatorsOverloading" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;]" data-referer-original-href="https://github.com/shtigran/VectorsOperatorsOverloading" rel="noreferrer" target="_blank">https://github.com/shtigran/VectorsOperatorsOverloading</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/shtigran/VectorsOperatorsOverloading">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/shtigran/VectorsOperatorsOverloading" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;]" data-referer-original-href="https://github.com/shtigran/VectorsOperatorsOverloading" rel="noreferrer" target="_blank">
						shtigran/VectorsOperatorsOverloading</a>
						
					</div>

						VectorsOperatorsOverloading - Operators overloading for Matematical Vectors.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/shtigran/VectorsOperatorsOverloading" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;]" data-referer-original-href="https://github.com/shtigran/VectorsOperatorsOverloading" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485032934_000009-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485032934_000009_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/VectorsOperatorsOverloading" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FVectorsOperatorsOverloading&quot;]" data-referer-original-href="https://github.com/shtigran/VectorsOperatorsOverloading" rel="noreferrer" target="_blank">https://github.com/shtigran/VectorsOperatorsOverloading</a>.
			NaN replies
			one oh-eight AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485099772_000005" data-ts="1485099772.000005" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485099772000005">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485099772000005" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:42 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 7:42:52 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485099772.000005" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485099772000005" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>7:42 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 7:42:52 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485099772.000005" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/ProjectsGroup/blob/master/integralCalculate</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb can_delete" data-attachment-id="1" data-real-src="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" rel="noreferrer" target="_blank">
						<span class="mention">VanHakobyan</span>/ProjectsGroup</a>
						
					</div>

						ProjectsGroup - BetConstruct , Projects,lessons,Vector, Smile,English,Armenian,Extension,Converter,stack,exception.File,override
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F23220521%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F23220521%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	

		<div class="delete_attachment_link" data-attachment-id="1"><ts-icon class="ts_icon_times_small"></ts-icon></div>

	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485099772_000005-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485099772_000005_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Fblob%2Fmaster%2FintegralCalculate&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/blob/master/integralCalculate" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/ProjectsGroup/blob/master/integralCalculate</a>.
			NaN replies
			seven forty-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485101520_000007" data-ts="1485101520.000007" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/aramjam/F3VFB4ETY/gif.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485101520000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:12 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 8:12:00 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3VFB4ETY" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485101520000007" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:12 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 8:12:00 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3VFB4ETY" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3VFB4ETY" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/aramjam/F3VFB4ETY/gif.gif" target="https://micarmenia.slack.com/files/aramjam/F3VFB4ETY/gif.gif" data-file-id="F3VFB4ETY">
						
						
						

							uploaded this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">@hovo</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3VFB4ETY" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VFB4ETY-cc6d963c63/gif_360.gif" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VFB4ETY/gif.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3VFB4ETY/gif.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3VFB4ETY/gif.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3VFB4ETY-cc6d963c63/gif_360.gif" style="padding-top: calc(66.9444%); background-image: url(&quot;https://files.slack.com/files-tmb/T0U4V6GA0-F3VFB4ETY-cc6d963c63/gif_360.gif&quot;);">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VFB4ETY-cc6d963c63/gif_360.gif" src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VFB4ETY-cc6d963c63/gif_360.gif">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3VFB4ETY" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VFB4ETY/download/gif.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3VFB4ETY" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/aramjam/F3VFB4ETY/gif.gif" target="https://micarmenia.slack.com/files/aramjam/F3VFB4ETY/gif.gif" data-file-id="F3VFB4ETY" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>Add Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3VFB4ETY-"></div>





		<i class="copy_only"><br></i>


		<span id="msg_1485101520_000007_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> uploaded a file: <a href="https://micarmenia.slack.com/files/aramjam/F3VFB4ETY/gif.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3VFB4ETY">@hovo</a>.
			NaN replies
			eight twelve PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485108124_000008" data-ts="1485108124.000008" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BTJ0H5K" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485108124000008">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hovo" target="/team/hovo" class=" member_preview_link member_image thumb_36" data-member-id="U3BTJ0H5K" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BTJ0H5K-7c76331c1e87-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485108124000008" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:02 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:02:04 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485108124.000008" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hovo" target="/team/hovo" class="message_sender color_U3BTJ0H5K color_4cc091 member member_preview_link " data-member-id="U3BTJ0H5K">hovo</a>
				<a href="/archives/betconstruct_backend/p1485108124000008" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:02 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:02:04 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485108124.000008" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> Its Cool//<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485108124_000008-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485108124_000008_label" class="message_aria_label hidden">
			<strong>hovo</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> Its Cool//.
			NaN replies
			ten oh-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485108427_000009" data-ts="1485108427.000009" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485108427000009">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485108427000009" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485108427000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:07 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:07:07 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485108427.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1485108427000009" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:07 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:07:07 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485108427.000009" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" rel="noreferrer" target="_blank">https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" rel="noreferrer" target="_blank">
						tigranv/Useful-examples</a>
						
					</div>

						Useful-examples - In this repository, I gathered a lot of useful examples of code that I create while studying programming. Here you can find examples on the use of the Inheritance, Interfacies, In...
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24522089%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F24522089%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485108427_000009-G3B6Z0Y81 " data-rxn-key="message-1485108427.000009-G3B6Z0Y81"><span data-emoji="heavy_check_mark" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="@aramjam <span class=&quot;subtle_silver&quot;>reacted with :heavy_check_mark:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:7.5% 87.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 ts_tip_hidden">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		<span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Add reaction...</span></span></span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485108427_000009_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Ftigranv%2FUseful-examples%2Ftree%2Fmaster%2FIntegral%2520Calculator&quot;]" data-referer-original-href="https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator" rel="noreferrer" target="_blank">https://github.com/tigranv/Useful-examples/tree/master/Integral%20Calculator</a>.
			NaN replies
			ten oh-seven PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485108996_000012" data-ts="1485108996.000012" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485108996000012">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485108996000012" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485108996000012" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:16 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:16:36 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485108996.000012" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485108996000012" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:16 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:16:36 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485108996.000012" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> &nbsp;Ինտեգրալը որպես .net -ի ֆուկցիա է?<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485108996_000012-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485108996_000012_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> &nbsp;Ինտեգրալը որպես .net -ի ֆուկցիա է?.
			NaN replies
			ten sixteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485109170_000013" data-ts="1485109170.000013" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485109170000013">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60 ts_tip_hidden"><span class="ts_tip_tip">Add reaction …</span></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485109170000013" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485109170000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:19:30 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485109170.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1485109170000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:19:30 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485109170.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> &nbsp;Չէ &nbsp;ես եմ գրել, ուղղակի ուրիշ կլասի մեջա, README - ի ներքևում &nbsp;կա<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485109170_000013-G3B6Z0Y81 " data-rxn-key="message-1485109170.000013-G3B6Z0Y81"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 user_reacted" title="You (click to remove) <span class=&quot;subtle_silver&quot;>reacted with :+1::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485109170_000013_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> &nbsp;Չէ &nbsp;ես եմ գրել, ուղղակի ուրիշ կլասի մեջա, README - ի ներքևում &nbsp;կա.
			NaN replies
			ten nineteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485112540_000015" data-ts="1485112540.000015" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485112540000015">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485112540000015" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485112540000015" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 11:15:40 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485112540.000015" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485112540000015" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 11:15:40 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485112540.000015" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/ProjectsGroup/tree/master/calculatorUsingDelegates</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb can_delete" data-attachment-id="1" data-real-src="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" rel="noreferrer" target="_blank">
						<span class="mention">VanHakobyan</span>/ProjectsGroup</a>
						
					</div>

						ProjectsGroup - BetConstruct , Projects,lessons,Vector, Smile,English,Armenian,Extension,Converter,stack,exception.File,override
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F23220521%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars1.githubusercontent.com%2Fu%2F23220521%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	

		<div class="delete_attachment_link" data-attachment-id="1"><ts-icon class="ts_icon_times_small"></ts-icon></div>

	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485112540_000015-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485112540_000015_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FVanHakobyan%2FProjectsGroup%2Ftree%2Fmaster%2FcalculatorUsingDelegates&quot;]" data-referer-original-href="https://github.com/VanHakobyan/ProjectsGroup/tree/master/calculatorUsingDelegates" rel="noreferrer" target="_blank">https://github.com/<span class="mention">VanHakobyan</span>/ProjectsGroup/tree/master/calculatorUsingDelegates</a>.
			NaN replies
			eleven fifteen PM.
		</span>

	</div>

</ts-message>
 </div></div><div class="day_container"><div class="day_divider" id="day_divider_1485115210_000017" data-date="January 23rd, 2017" data-ts="1485115210.000017"><i class="copy_only"><br>----- </i><div class="day_divider_label" aria-label="Today">Today</div><i class="copy_only"> January 23rd, 2017 -----</i></div>
<div class="day_msgs" data-date="January 23rd, 2017" data-ts="1485115210.000017">

<ts-message id="msg_1485115210_000017" data-ts="1485115210.000017" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="comment" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add comment …"></a><a data-action="share_file" data-permalink="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share file …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485115210000017" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:00 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 12:00:10 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3U5NT5B3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1485115210000017" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:00 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 12:00:10 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3U5NT5B3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3U5NT5B3" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" target="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" data-file-id="F3U5NT5B3">
						
						
						

							added and commented on this C# snippet<span class="msg_inline_file_title_hider">:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Untitled</span>
							</span>

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							

<div data-file-id="F3U5NT5B3" class="file_container snippet_container
				inline_collapsed
">

	<div class="file_body snippet_body">
			<div class="CodeMirror cm-s-default CodeMirrorServer" oncopy="if(event.clipboardData){event.clipboardData.setData('text/plain',window.getSelection().toString().replace(/\u200b/g,''));event.preventDefault();event.stopPropagation();}">
<div class="CodeMirror-code">
<div><pre>  <span class="cm-variable">st</span>: <span class="cm-variable-3">string</span> <span class="cm-variable">st</span> <span class="cm-operator">=</span> <span class="cm-variable">Console</span>.<span class="cm-variable">ReadLine</span>();</pre></div>
<div><pre>​</pre></div>
<div><pre>            <span class="cm-keyword">if</span> (<span class="cm-variable">st</span> <span class="cm-operator">!=</span> <span class="cm-string">"+"</span> <span class="cm-operator">&amp;&amp;</span> <span class="cm-variable">st</span> <span class="cm-operator">!=</span> <span class="cm-string">"*"</span> <span class="cm-operator">&amp;&amp;</span> <span class="cm-variable">st</span> <span class="cm-operator">!=</span> <span class="cm-string">"-"</span> <span class="cm-operator">&amp;&amp;</span> <span class="cm-variable">st</span> <span class="cm-operator">!=</span> <span class="cm-string">"/"</span>)</pre></div>
<div><pre>            {</pre></div>
<div><pre>                <span class="cm-variable">Console</span>.<span class="cm-variable">WriteLine</span>(<span class="cm-string">"false symbols write again"</span>);</pre></div>
</div>
</div>

	</div>

		
		
		<div class="preview_actions">
			<a class="file_preview_action preview_show_less_header btn btn_outline btn_icon ts_icon ts_icon_collapse_vertical ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Collapse"></a>
		
			<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3U5NT5B3" href="https://files.slack.com/files-pri/T0U4V6GA0-F3U5NT5B3/download/-.cs" target="new_1485198992132" title="Download"></a>
		
			
		
						<a class="file_preview_action file_new_window_link btn btn_outline btn_icon ts_icon ts_icon_external_link ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3U5NT5B3" href="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" target="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" title="Open in new window"></a>
			<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3U5NT5B3" data-include-open-flexpane="true" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
			<a href="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" target="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" data-file-id="F3U5NT5B3" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
				<span>1 Comment</span>
			</a>
		</div>
		 		
		
			<div class="preview_show preview_show_more">
				<div class="preview_show_center">
					<button class="preview_show_btn" data-file-id="F3U5NT5B3">
						<i class="ts_icon ts_icon_plus_small"></i>Click to expand inline
						<span class="line_count">7 lines</span>
					</button>
				</div>
			</div>
			<div class="preview_show preview_show_less">
				<button class="preview_show_btn">Collapse<i class="ts_icon ts_icon_arrow_up_medium"></i></button>
			</div>
		 
</div>


 
							
							
							
							
					<div class="rxn_panel rxns_key_file-F3U5NT5B3- " data-rxn-key="file-F3U5NT5B3-"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 user_reacted" title="You (click to remove) <span class=&quot;subtle_silver&quot;>reacted with :+1::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> &nbsp;instead of goto(bad practice) use do-while
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1485115210_000017_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/tigran/F3U5NT5B3/-.cs" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3U5NT5B3">Untitled</a> and commented: <a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> &nbsp;instead of goto(bad practice) use do-while.
			NaN replies
			midnight.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485121206_000018" data-ts="1485121206.000018" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B45EY1E" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/suren/F3VGY8CCF/files_delete.gif">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/suren" target="/team/suren" class=" member_preview_link member_image thumb_36" data-member-id="U3B45EY1E" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B45EY1E-3e93cfe1e3db-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485121206000018" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:40 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 1:40:06 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3VGY8CCF" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/suren" target="/team/suren" class="message_sender color_U3B45EY1E color_df3dc0 member member_preview_link " data-member-id="U3B45EY1E">suren</a>
				<a href="/archives/betconstruct_backend/p1485121206000018" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:40 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 1:40:06 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3VGY8CCF" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3VGY8CCF" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/suren/F3VGY8CCF/files_delete.gif" target="https://micarmenia.slack.com/files/suren/F3VGY8CCF/files_delete.gif" data-file-id="F3VGY8CCF">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Files delete</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3VGY8CCF" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VGY8CCF-77710ae24e/files_delete_720.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VGY8CCF/files_delete.gif" target="https://files.slack.com/files-pri/T0U4V6GA0-F3VGY8CCF/files_delete.gif" style="width: 360px;" class="file_body image_body image_gif
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3VGY8CCF/files_delete.gif" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3VGY8CCF-77710ae24e/files_delete_720.png" style="padding-top: calc(56.3889%); background-image: url(&quot;https://files.slack.com/files-tmb/T0U4V6GA0-F3VGY8CCF-77710ae24e/files_delete_720.png&quot;);">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VGY8CCF-77710ae24e/files_delete_720.png" src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VGY8CCF-77710ae24e/files_delete_720.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3VGY8CCF" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VGY8CCF/download/files_delete.gif" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3VGY8CCF" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/suren/F3VGY8CCF/files_delete.gif" target="https://micarmenia.slack.com/files/suren/F3VGY8CCF/files_delete.gif" data-file-id="F3VGY8CCF" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3VGY8CCF-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							Ուշացումով
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1485121206_000018_label" class="message_aria_label hidden">
			<strong>suren</strong>.
			<a href="/team/suren" target="/team/suren" data-member-name="suren" data-stringify-text="@U3B45EY1E" class="internal_member_link">@suren</a> uploaded a file: <a href="https://micarmenia.slack.com/files/suren/F3VGY8CCF/files_delete.gif" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3VGY8CCF">Files delete</a> and commented: Ուշացումով.
			NaN replies
			one forty AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485121787_000019" data-ts="1485121787.000019" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485121787000019">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485121787000019" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:49 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 1:49:47 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485121787.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1485121787000019" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>1:49 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 1:49:47 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485121787.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> could you please tell what is the difference delegate1+=delegate2 and Delegate.Combine(delegate1, delegate2)? first one is working, second one not <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 52.5%;background-size:4100%" title="grin">:grin:</span> example is here... &nbsp;<a href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" rel="noreferrer" target="_blank">https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" rel="noreferrer" target="_blank">
						harutyunyanhayk/ForTest</a>
						
					</div>

						Contribute to ForTest development by creating an account on GitHub.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F19515285%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F19515285%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485121787_000019-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485121787_000019_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> could you please tell what is the difference delegate1+=delegate2 and Delegate.Combine(delegate1, delegate2)? first one is working, second one not <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 52.5%;background-size:4100%" title="grin">:grin:</span> example is here... &nbsp;<a href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fharutyunyanhayk%2FForTest%2Fblob%2Fmaster%2FDelegateTests%2FDelegateTests%2FCar.cs&quot;]" data-referer-original-href="https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs" rel="noreferrer" target="_blank">https://github.com/harutyunyanhayk/ForTest/blob/master/DelegateTests/DelegateTests/Car.cs</a>.
			NaN replies
			one forty-nine AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485154370_000003" data-ts="1485154370.000003" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485154370000003">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485154370000003" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485154370000003" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:52 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:52:50 AM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485154370.000003" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1485154370000003" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:52 AM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:52:50 AM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485154370.000003" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/MyDictionary" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;]" data-referer-original-href="https://github.com/shtigran/MyDictionary" rel="noreferrer" target="_blank">https://github.com/shtigran/MyDictionary</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/shtigran/MyDictionary">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/shtigran/MyDictionary" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;]" data-referer-original-href="https://github.com/shtigran/MyDictionary" rel="noreferrer" target="_blank">
						shtigran/MyDictionary</a>
						
					</div>

						MyDictionary Class, Dictionary, System.Collections, Generics
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/shtigran/MyDictionary" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;]" data-referer-original-href="https://github.com/shtigran/MyDictionary" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars2.githubusercontent.com%2Fu%2F24455154%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485154370_000003-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485154370_000003_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;<a href="https://github.com/shtigran/MyDictionary" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2Fshtigran%2FMyDictionary&quot;]" data-referer-original-href="https://github.com/shtigran/MyDictionary" rel="noreferrer" target="_blank">https://github.com/shtigran/MyDictionary</a>.
			NaN replies
			ten fifty-two AM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485161579_000005" data-ts="1485161579.000005" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485161579000005">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485161579000005" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485161579000005" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:52 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 12:52:59 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485161579.000005" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1485161579000005" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>12:52 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 12:52:59 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485161579.000005" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://github.com/LusineHovs/DelegatesExamples" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;]" data-referer-original-href="https://github.com/LusineHovs/DelegatesExamples" rel="noreferrer" target="_blank">https://github.com/LusineHovs/DelegatesExamples</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone has_thumb" data-attachment-id="1" data-real-src="https://github.com/LusineHovs/DelegatesExamples">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fgithub.com%2Fapple-touch-icon.png" alt=""></span>

					<span class="attachment_source_name">GitHub</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://github.com/LusineHovs/DelegatesExamples" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;]" data-referer-original-href="https://github.com/LusineHovs/DelegatesExamples" rel="noreferrer" target="_blank">
						LusineHovs/DelegatesExamples</a>
						
					</div>

						Contribute to DelegatesExamples development by creating an account on GitHub.
					<span class="media_caret"></span>
			</div>





	</div>

	
		<div class="msg_inline_attachment_column column_thumb">
			<div class="msg_inline_attachment_row">
				<a href="https://github.com/LusineHovs/DelegatesExamples" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;]" data-referer-original-href="https://github.com/LusineHovs/DelegatesExamples" rel="noreferrer" target="_blank">
				<div class="msg_inline_attachment_thumb_holder" style="background-image: url(https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24455176%3Fv%3D3%26s%3D400);">
					<img class="msg_inline_attachment_thumb" src="https://slack-imgs.com/?c=1&amp;o1=wi75.he75&amp;url=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F24455176%3Fv%3D3%26s%3D400" alt="">
				</div>
				</a>
			</div>
		</div>
	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485161579_000005-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485161579_000005_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			<a href="https://github.com/LusineHovs/DelegatesExamples" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgithub.com%2FLusineHovs%2FDelegatesExamples&quot;]" data-referer-original-href="https://github.com/LusineHovs/DelegatesExamples" rel="noreferrer" target="_blank">https://github.com/LusineHovs/DelegatesExamples</a>.
			NaN replies
			zero fifty-two PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485170947_000008" data-ts="1485170947.000008" data-model-ob-id="G3B6Z0Y81" data-member-id="U0U59721F" class="message feature_fix_files first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485170947000008">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Start a thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485170947000008" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_36" data-member-id="U0U59721F" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485170947000008" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:29 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 3:29:07 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485170947.000008" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class="message_sender color_U0U59721F color_9f69e7 member member_preview_link " data-member-id="U0U59721F">aghasi.lorsabyan</a>
				<a href="/archives/betconstruct_backend/p1485170947000008" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>3:29 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 3:29:07 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485170947.000008" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;]" data-referer-original-href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" rel="noreferrer" target="_blank">http://dotnetcrunch.com/list-of-c-new-features-by-version/</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone" data-attachment-id="1" data-real-src="http://dotnetcrunch.com/wp-content/uploads/2016/09/csharp-new-features-by-version.png">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fi1.wp.com%2Fdotnetcrunch.com%2Fwp-content%2Fuploads%2F2016%2F08%2F1471381675_d-single-letter-circle-chat-brand.png%3Ffit%3D180%252C180" alt=""></span>

					<span class="attachment_source_name">DotNetCrunch</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;]" data-referer-original-href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" rel="noreferrer" target="_blank">
						List of C# new features version by version - DotNetCrunch</a>
						
					</div>

						List of C# new features by version, c# features by version, c# new features, evolution of c#, list of all the versions of c# and it's features, c#7, c#7.0
					<span class="media_caret"><span class="inline_img_bytes "> (20KB)</span><i data-real-src="http://dotnetcrunch.com/wp-content/uploads/2016/09/csharp-new-features-by-version.png" class="msg_inline_img_collapser ts_icon ts_icon_caret_down "></i><i data-real-src="http://dotnetcrunch.com/wp-content/uploads/2016/09/csharp-new-features-by-version.png" class="msg_inline_img_expander ts_icon ts_icon_caret_right hidden"></i></span>
			</div>


			<div class="msg_inline_attachment_row attachment_flush_text attachment_footer">
				<span class="attachment_ts">Jan 17th at 8:12 PM</span>
				
				
			</div>

			<div class="msg_inline_attachment_row attachment_media">
				
				<div data-real-src="http://dotnetcrunch.com/wp-content/uploads/2016/09/csharp-new-features-by-version.png" class="clear_both msg_inline_img_holder msg_inline_holder msg_inline_holder_rounded file_container_fixed_dimensions"><a href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;]" data-referer-original-href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" rel="noreferrer" target="_blank" title="" class="file_viewer_external_link" data-src="http://dotnetcrunch.com/wp-content/uploads/2016/09/csharp-new-features-by-version.png" data-link-url="http://dotnetcrunch.com/list-of-c-new-features-by-version/" data-width="444" data-height="250"><div class="msg_inline_img_container"><div class="file_preview_preserve_aspect_ratio" style="width: 400px; height: 225px;"><figure class="msg_inline_img msg_inline_child" data-real-background-image="https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fdotnetcrunch.com%2Fwp-content%2Fuploads%2F2016%2F09%2Fcsharp-new-features-by-version.png" style="background-image: url(&quot;https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fdotnetcrunch.com%2Fwp-content%2Fuploads%2F2016%2F09%2Fcsharp-new-features-by-version.png&quot;);"><img data-real-src="https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fdotnetcrunch.com%2Fwp-content%2Fuploads%2F2016%2F09%2Fcsharp-new-features-by-version.png" src="https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fdotnetcrunch.com%2Fwp-content%2Fuploads%2F2016%2F09%2Fcsharp-new-features-by-version.png"></figure></div></div></a></div></div>


	</div>

	


	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485170947_000008-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485170947_000008_label" class="message_aria_label hidden">
			<strong>aghasi.lorsabyan</strong>.
			<a href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fdotnetcrunch.com%2Flist-of-c-new-features-by-version%2F&quot;]" data-referer-original-href="http://dotnetcrunch.com/list-of-c-new-features-by-version/" rel="noreferrer" target="_blank">http://dotnetcrunch.com/list-of-c-new-features-by-version/</a>.
			NaN replies
			three twenty-nine PM.
		</span>

	</div>

</ts-message>
 



<ts-message id="msg_1485180411_000010" data-ts="1485180411.000010" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485180411000010" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:06 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:06:51 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485180411000010" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:06 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:06:51 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3UD77DB3" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf" target="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf" data-file-id="F3UD77DB3">
						
						
						

							uploaded and commented on this file<span class="msg_inline_file_title_hider">:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">VanikHakobyanResume 2017.pdf</span>
							</span>

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							

<div class="file_container generic_container">

	<a data-file-id="F3UD77DB3" target="new_1485198992132" class="file_header generic_header  file_viewer_channel_link file_viewer_link" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UD77DB3/vanikhakobyanresume_2017.pdf">

		<i class="file_header_icon generic_header_icon filetype_icon pdf s48">
					<i class="ts_icon ts_icon_search_small pdf"></i>
		</i>

		<h4 class="file_header_title generic_header_title overflow_ellipsis">VanikHakobyanResume 2017.pdf</h4>

		<p class="file_header_meta generic_header_meta">
				<span class="meta_size">131KB</span><span class="meta_hover_placement">
				<span class="meta_type overflow_ellipsis">PDF</span>

			<span class="meta_hover overflow_ellipsis">
							Click to view
			</span></span>
		</p>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3UD77DB3" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UD77DB3/download/vanikhakobyanresume_2017.pdf" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3UD77DB3" data-include-open-flexpane="true" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf" target="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf" data-file-id="F3UD77DB3" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>2 Comments</span>
					</a>
				</div>
				 

</div>
 
							
							
					<div class="rxn_panel rxns_key_file-F3UD77DB3- " data-rxn-key="file-F3UD77DB3-"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 " title="@aramjam and @gayane <span class=&quot;subtle_silver&quot;>reacted with :+1::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							էս կանֆետի թուղթա?
						</div>
						<div class="rxn_panel rxns_key_file_comment-Fc3UD77GQZ-"></div>
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1485180411_000010_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> uploaded a file: <a href="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UD77DB3">VanikHakobyanResume 2017.pdf</a> and commented: էս կանֆետի թուղթա?.
			NaN replies
			six oh-six PM.
		</span>

	</div>

</ts-message>
 
 



<ts-message id="msg_1485181681_000012" data-ts="1485181681.000012" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first file_reference file_share comment_continuation" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485181681000012">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485181681000012" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:28 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:28:01 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-comment-id="Fc3UCPR2L8" data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
						<span class="meta message_commented">commented:</span>
				<a href="/archives/betconstruct_backend/p1485181681000012" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:28 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:28:01 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-comment-id="Fc3UCPR2L8" data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
					
			</div>
				
		</div>








					<div class="comment">
						how did you do that?
					</div>
					<div class="rxn_panel rxns_key_file_comment-Fc3UCPR2L8-"></div>



		<i class="copy_only"><br></i>


		<span id="msg_1485181681_000012_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> commented on <a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a>’s file <a href="https://micarmenia.slack.com/files/vanhakobyan/F3UD77DB3/vanikhakobyanresume_2017.pdf" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UD77DB3">VanikHakobyanResume 2017.pdf</a>: how did you do that?.
			NaN replies
			six twenty-eight PM.
		</span>

	</div>

</ts-message>
 
 

<ts-message id="msg_1485181718_000013" data-ts="1485181718.000013" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="">
		<div class="action_hover_container stretch_btn_heights narrow_buttons" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485181718000013">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="reply" class="ts_icon ts_icon_comment_alt ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Reply to thread"></a><a data-action="share_message" data-permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485181718000013" class="ts_icon ts_icon_share_action ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Share message …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485181718000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:28 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:28:38 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485181718.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485181718000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>6:28 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:28:38 PM</span></span></span></a>
					
				

					
					<span class="message_star_holder">

<button data-msg-id="1485181718.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://enhancv.com/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fenhancv.com%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fenhancv.com%2F&quot;]" data-referer-original-href="https://enhancv.com/" rel="noreferrer" target="_blank">https://enhancv.com/</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone can_delete" data-attachment-id="1" data-real-src="https://enhancv.com/">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fenhancv.com%2Fimg%2Ffavicon.29f993c1.png" alt=""></span>

					<span class="attachment_source_name">enhancv.com</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://enhancv.com/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fenhancv.com%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fenhancv.com%2F&quot;]" data-referer-original-href="https://enhancv.com/" rel="noreferrer" target="_blank">
						Enhancv</a>
						
					</div>

						Enhancv helps you create compelling human-centric resumes that unveil the real person behind.
					<span class="media_caret"></span>
			</div>





	</div>

	

		<div class="delete_attachment_link" data-attachment-id="1"><ts-icon class="ts_icon_times_small"></ts-icon></div>

	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				





						<div class="rxn_panel rxns_key_message-1485181718_000013-G3B6Z0Y81 " data-rxn-key="message-1485181718.000013-G3B6Z0Y81"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 " title="@aramjam and @gayane <span class=&quot;subtle_silver&quot;>reacted with :+1::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						

<div class="reply_bar">
	<div class="reply_faces">
					<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_24" data-member-id="U3CD6J85V" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-24')" aria-hidden="true"></a>
	
					<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_24" data-member-id="U3B5F2125" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-24')" aria-hidden="true"></a>
	
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_24" data-member-id="U0U59721F" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-24')" aria-hidden="true"></a>
	
	</div>	<div class="reply_summary">
		<a href="/conversation/betconstruct_backend/p1485181718000013" target="_blank" class="reply_count">
			5 replies
		</a>

		<div class="meta_hover_placement">
			<span class="last_reply_at">Last reply today at 7:50 PM</span>
			<span class="view_conv_hover">View thread</span>
		</div>
	</div>
	<ts-icon class="reply_bar_caret ts_icon_chevron_right"></ts-icon>
</div>
 





		<i class="copy_only"><br></i>


		<span id="msg_1485181718_000013_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="https://enhancv.com/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fenhancv.com%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fenhancv.com%2F&quot;]" data-referer-original-href="https://enhancv.com/" rel="noreferrer" target="_blank">https://enhancv.com/</a>.
						5 replies
			5 replies
			six twenty-eight PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485188677_000037" data-ts="1485188677.000037" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485188677000037">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485188677000037" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:24 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:24:37 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485188677.000037" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485188677000037" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:24 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:24:37 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485188677.000037" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> jan, can you, please, tell us what should we write in technical skills section? I mean, I can write only C# in language field, nothing else.<br><a href="https://gyazo.com/180be84bebb89b54bf71945706e3a994" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgyazo.com%2F180be84bebb89b54bf71945706e3a994&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgyazo.com%2F180be84bebb89b54bf71945706e3a994&quot;]" data-referer-original-href="https://gyazo.com/180be84bebb89b54bf71945706e3a994" rel="noreferrer" target="_blank">https://gyazo.com/180be84bebb89b54bf71945706e3a994</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone" data-attachment-id="1" data-real-src="https://bot.gyazo.com/180be84bebb89b54bf71945706e3a994.png">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><a href="https://gyazo.com" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgyazo.com&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgyazo.com&quot;]" data-referer-original-href="https://gyazo.com" rel="noreferrer" target="_blank"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16.ip&amp;url=https%3A%2F%2Fgyazo.com%2Ffavicon.ico" alt=""></a></span>

					<span class="attachment_source_name"><a href="https://gyazo.com" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgyazo.com&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgyazo.com&quot;]" data-referer-original-href="https://gyazo.com" rel="noreferrer" target="_blank">Gyazo</a></span>



				<span class="media_caret"><span class="inline_img_bytes "> (24KB)</span><i data-real-src="https://bot.gyazo.com/180be84bebb89b54bf71945706e3a994.png" class="msg_inline_img_collapser ts_icon ts_icon_caret_down "></i><i data-real-src="https://bot.gyazo.com/180be84bebb89b54bf71945706e3a994.png" class="msg_inline_img_expander ts_icon ts_icon_caret_right hidden"></i></span>
			</div>




			<div class="msg_inline_attachment_row attachment_media">
				
				<div data-real-src="https://bot.gyazo.com/180be84bebb89b54bf71945706e3a994.png" class="clear_both msg_inline_img_holder msg_inline_holder msg_inline_holder_rounded file_container_fixed_dimensions"><a href="https://gyazo.com/180be84bebb89b54bf71945706e3a994" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgyazo.com%2F180be84bebb89b54bf71945706e3a994&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgyazo.com%2F180be84bebb89b54bf71945706e3a994&quot;]" data-referer-original-href="https://gyazo.com/180be84bebb89b54bf71945706e3a994" rel="noreferrer" target="_blank" title="" class="file_viewer_external_link" data-src="https://bot.gyazo.com/180be84bebb89b54bf71945706e3a994.png" data-link-url="https://gyazo.com/180be84bebb89b54bf71945706e3a994" data-width="886" data-height="168"><div class="msg_inline_img_container"><div class="file_preview_preserve_aspect_ratio" style="width: 400px; height: 75px;"><figure class="msg_inline_img msg_inline_child" data-real-background-image="https://slack-imgs.com/?c=1&amp;url=https%3A%2F%2Fbot.gyazo.com%2F180be84bebb89b54bf71945706e3a994.png" style="background-image: url(&quot;https://slack-imgs.com/?c=1&amp;url=https%3A%2F%2Fbot.gyazo.com%2F180be84bebb89b54bf71945706e3a994.png&quot;);"><img data-real-src="https://slack-imgs.com/?c=1&amp;url=https%3A%2F%2Fbot.gyazo.com%2F180be84bebb89b54bf71945706e3a994.png" src="https://slack-imgs.com/?c=1&amp;url=https%3A%2F%2Fbot.gyazo.com%2F180be84bebb89b54bf71945706e3a994.png"></figure></div></div></a></div></div>


	</div>

	


	

</div>

 
	</div>
	
<span class="edited ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Today at 8:25 PM"> (edited)</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485188677_000037-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485188677_000037_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> jan, can you, please, tell us what should we write in technical skills section? I mean, I can write only C# in language field, nothing else.<br><a href="https://gyazo.com/180be84bebb89b54bf71945706e3a994" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fgyazo.com%2F180be84bebb89b54bf71945706e3a994&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fgyazo.com%2F180be84bebb89b54bf71945706e3a994&quot;]" data-referer-original-href="https://gyazo.com/180be84bebb89b54bf71945706e3a994" rel="noreferrer" target="_blank">https://gyazo.com/180be84bebb89b54bf71945706e3a994</a>.
			NaN replies
			eight twenty-four PM. Edited.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485188835_000040" data-ts="1485188835.000040" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485188835000040">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485188835000040" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="light_only">8:27</span><span class="dense_only">8:27 PM</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:27:15 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485188835.000040" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485188835000040" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:27 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:27:15 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485188835.000040" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>well, this one too <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><br>Operating systems: Windows XP and Windows 8<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485188835_000040-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485188835_000040_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			well, this one too <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><br>Operating systems: Windows XP and Windows 8.
			NaN replies
			eight twenty-seven PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485189405_000041" data-ts="1485189405.000041" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1485189405.000041" data-parent-user-id="">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485189405000041">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485189405000041" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:36:45 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485189405.000041" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485189405000041" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:36 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:36:45 PM</span></span></span></a>
					
				

					
					<span class="message_star_holder">

<button data-msg-id="1485189405.000041" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> &nbsp;maybe should not write OS<span class="constrain_triple_clicks"></span></span>

				





						<div class="rxn_panel rxns_key_message-1485189405_000041-G3B6Z0Y81"></div>
						

<div class="reply_bar">
	<div class="reply_faces">
					<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_24" data-member-id="U3CD6J85V" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-24')" aria-hidden="true"></a>
	
					<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_24" data-member-id="U3B5F2125" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-24')" aria-hidden="true"></a>
	
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_24" data-member-id="U3BR8V9PE" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-24')" aria-hidden="true"></a>
	
	</div>	<div class="reply_summary">
		<a href="/conversation/betconstruct_backend/p1485189405000041" target="_blank" class="reply_count">
			12 replies
		</a>

		<div class="meta_hover_placement">
			<span class="last_reply_at">Last reply today at 9:11 PM</span>
			<span class="view_conv_hover">View thread</span>
		</div>
	</div>
	<ts-icon class="reply_bar_caret ts_icon_chevron_right"></ts-icon>
</div>
 





		<i class="copy_only"><br></i>


		<span id="msg_1485189405_000041_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> &nbsp;maybe should not write OS.
						12 replies
			12 replies
			eight thirty-six PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485189831_000052" data-ts="1485189831.000052" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/vanhakobyan/F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485189831000052" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:43 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:43:51 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3VSU2HU7" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485189831000052" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:43 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:43:51 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3VSU2HU7" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3VSU2HU7" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" data-file-id="F3VSU2HU7">
						
						
						

							uploaded this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Pasted image at 2017-01-23, 8:43 PM</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3VSU2HU7" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VSU2HU7-74e034eebc/pasted_image_at_2017_01_23_08_43_pm_720.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" target="https://files.slack.com/files-pri/T0U4V6GA0-F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" style="width: 360px;" class="file_body image_body image_png
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3VSU2HU7-74e034eebc/pasted_image_at_2017_01_23_08_43_pm_720.png" style="
					padding-top: -webkit-calc( 182 / 360 * 100%); padding-top: -moz-calc( 182 / 360 * 100%); padding-top: calc( 182 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VSU2HU7-74e034eebc/pasted_image_at_2017_01_23_08_43_pm_720.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3VSU2HU7" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VSU2HU7/download/pasted_image_at_2017_01_23_08_43_pm.png" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3VSU2HU7" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" data-file-id="F3VSU2HU7" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>Add Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3VSU2HU7-"></div>





		<i class="copy_only"><br></i>


		<span id="msg_1485189831_000052_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> uploaded a file: <a href="https://micarmenia.slack.com/files/vanhakobyan/F3VSU2HU7/pasted_image_at_2017_01_23_08_43_pm.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3VSU2HU7">Pasted image at 2017-01-23, 8:43 PM</a>.
			NaN replies
			eight forty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485189970_000055" data-ts="1485189970.000055" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1485189970.000055" data-parent-user-id="">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485189970000055">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485189970000055" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:46 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:46:10 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485189970.000055" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485189970000055" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>8:46 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 8:46:10 PM</span></span></span></a>
					
				

					
					<span class="message_star_holder">

<button data-msg-id="1485189970.000055" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> պարզ ու հասկանալի <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span><span class="edited ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Today at 8:46 PM"> (edited)</span><span class="constrain_triple_clicks"></span></span>

				





						<div class="rxn_panel rxns_key_message-1485189970_000055-G3B6Z0Y81"></div>
						

<div class="reply_bar">
	<div class="reply_faces">
					<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_24" data-member-id="U3B5F2125" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-24')" aria-hidden="true"></a>
	
					<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_24" data-member-id="U3CD6J85V" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-24')" aria-hidden="true"></a>
	
						<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_24" data-member-id="U3BSURBNW" data-thumb-size="24" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-24')" aria-hidden="true"></a>
	
	</div>	<div class="reply_summary">
		<a href="/conversation/betconstruct_backend/p1485189970000055" target="_blank" class="reply_count">
			4 replies
		</a>

		<div class="meta_hover_placement">
			<span class="last_reply_at">Last reply today at 8:56 PM</span>
			<span class="view_conv_hover">View thread</span>
		</div>
	</div>
	<ts-icon class="reply_bar_caret ts_icon_chevron_right"></ts-icon>
</div>
 





		<i class="copy_only"><br></i>


		<span id="msg_1485189970_000055_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> պարզ ու հասկանալի <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span>.
						4 replies
			4 replies
			eight forty-six PM. Edited.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191363_000077" data-ts="1485191363.000077" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191363000077">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191363000077" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:09 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:09:23 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191363.000077" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485191363000077" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:09 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:09:23 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191363.000077" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><b class="mention">@channel</b> who knows, shall we insert a photo on the CV or not?<span class="edited ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="Today at 9:09 PM"> (edited)</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191363_000077-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191363_000077_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<b class="mention">@channel</b> who knows, shall we insert a photo on the CV or not?.
			NaN replies
			nine oh-nine PM. Edited.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191660_000081" data-ts="1485191660.000081" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CCUK1JA" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191660000081">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/narekye" target="/team/narekye" class=" member_preview_link member_image thumb_36" data-member-id="U3CCUK1JA" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CCUK1JA-9befd71c7192-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191660000081" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:14 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:14:20 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191660.000081" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/narekye" target="/team/narekye" class="message_sender color_U3CCUK1JA color_e96699 member member_preview_link " data-member-id="U3CCUK1JA">narekye</a>
				<a href="/archives/betconstruct_backend/p1485191660000081" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:14 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:14:20 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191660.000081" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a>: on right up corner<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191660_000081-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191660_000081_label" class="message_aria_label hidden">
			<strong>narekye</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a>: on right up corner.
			NaN replies
			nine fourteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191739_000082" data-ts="1485191739.000082" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191739000082">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191739000082" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:15:39 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191739.000082" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485191739000082" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:15:39 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191739.000082" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/narekye" target="/team/narekye" data-member-name="narekye" data-stringify-text="@U3CCUK1JA" class="internal_member_link">@narekye</a> is it optional or obligatory?<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191739_000082-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191739_000082_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/narekye" target="/team/narekye" data-member-name="narekye" data-stringify-text="@U3CCUK1JA" class="internal_member_link">@narekye</a> is it optional or obligatory?.
			NaN replies
			nine fifteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191741_000083" data-ts="1485191741.000083" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191741000083">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191741000083" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:15:41 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191741.000083" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1485191741000083" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:15 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:15:41 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191741.000083" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>its not necessary<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191741_000083-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191741_000083_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			its not necessary.
			NaN replies
			nine fifteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191779_000084" data-ts="1485191779.000084" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files dirty_hover_container" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191779000084">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191779000084" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="light_only">9:16</span><span class="dense_only">9:16 PM</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:16:19 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191779.000084" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1485191779000084" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:16 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:16:19 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191779.000084" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>mainly people dont put pic<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191779_000084-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191779_000084_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			mainly people dont put pic.
			NaN replies
			nine sixteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191858_000085" data-ts="1485191858.000085" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CCUK1JA" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191858000085">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/narekye" target="/team/narekye" class=" member_preview_link member_image thumb_36" data-member-id="U3CCUK1JA" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CCUK1JA-9befd71c7192-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191858000085" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:17 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:17:38 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191858.000085" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/narekye" target="/team/narekye" class="message_sender color_U3CCUK1JA color_e96699 member member_preview_link " data-member-id="U3CCUK1JA">narekye</a>
				<a href="/archives/betconstruct_backend/p1485191858000085" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:17 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:17:38 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191858.000085" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a>: by own wish, it isnt obligatory <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 72.5%;background-size:4100%" title="wink">:wink:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191858_000085-G3B6Z0Y81 " data-rxn-key="message-1485191858.000085-G3B6Z0Y81"><span data-emoji="ok_hand::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 " title="@aramjam <span class=&quot;subtle_silver&quot;>reacted with :ok_hand::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 10%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191858_000085_label" class="message_aria_label hidden">
			<strong>narekye</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a>: by own wish, it isnt obligatory <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 72.5%;background-size:4100%" title="wink">:wink:</span>.
			NaN replies
			nine seventeen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191871_000086" data-ts="1485191871.000086" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CCUK1JA" class="message feature_fix_files dirty_hover_container" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191871000086">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/narekye" target="/team/narekye" class=" member_preview_link member_image thumb_36" data-member-id="U3CCUK1JA" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CCUK1JA-9befd71c7192-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191871000086" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="light_only">9:17</span><span class="dense_only">9:17 PM</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:17:51 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191871.000086" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/narekye" target="/team/narekye" class="message_sender color_U3CCUK1JA color_e96699 member member_preview_link " data-member-id="U3CCUK1JA">narekye</a>
				<a href="/archives/betconstruct_backend/p1485191871000086" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:17 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:17:51 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191871.000086" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a>: which redactor you use?<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191871_000086-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191871_000086_label" class="message_aria_label hidden">
			<strong>narekye</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a>: which redactor you use?.
			NaN replies
			nine seventeen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191886_000088" data-ts="1485191886.000088" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191886000088">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191886000088" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:18 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:18:06 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191886.000088" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485191886000088" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:18 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:18:06 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191886.000088" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>Microsoft Word<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191886_000088-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191886_000088_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			Microsoft Word.
			NaN replies
			nine eighteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191887_000089" data-ts="1485191887.000089" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191887000089">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191887000089" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="light_only">9:18</span><span class="dense_only">9:18 PM</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:18:07 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191887.000089" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485191887000089" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:18 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:18:07 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191887.000089" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><span class="emoji-outer emoji-sizer emoji-only" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191887_000089-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191887_000089_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<span class="emoji-outer emoji-sizer emoji-only" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			nine eighteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191930_000090" data-ts="1485191930.000090" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CCUK1JA" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485191930000090">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/narekye" target="/team/narekye" class=" member_preview_link member_image thumb_36" data-member-id="U3CCUK1JA" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CCUK1JA-9befd71c7192-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191930000090" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:18 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:18:50 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485191930.000090" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/narekye" target="/team/narekye" class="message_sender color_U3CCUK1JA color_e96699 member member_preview_link " data-member-id="U3CCUK1JA">narekye</a>
				<a href="/archives/betconstruct_backend/p1485191930000090" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:18 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:18:50 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485191930.000090" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> : <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485191930_000090-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485191930_000090_label" class="message_aria_label hidden">
			<strong>narekye</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> : <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			nine eighteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485191972_000091" data-ts="1485191972.000091" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/aramjam/F3UGMRQ1X/aram_cv_in_english_230117.docx">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485191972000091" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:19:32 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3UGMRQ1X" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<a href="/archives/betconstruct_backend/p1485191972000091" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:19 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:19:32 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3UGMRQ1X" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3UGMRQ1X" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/aramjam/F3UGMRQ1X/aram_cv_in_english_230117.docx" target="https://micarmenia.slack.com/files/aramjam/F3UGMRQ1X/aram_cv_in_english_230117.docx" data-file-id="F3UGMRQ1X">
						
						
						

							uploaded this file<span class="msg_inline_file_title_hider">:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Aram CV in english 230117.docx</span>
							</span>

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							

<div class="file_container generic_container">

	<a data-file-id="F3UGMRQ1X" target="new_1485198992132" class="file_header generic_header file_ssb_download_link " href="https://files.slack.com/files-pri/T0U4V6GA0-F3UGMRQ1X/download/aram_cv_in_english_230117.docx">

		<i class="file_header_icon generic_header_icon filetype_icon docx s48">
				<i class="ts_icon ts_icon_arrow_down docx"></i>
		</i>

		<h4 class="file_header_title generic_header_title overflow_ellipsis">Aram CV in english 230117.docx</h4>

		<p class="file_header_meta generic_header_meta">
				<span class="meta_hover_placement"><span class="meta_type overflow_ellipsis">Word Document</span>

			<span class="meta_hover overflow_ellipsis">
						Click to download
			</span></span>
		</p>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3UGMRQ1X" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UGMRQ1X/download/aram_cv_in_english_230117.docx" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3UGMRQ1X" data-include-open-flexpane="true" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/aramjam/F3UGMRQ1X/aram_cv_in_english_230117.docx" target="https://micarmenia.slack.com/files/aramjam/F3UGMRQ1X/aram_cv_in_english_230117.docx" data-file-id="F3UGMRQ1X" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>Add Comment</span>
					</a>
				</div>
				 

</div>
 
							
							
					<div class="rxn_panel rxns_key_file-F3UGMRQ1X- " data-rxn-key="file-F3UGMRQ1X-"><span data-emoji="+1" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 user_reacted" title="@narekye and you <span class=&quot;subtle_silver&quot;>reacted with :+1:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 22.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>





		<i class="copy_only"><br></i>


		<span id="msg_1485191972_000091_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<a href="/team/aramjam" target="/team/aramjam" data-member-name="aramjam" data-stringify-text="@U3CD6J85V" class="internal_member_link">@aramjam</a> uploaded a file: <a href="https://micarmenia.slack.com/files/aramjam/F3UGMRQ1X/aram_cv_in_english_230117.docx" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UGMRQ1X">Aram CV in english 230117.docx</a>.
			NaN replies
			nine nineteen PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485192067_000093" data-ts="1485192067.000093" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485192067000093" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:21 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:21:07 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3UGNMG8H" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485192067000093" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:21 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:21:07 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3UGNMG8H" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3UGNMG8H" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" data-file-id="F3UGNMG8H">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Pasted image at 2017-01-23, 9:20 PM</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 360px;">

	<a data-file-id="F3UGNMG8H" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UGNMG8H-51a76e7fdd/pasted_image_at_2017_01_23_09_20_pm_720.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" target="https://files.slack.com/files-pri/T0U4V6GA0-F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" style="width: 360px;" class="file_body image_body image_png
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3UGNMG8H-51a76e7fdd/pasted_image_at_2017_01_23_09_20_pm_720.png" style="
					padding-top: -webkit-calc( 133 / 360 * 100%); padding-top: -moz-calc( 133 / 360 * 100%); padding-top: calc( 133 / 360 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3UGNMG8H-51a76e7fdd/pasted_image_at_2017_01_23_09_20_pm_720.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3UGNMG8H" href="https://files.slack.com/files-pri/T0U4V6GA0-F3UGNMG8H/download/pasted_image_at_2017_01_23_09_20_pm.png" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3UGNMG8H" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" data-file-id="F3UGNMG8H" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>2 Comments</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3UGNMG8H-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							Մոտավոր տեսքը
						</div>
						<div class="rxn_panel rxns_key_file_comment-Fc3V9H8AVA-"></div>
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1485192067_000093_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> uploaded a file: <a href="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UGNMG8H">Pasted image at 2017-01-23, 9:20 PM</a> and commented: Մոտավոր տեսքը.
			NaN replies
			nine twenty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485192103_000094" data-ts="1485192103.000094" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CCUK1JA" class="message feature_fix_files dirty_hover_container first file_reference file_share comment_continuation" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485192103000094">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/narekye" target="/team/narekye" class=" member_preview_link member_image thumb_36" data-member-id="U3CCUK1JA" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CCUK1JA-9befd71c7192-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485192103000094" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:21 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:21:43 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-comment-id="Fc3V9TKNLD" data-file-id="F3UGNMG8H" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/narekye" target="/team/narekye" class="message_sender color_U3CCUK1JA color_e96699 member member_preview_link " data-member-id="U3CCUK1JA">narekye</a>
						<span class="meta message_commented">commented:</span>
				<a href="/archives/betconstruct_backend/p1485192103000094" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:21 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:21:43 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-comment-id="Fc3V9TKNLD" data-file-id="F3UGNMG8H" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
					
			</div>
				
		</div>








					<div class="comment">
						<span class="emoji-outer emoji-sizer emoji-only" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span>
					</div>
					<div class="rxn_panel rxns_key_file_comment-Fc3V9TKNLD-"></div>



		<i class="copy_only"><br></i>


		<span id="msg_1485192103_000094_label" class="message_aria_label hidden">
			<strong>narekye</strong>.
			<a href="/team/narekye" target="/team/narekye" data-member-name="narekye" data-stringify-text="@U3CCUK1JA" class="internal_member_link">@narekye</a> commented on <a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a>’s file <a href="https://micarmenia.slack.com/files/vanhakobyan/F3UGNMG8H/pasted_image_at_2017_01_23_09_20_pm.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3UGNMG8H">Pasted image at 2017-01-23, 9:20 PM</a>: <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span>.
			NaN replies
			nine twenty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485193887_000096" data-ts="1485193887.000096" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/vanhakobyan/F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485193887000096" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:51 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:51:27 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3VTREV38" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485193887000096" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:51 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:51:27 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3VTREV38" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3VTREV38" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" data-file-id="F3VTREV38">
						
						
						

							uploaded and commented on this image:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Pasted image at 2017-01-23, 9:50 PM</span>
							

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							
							

<div class="file_container image_container" style="width: 216px;">

	<a data-file-id="F3VTREV38" data-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VTREV38-c3f6dadd5f/pasted_image_at_2017_01_23_09_50_pm_360.png" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" target="https://files.slack.com/files-pri/T0U4V6GA0-F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" style="width: 216px;" class="file_body image_body image_png
			file_viewer_channel_link file_viewer_link" data-link-url="https://files.slack.com/files-pri/T0U4V6GA0-F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" title="ctrl+click to open original in new tab">

		<div class="image_preserve_aspect_ratio">
			<figure class="image_bg" data-real-background-image="https://files.slack.com/files-tmb/T0U4V6GA0-F3VTREV38-c3f6dadd5f/pasted_image_at_2017_01_23_09_50_pm_360.png" style="
					padding-top: -webkit-calc( 271 / 216 * 100%); padding-top: -moz-calc( 271 / 216 * 100%); padding-top: calc( 271 / 216 * 100%);
">

				<img class="image_hide" data-real-src="https://files.slack.com/files-tmb/T0U4V6GA0-F3VTREV38-c3f6dadd5f/pasted_image_at_2017_01_23_09_50_pm_360.png">

			</figure>
		</div>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3VTREV38" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VTREV38/download/pasted_image_at_2017_01_23_09_50_pm.png" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3VTREV38" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/vanhakobyan/F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" target="https://micarmenia.slack.com/files/vanhakobyan/F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" data-file-id="F3VTREV38" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 
</div>
 
							
					<div class="rxn_panel rxns_key_file-F3VTREV38-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							սենց բան հազարից մեկա լինում ՖԻՔՍԵՆՔ
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1485193887_000096_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" data-member-name="vanhakobyan" data-stringify-text="@U3B5F2125" class="internal_member_link"><span class="mention">@vanhakobyan</span></a> uploaded a file: <a href="https://micarmenia.slack.com/files/vanhakobyan/F3VTREV38/pasted_image_at_2017_01_23_09_50_pm.png" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3VTREV38">Pasted image at 2017-01-23, 9:50 PM</a> and commented: սենց բան հազարից մեկա լինում ՖԻՔՍԵՆՔ.
			NaN replies
			nine fifty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485194081_000097" data-ts="1485194081.000097" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BS7F6H0" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/tigran/F3VTTCBDL/cv_tigran_vardanyan.pdf">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/tigran" target="/team/tigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BS7F6H0" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BS7F6H0-db1f2d179132-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485194081000097" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:54 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:54:41 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3VTTCBDL" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/tigran" target="/team/tigran" class="message_sender color_U3BS7F6H0 color_db3150 member member_preview_link " data-member-id="U3BS7F6H0">tigran</a>
				<a href="/archives/betconstruct_backend/p1485194081000097" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>9:54 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 9:54:41 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3VTTCBDL" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3VTTCBDL" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/tigran/F3VTTCBDL/cv_tigran_vardanyan.pdf" target="https://micarmenia.slack.com/files/tigran/F3VTTCBDL/cv_tigran_vardanyan.pdf" data-file-id="F3VTTCBDL">
						
						
						

							uploaded and commented on this file<span class="msg_inline_file_title_hider">:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">CV Tigran Vardanyan.pdf</span>
							</span>

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							

<div class="file_container generic_container">

	<a data-file-id="F3VTTCBDL" target="new_1485198992132" class="file_header generic_header  file_viewer_channel_link file_viewer_link" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VTTCBDL/cv_tigran_vardanyan.pdf">

		<i class="file_header_icon generic_header_icon filetype_icon pdf s48">
					<i class="ts_icon ts_icon_search_small pdf"></i>
		</i>

		<h4 class="file_header_title generic_header_title overflow_ellipsis">CV Tigran Vardanyan.pdf</h4>

		<p class="file_header_meta generic_header_meta">
				<span class="meta_size">280KB</span><span class="meta_hover_placement">
				<span class="meta_type overflow_ellipsis">PDF</span>

			<span class="meta_hover overflow_ellipsis">
							Click to view
			</span></span>
		</p>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3VTTCBDL" href="https://files.slack.com/files-pri/T0U4V6GA0-F3VTTCBDL/download/cv_tigran_vardanyan.pdf" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3VTTCBDL" data-include-open-flexpane="true" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/tigran/F3VTTCBDL/cv_tigran_vardanyan.pdf" target="https://micarmenia.slack.com/files/tigran/F3VTTCBDL/cv_tigran_vardanyan.pdf" data-file-id="F3VTTCBDL" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>1 Comment</span>
					</a>
				</div>
				 

</div>
 
							
							
					<div class="rxn_panel rxns_key_file-F3VTTCBDL-"></div>


					<div class="initial_comment">
						<div class="comment no_bottom_margin">
							<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;ok?
						</div>
						
					</div>



		<i class="copy_only"><br></i>


		<span id="msg_1485194081_000097_label" class="message_aria_label hidden">
			<strong>tigran</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> uploaded a file: <a href="https://micarmenia.slack.com/files/tigran/F3VTTCBDL/cv_tigran_vardanyan.pdf" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3VTTCBDL">CV Tigran Vardanyan.pdf</a> and commented: <a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> &nbsp;ok?.
			NaN replies
			nine fifty-four PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485194493_000098" data-ts="1485194493.000098" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485194493000098">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485194493000098" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:01 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:01:33 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485194493.000098" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485194493000098" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:01 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:01:33 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485194493.000098" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> &nbsp;միանգամից կարելի էր wikipedia-ում հավաքել <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 57.5%;background-size:4100%" title="smiley">:smiley:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485194493_000098-G3B6Z0Y81 " data-rxn-key="message-1485194493.000098-G3B6Z0Y81"><span data-emoji="grimacing" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 " title="@tigran <span class=&quot;subtle_silver&quot;>reacted with :grimacing:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:67.5% 57.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="1"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485194493_000098_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="/team/tigran" target="/team/tigran" data-member-name="tigran" data-stringify-text="@U3BS7F6H0" class="internal_member_link">@tigran</a> &nbsp;միանգամից կարելի էր wikipedia-ում հավաքել <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 57.5%;background-size:4100%" title="smiley">:smiley:</span>.
			NaN replies
			ten oh-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485195699_000100" data-ts="1485195699.000100" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BSURBNW" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485195699000100">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/lusine" target="/team/lusine" class=" member_preview_link member_image thumb_36" data-member-id="U3BSURBNW" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BSURBNW-f11792280621-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485195699000100" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:21 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:21:39 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485195699.000100" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/lusine" target="/team/lusine" class="message_sender color_U3BSURBNW color_235e5b member member_preview_link " data-member-id="U3BSURBNW">lusine</a>
				<a href="/archives/betconstruct_backend/p1485195699000100" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:21 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:21:39 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485195699.000100" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>Guys who has FineReader?<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485195699_000100-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485195699_000100_label" class="message_aria_label hidden">
			<strong>lusine</strong>.
			Guys who has FineReader?.
			NaN replies
			ten twenty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485196486_000101" data-ts="1485196486.000101" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container first" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485196486000101">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485196486000101" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:34 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:34:46 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485196486.000101" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1485196486000101" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:34 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:34:46 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485196486.000101" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/lusine" target="/team/lusine" data-member-name="lusine" data-stringify-text="@U3BSURBNW" class="internal_member_link">@lusine</a> &nbsp;I have<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485196486_000101-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485196486_000101_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/lusine" target="/team/lusine" data-member-name="lusine" data-stringify-text="@U3BSURBNW" class="internal_member_link">@lusine</a> &nbsp;I have.
			NaN replies
			ten thirty-four PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485196504_000102" data-ts="1485196504.000102" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BEMJGFK" class="message feature_fix_files dirty_hover_container" data-selectable="true">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="true" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485196504000102">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/shtigran" target="/team/shtigran" class=" member_preview_link member_image thumb_36" data-member-id="U3BEMJGFK" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BEMJGFK-2bb2a3ad9e7f-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485196504000102" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="light_only">10:35</span><span class="dense_only">10:35 PM</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:35:04 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-msg-id="1485196504.000102" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/shtigran" target="/team/shtigran" class="message_sender color_U3BEMJGFK color_50a0cf member member_preview_link " data-member-id="U3BEMJGFK">shtigran</a>
				<a href="/archives/betconstruct_backend/p1485196504000102" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>10:35 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 10:35:04 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485196504.000102" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="/team/lusine" target="/team/lusine" data-member-name="lusine" data-stringify-text="@U3BSURBNW" class="internal_member_link">@lusine</a> &nbsp;what need ?<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485196504_000102-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485196504_000102_label" class="message_aria_label hidden">
			<strong>shtigran</strong>.
			<a href="/team/lusine" target="/team/lusine" data-member-name="lusine" data-stringify-text="@U3BSURBNW" class="internal_member_link">@lusine</a> &nbsp;what need ?.
			NaN replies
			ten thirty-five PM.
		</span>

	</div>

</ts-message>

<div id="msgs_unread_divider" class="unread_divider no_unreads">
	<hr role="separator" aria-hidden="true">
	<span class="divider_label">
			NEW MESSAGES
	</span>
</div>
 
 

<ts-message id="msg_1485198855_000103" data-ts="1485198855.000103" data-model-ob-id="G3B6Z0Y81" data-member-id="U3BR8V9PE" class="message feature_fix_files dirty_hover_container first file_reference file_share" data-selectable="false">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="true" data-abs_permalink="https://micarmenia.slack.com/files/hayk.harutyunyan/F3W054QH5/hayk_harutyunyan_cv.pdf">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class=" member_preview_link member_image thumb_36" data-member-id="U3BR8V9PE" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3BR8V9PE-aeb52f0bf749-48')" aria-hidden="true"></a>
				
			</div>
			<a href="/archives/betconstruct_backend/p1485198855000103" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:14 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 11:14:15 PM</span></span></span></a>
			<span class="message_star_holder">

<button data-file-id="F3W054QH5" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" class="message_sender color_U3BR8V9PE color_2b6836 member member_preview_link " data-member-id="U3BR8V9PE">hayk.harutyunyan</a>
				<a href="/archives/betconstruct_backend/p1485198855000103" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i>11:14 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 11:14:15 PM</span></span></span></a>
					

 
				

					
					<span class="message_star_holder">

<button data-file-id="F3W054QH5" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 </span>
					
			</div>
				
		</div>


				<span data-file-id="F3W054QH5" class="meta message_body  msg_inline_file_preview_toggler expanded">
					<a href="https://micarmenia.slack.com/files/hayk.harutyunyan/F3W054QH5/hayk_harutyunyan_cv.pdf" target="https://micarmenia.slack.com/files/hayk.harutyunyan/F3W054QH5/hayk_harutyunyan_cv.pdf" data-file-id="F3W054QH5">
						
						
						

							uploaded this file<span class="msg_inline_file_title_hider">:
								<span class="file_preview_link no_jumbomoji file_force_flexpane bold msg_inline_file_preview_title">Hayk Harutyunyan CV.pdf</span>
							</span>

								<ts-icon class="msg_inline_media_toggler"></ts-icon>
					</a>
				</span>




							
							
							

<div class="file_container generic_container">

	<a data-file-id="F3W054QH5" target="new_1485198992132" class="file_header generic_header  file_viewer_channel_link file_viewer_link" href="https://files.slack.com/files-pri/T0U4V6GA0-F3W054QH5/hayk_harutyunyan_cv.pdf">

		<i class="file_header_icon generic_header_icon filetype_icon pdf s48">
					<i class="ts_icon ts_icon_search_small pdf"></i>
		</i>

		<h4 class="file_header_title generic_header_title overflow_ellipsis">Hayk Harutyunyan CV.pdf</h4>

		<p class="file_header_meta generic_header_meta">
				<span class="meta_size">495KB</span><span class="meta_hover_placement">
				<span class="meta_type overflow_ellipsis">PDF</span>

			<span class="meta_hover overflow_ellipsis">
							Click to view
			</span></span>
		</p>

	</a>

				
				
				<div class="preview_actions">
					
				
					<a class="file_preview_action file_ssb_download_link btn btn_outline btn_icon ts_icon ts_icon_cloud_download ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" data-file-id="F3W054QH5" href="https://files.slack.com/files-pri/T0U4V6GA0-F3W054QH5/download/hayk_harutyunyan_cv.pdf" target="new_1485198992132" title="Download"></a>
				
					
				
					<a class="file_preview_action file_actions btn btn_outline btn_icon ts_icon ts_icon_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_300" title="More actions" data-file-id="F3W054QH5" data-include-open-flexpane="true" data-exclude-comment="true" data-exclude-print="true" data-include-view-public-link="true" data-exclude-download="true"></a>
					<a href="https://micarmenia.slack.com/files/hayk.harutyunyan/F3W054QH5/hayk_harutyunyan_cv.pdf" target="https://micarmenia.slack.com/files/hayk.harutyunyan/F3W054QH5/hayk_harutyunyan_cv.pdf" data-file-id="F3W054QH5" class="file_preview_action btn btn_outline file_preview_link file_comment_link file_force_flexpane">
						<span>Add Comment</span>
					</a>
				</div>
				 

</div>
 
							
							
					<div class="rxn_panel rxns_key_file-F3W054QH5-"></div>





		<i class="copy_only"><br></i>


		<span id="msg_1485198855_000103_label" class="message_aria_label hidden">
			<strong>hayk.harutyunyan</strong>.
			<a href="/team/hayk.harutyunyan" target="/team/hayk.harutyunyan" data-member-name="hayk.harutyunyan" data-stringify-text="@U3BR8V9PE" class="internal_member_link">@hayk.harutyunyan</a> uploaded a file: <a href="https://micarmenia.slack.com/files/hayk.harutyunyan/F3W054QH5/hayk_harutyunyan_cv.pdf" target="_blank" class="no_jumbomoji file_preview_link" data-file-id="F3W054QH5">Hayk Harutyunyan CV.pdf</a>.
			NaN replies
			eleven fourteen PM.
		</span>

	</div>

</ts-message>
 </div></div></div>
						<div id="msgs_overlay_div" class="hidden" style="opacity: 0;"></div>

					</div>

					<div id="messages_unread_status" class="messages_banner quiet no_pointer_events no_opacity flex_pane_showing">
						<ts-icon class="new_msgs_arrow ts_icon_arrow_up hidden" aria-hidden="true"></ts-icon>						<span class="actual new_msgs_jump_link" style="display: none;">Jump</span>
						<span id="new_msg_info" class="overflow_ellipsis">1 new message since 11:14 PM</span>
						<a role="button" class="clear_unread_messages ts_tip ts_tip_bottom ts_tip_right" onclick="TS.client.ui.forceMarkAllRead(TS.model.marked_reasons.clicked); return false;" data-original-title="" title="">
							<span class="ts_tip_tip">Mark as read (esc)</span>
							<span class="clear_unread_messages_text">Mark as read</span> <ts-icon class="ts_icon_times_small float_right" aria-hidden="true"></ts-icon>						</a>
					</div>

					<div id="file_progress" class="messages_banner hidden flex_pane_showing">
						<div class="progress_bar">
							<span class="progress_bar_progress_thin progress_bar_progress_striped"></span>
						</div>
						<div id="progress_text"></div>
					</div>

					<div id="connection_div" class="messages_banner hidden flex_pane_showing" role="status" aria-live="assertive" aria-atomic="true"></div>

					<div id="archives_return" class="messages_banner messages_banner_bottom hidden flex_pane_showing" style="top: 519px;">
						<span id="archives_info" class="overflow_ellipsis">Viewing archives from <span id="archives_return_date" class=""></span></span>
						<a role="button" class="cancel_archives hidden">Jump to recent messages <ts-icon class="ts_icon_arrow_down float_right" aria-hidden="true"></ts-icon></a>
					</div>

											<div id="threads_view_banner" class="messages_banner hidden no_opacity flex_pane_showing">
							<ts-icon class="new_msgs_arrow ts_icon_arrow_up"></ts-icon>
							<span class="actual new_msgs_jump_link">Jump</span>
							<span id="new_replies_info" class="overflow_ellipsis"></span>
							<a class="clear_unread_messages ts_tip ts_tip_bottom ts_tip_right" data-original-title="" title="">
								<span class="ts_tip_tip">Mark as read (esc)</span>
								<ts-icon class="ts_icon_times_small float_right"></ts-icon>
							</a>
						</div>
									</div>

		</div>

	
	<div id="col_flex">

		<div id="flex_contents" role="complementary" class="tab_panels tab_container" style="opacity: 100;">

		
		
			<div class="panel" id="stars_tab" style="height: 609px;">
									<div class="heading" tabindex="-1">
						<div class="heading_row">
							<h2 class="heading_text overflow_ellipsis">Starred Items</h2>
							<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
						</div>
					</div>
				
				<div id="stars_scroller" class="flex_content_scroller">
					<div class="selectable_flex_pane_padder">
						<div id="member_stars_list"></div>
						<div id="member_stars_explanation" class="hidden help">
							<p>You haven't starred any messages or files yet. Maybe now's the time to start? You can add a star to messages, files, snippets, posts, comments … pretty much anything in Slack.</p>
							<p>Starring makes things easier to find: they'll show up right here in this list.</p>						</div>
						<div id="member_stars_more" class="flexpane_load_more">
							<button id="member_stars_more_btn" class="btn btn_outline ladda-button flexpane_load_more_btn" data-spinner-color="#000" data-style="expand-right"><span class="ladda-label">Load more…</span></button>
						</div>
						<div id="member_stars_error" class="flexpane_load_error hidden">
							<p class="flexpane_load_error_msg">We're having trouble loading your Starred Items.</p>
							<button id="member_stars_error_btn" class="btn btn_outline ladda-button flexpane_load_more_btn" data-spinner-color="#000" data-style="expand-right"><span class="ladda-label">Try again?</span></button>						</div>
					</div>
				</div>
			</div>

			<div class="panel" id="mentions_tab" style="height: 609px;">
				<div class="heading" tabindex="-1">
											<div class="heading_row">
							<h2 class="heading_text overflow_ellipsis">Activity</h2>
							<span id="mentions_spinner"></span>
							<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
							<div id="mentions_clear_notifications_container" class="hidden"><button id="mentions_clear_notifications" class="btn_unstyle">Clear notifications</button></div>						</div>
									</div>
				<div id="mentions_options" class="subheading feature_message_replies_simple"></div>
				<div id="mentions_scroller" class="flex_content_scroller">
					<div class="selectable_flex_pane_padder">
						<div id="member_mentions" class="feature_message_replies_simple"></div>
						<div id="member_mentions_explanation" class="hidden help">
							<p>You don't have any mentions yet. When someone mentions you by name or uses one of your highlight words, that message will appear here.</p>
						</div>
						<div id="member_mentions_more" class="flexpane_load_more">
							<button id="member_mentions_more_btn" class="btn btn_outline ladda-button" data-spinner-color="#000" data-style="expand-right"><span class="ladda-label">Load more…</span></button>
						</div>
					</div>
				</div>
			</div>

			<div class="panel" id="files_tab" style="height: 609px;">
				<div id="file_list_container">
					<div class="heading" tabindex="-1">
													<div class="heading_row">
								<button id="file_list_clear_filter" class="menu_icon btn_link hidden" type="button">
									<i class="ts_icon ts_icon_times_circle"></i>
								</button>
								<h2 class="heading_text overflow_ellipsis">
									<button id="file_list_heading" class="btn_link" type="button">
										<span class="heading_label">All File Types</span>
										<i class="ts_icon ts_icon_caret_down"></i>
									</button>
								</h2>
								<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
							</div>
											</div>
					<div class="toolbar_container">
						<div class="toolbar clearfix">
							<ul id="file_list_toggle" class="flexpane_tab_bar">
								<li id="file_list_toggle_all" class="active"><a role="button">Everyone</a></li>
								<li id="file_list_toggle_user">
									<i id="file_list_toggle_users" class="ts_icon ts_icon_caret_down"></i>
									<a role="button">Just You</a>
								</li>
							</ul>
						</div>
					</div>
					<div id="file_list_scroller" class="flex_content_scroller">
												<div id="file_list" class="feature_fast_files_flexpane not_scrolling" data-list="all"></div>
						<div id="file_list_block" class="help">
							<div class="subsection" data-filter="all">
								<p>Files live in channels, but you can search and sort them here.</p>
																	<p>
																		To add a file, click the <ts-icon class="ts_icon_plus_square_o ts_icon_inherit ts_icon_align_bottom" aria-hidden="true"></ts-icon> in any channel.									</p>
															</div>
							<div class="subsection hidden" data-filter="posts">
								<p>Posts are useful for sharing longer documents with your team: information that's longer than a chat message or that needs to be formatted. Posts have the same commenting and sharing functionality as other files.</p>
								<p>If you'd like, you can <a href="/files/create/post" target="new">create a new post</a>.</p>							</div>
							<div class="subsection hidden" data-filter="spaces">
								<p>Posts are useful for sharing longer documents with your team: information that's longer than a chat message or that needs to be formatted. Posts have the same commenting and sharing functionality as other files.</p>
								<p>If you'd like, you can <a href="/files/create/space" target="new">create a new post</a>.</p>							</div>
							<div class="subsection hidden" data-filter="snippets">
								<p>Snippets are useful for pasting code or large blocks of text into Slack. Snippets can be shared into channels so your teammates can add comments.</p>
								<p>Like other files, all content in a snippet is indexed and searchable. Snippet content will appear in the Files tab of search results.</p>
								<p>If you'd like, you can <a role="button" onclick="TS.ui.snippet_dialog.startCreate();">create a new Snippet</a>.</p>							</div>
							<div class="subsection hidden" data-filter="images">
								<p>All sorts of image files can be uploaded to Slack. When you share an image file, it can be previewed inline in chat.</p>
								<p>If you'd like, you can <a role="button" onclick="TS.client.ui.files.$upload.trigger('click');">upload a new image</a>.</p>							</div>
							<div class="subsection hidden" data-filter="pdfs">
								<p>PDFs uploaded to Slack are indexed and searchable. PDF content will appear in the Files tab of search results.</p>
								<p>If you'd like, you can <a role="button" onclick="TS.client.ui.files.$upload.trigger('click');">upload a new PDF document</a>.</p>							</div>
							<div class="subsection hidden" data-filter="gdocs">
								<p>Slack provides built-in support for Google Docs. Just paste in a link to a Google Doc and follow the prompts to set it up.</p>
								<p>When you add a Google Doc, Slack will index it for search and keep it up to date automatically so any changes you make in Google Docs will be reflected here.</p>							</div>
							<a href="/files" target="new" id="file_listing_bottom_button" class="top_margin btn full_width">Open Files Archive</a>
						</div>
					</div>
				</div>

									<div id="file_preview_container" class="hidden">
						<div class="heading">
															<div class="heading_row">
									<h2 class="heading_text overflow_ellipsis">
																				<button id="back_from_file_preview" class="btn_link" type="button"><i class="ts_icon ts_icon_chevron_medium_left back_icon"></i> Files</button>
									</h2>
									<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
								</div>
													</div>

						<div id="file_preview_scroller" class="flex_content_scroller">
							<div id="file_preview_head_section"></div>
							<div id="file_preview_comments_section"></div>
							



						</div>
					</div>
				
			</div>
			<div class="panel" id="team_tab" style="height: 609px;">
							  		<div id="team_list_container">
						<div class="heading" tabindex="-1">
															<div class="heading_row">
									<h2 class="heading_text overflow_ellipsis">Directory</h2>
									<div id="flannel_team_dir_loading"><div class="infinite_spinner infinite_spinner_small">
	<svg class="infinite_spinner_spinner infinite_spinner_fast" viewBox="0 0 100 100">
		<circle class="infinite_spinner_bg" cx="50%" cy="50%" r="35"></circle>
		<circle class="infinite_spinner_path infinite_spinner_blue" cx="50%" cy="50%" r="35"></circle>
	</svg>
	<svg class="infinite_spinner_spinner infinite_spinner_tail infinite_spinner_fast" viewBox="0 0 100 100">
		<circle class="infinite_spinner_path infinite_spinner_blue" cx="50%" cy="50%" r="35"></circle>
	</svg>
</div></div>									<a id="team_list_admin_link" href="/admin" class="ts_tip ts_tip_bottom float_right right_margin hidden"><span class="ts_tip_tip">Manage team<br>members</span><ts-icon class="ts_icon_cog_o"></ts-icon></a>
									<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
								</div>
													</div>

						<div class="team_tabs_container clearfix no_bottom_border">
							<div id="team_tabs"></div>
						</div>
						<div id="team_list_scroller" class="flex_content_scroller">
							<div id="team_list_members_wrapper">
								
							</div>
							<div id="team_block" class="hidden help">

								<p id="team_block_admin_invite_few" class="hidden">There aren't many people here: you should <a href="/admin/invites" target="_blank">invite some</a>!</p>

								<p id="team_block_admin_invite_many" class="hidden">Is everyone on your team already on Slack? If not, <a href="/admin/invites" target="_blank">send them an invite!</a></p>

								<p id="team_block_description" class="hidden">
									The directory is an easy way to find contact details, start direct message conversations and view individual team members’ activity feeds.								</p>

								<p id="team_block_email_on" class="hidden">Anyone with an <span id="team_block_email_domains"></span> email address will be able to join automatically if you send them a link to <a href="https://micarmenia.slack.com">https://micarmenia.slack.com</a>.</p>

								<p id="team_block_admin_email_off" class="hidden">To make it easier, you can <a href="/admin/settings#signup_mode" target="_blank">change your settings</a> to allow anyone with a work email address (at a domain of your choice) to sign up by themselves by visiting <strong>https://micarmenia.slack.com</strong>.</p>

								<div id="team_block_fill_prompt" class="hidden">
									<i class="ts_icon ts_icon_user callout" style="float: left; margin: 0 1rem 1rem 0;"></i>
									<p>To make it easier for your colleagues, we suggest you <a href="/account/profile" target="_blank">add some details to your profile</a> (such as your phone number, Skype name and your role on the team).</p>
								</div>

							</div>
						</div>
					</div>
					<div id="member_preview_container" class="hidden">
						<div class="heading">
															<div class="heading_row">
									<h2 class="heading_text overflow_ellipsis">
										<button id="back_from_member_preview" class="btn_link" type="button"><i class="ts_icon ts_icon_chevron_medium_left back_icon"></i> Directory</button>
									</h2>
									<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
								</div>
													</div>
						<div id="member_preview_scroller" class="flex_content_scroller"></div>
					</div>
					<div id="user_group_preview_container" class="hidden">
						<div class="heading">
															<div class="heading_row">
									<h2 class="heading_text overflow_ellipsis">
										<button id="back_from_user_group_preview" class="btn_link" type="button"><i class="ts_icon ts_icon_chevron_medium_left back_icon"></i> Directory</button>
									</h2>
									<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
								</div>
													</div>

						<div id="user_group_preview_scroller"></div>
					</div>
						  	</div>
						<div class="panel" id="search_tab" style="height: 609px;">
				<div id="search_results_container">
					<div class="heading" tabindex="-1">
													<div class="heading_row">
								<h2 id="search_heading" class="heading_text overflow_ellipsis">Search Results</h2>

								<div class="search_sort_container very_small_right_margin">
																	<a id="search_sort_timestamp" class="search_segmented_control left active" onclick="TS.search.setSort('timestamp');">Recent</a><a id="search_sort_score" class="search_segmented_control right" onclick="TS.search.setSort('score');">Relevant</a>
																								</div>

								<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
							</div>
											</div>
					<div id="search_tabs" class="lato">
	<div id="search_filters" class="messages">
		<a id="filter_messages" onclick="TS.search.setFilter('messages'); return false;">Messages (0)</a>
		<a id="filter_files" onclick="TS.search.setFilter('files'); return false;">Files (0)</a>
	</div>

 </div>
					<div id="search_options" class="subheading"></div>
					<div id="search_results" class="flex_content_scroller">
						<div id="search_results_team"></div>
												<div id="search_results_items"></div>
						
					</div>
				</div>
			</div>
			<div class="panel" id="details_tab" style="height: 609px;">
				<div class="heading" tabindex="-1">
											<div class="heading_row">
							<h2 id="details_tab_header" class="heading_text overflow_ellipsis">Channel Info</h2>
							<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
						</div>
									</div>
			

	<div id="channel_page_scroller" class="flex_content_scroller">

		<div class="selectable_flex_pane_padder no_top_margin">

			<div class="conversation_details"></div>

			<div class="channel_page_about channel_page_section " data-section-name="about">

				<div class="section_header no_bottom_margin display_flex align_items_center">
					<i class="ts_icon ts_icon_info channel_page_blue small_right_margin"></i>
					<a id="channel_page_title" title="Click to expand or collapse" class="flex_one"></a>

					<div class="disclosure_triangle inline_block left_margin">
						<i class="ts_icon ts_icon_caret_right"></i>
						<i class="ts_icon ts_icon_caret_down"></i>
					</div>
				</div>

				<div class="section_content channel_purpose"></div>

			</div>

			<div class="channel_page_pinned_items channel_page_section expanded" data-section-name="pinned_items">

				<div class="section_header no_bottom_margin display_flex align_items_center">
					<i class="ts_icon ts_icon_thumb_tack pin_orange small_right_margin"></i>
					<a title="Click to expand or collapse" class="flex_one" id="pinned_items_title"></a>

					<div class="disclosure_triangle inline_block left_margin">
						<i class="ts_icon ts_icon_caret_right"></i>
						<i class="ts_icon ts_icon_caret_down"></i>
					</div>
				</div>

				<div class="section_content pinned_items"></div>

			</div>

			<div class="channel_page_members channel_page_section expanded" data-section-name="members">
				<div class="channel_page_member_tabs section_header"></div>
				<div class="channel_page_member_lists section_content"></div>
			</div>

			<div class="channel_page_shared_files channel_page_section " data-section-name="shared_files">

			<div class="section_header no_bottom_margin display_flex align_items_center">
				<i class="ts_icon ts_icon_all_files mustard_yellow small_right_margin"></i>
				<a title="Click to expand or collapse" class="flex_one" id="channel_files_title">Shared Files</a>

				<div class="disclosure_triangle inline-block left_margin">
					<i class="ts_icon ts_icon_caret_right"></i>
					<i class="ts_icon ts_icon_caret_down"></i>
				</div>
			</div>

			<div class="section_content bottom_margin"></div>

			</div>

			<div class="channel_page_notif_prefs channel_page_section " data-section-name="notif_prefs">

				<div class="section_header no_bottom_margin display_flex align_items_center">
					<span class="channel_page_notif_prefs_mute_state">
						<i class="ts_icon ts_icon_bell_o moscow_red small_right_margin"></i>
					</span>
					<a id="channel_notif_prefs_title" title="Click to expand or collapse" class="flex_one">Notification Preferences</a>

					<div class="disclosure_triangle inline_block left_margin">
						<i class="ts_icon ts_icon_caret_right"></i>
						<i class="ts_icon ts_icon_caret_down"></i>
					</div>
				</div>

				<div class="section_content"></div>
			</div>

		</div>

	</div>

</div>
			<div class="panel" id="downloads_tab" style="height: 609px;">
				<div class="heading" tabindex="-1">
											<div class="heading_row">
							<h2 id="downloads_tab_header" class="heading_text overflow_ellipsis">Downloads</h2>
							<button type="button" id="downloads_tab_clear" class="btn_link right_padding">Clear all</button>
							<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
						</div>
									</div>
				<div id="downloads_empty">
					<img alt="" src="https://cdx.slack-edge.com/0180/img/downloads_empty.png" srcset="https://cdx.slack-edge.com/0180/img/downloads_empty.png 1x, https://cdx.slack-edge.com/b8a7/img/downloads_empty@2x.png 2x">
										<p>You can download files by clicking the <ts-icon class="ts_icon_cloud_download" aria-hidden="true"></ts-icon> button.</p>
				</div>
				<div id="downloads_scroller" class="flex_content_scroller"></div>
				<div id="downloads_shift_hint">Hold <span class="key">Shift</span> to open the file.</div>
			</div>
			<div class="panel" id="whats_new_tab" style="height: 609px;">
				<div class="heading" tabindex="-1">
											<div class="heading_row">
							<h2 id="whats_new_tab_header" class="heading_text overflow_ellipsis">What's New</h2>
							<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
						</div>
						<div class="heading_row flex_heading_controls">
					
						<label class="checkbox" for="what_new_read_cb"><input id="what_new_read_cb" type="checkbox"> Notify me about updates</label>
					</div>
				</div>
				<div id="whats_new_scroller" class="flex_content_scroller">
					
<div id="whats_new_updates" class="lato normal_margin">
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1484758800">
			<h5 class="subtle_silver capitalize">January 18, 2017</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/threaded-messaging-comes-to-slack-417ffba054bd" target="new" class="indifferent_grey whats_new_content">Threaded messaging comes to Slack</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content html"></p><p>All kinds of conversations happen in channels. Now with Threads, you can branch off and have discussions around a particular message without having to skip to a different channel or a DM. Threads move conversations to your sidebar — where you can ask and answer questions, give feedback, or go off on an inspired tangent.</p><p><a href="https://slackhq.com/threaded-messaging-comes-to-slack-417ffba054bd">See our blog post</a> for more on Threads, or choose your own adventure by clicking the <ts-icon class="ts_icon_small_reply align_bottom"></ts-icon> <b>Start a thread</b> button on any message.</p><p></p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1484071200">
			<h5 class="subtle_silver capitalize">January 10, 2017</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">Slack for Windows Store</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content html"></p><p>Oh, hello. Did you know we have an app on the Windows Store? Desktop notifications and Windows Live tiles work right out of the box (might work while still in the box too, it’s just more difficult to tell).</p><p>To get started, <a href="http://bit.ly/slackforwindows10whatsnew" target="_blank">download Slack from the Windows Store</a>. You’ll need to be running Windows 10 Anniversary Edition.</p><p></p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1481644800">
			<h5 class="subtle_silver capitalize">December 13, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/slack-calls-now-with-100-more-video-50bf365a0d98" target="new" class="indifferent_grey whats_new_content">Slack Video Calls are here <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:22.5% 50%;background-size:4100%" title="movie_camera">:movie_camera:</span></a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content html">And it’s simple to make one!<br><br>
Step 1: Click on the phone icon to start a call<br>
Step 2: Click the camera button to enable video<br>
Step 3: Talk to your chosen human. (Or just make faces. It is video, after all…)<br><br>
For the best experience, make sure you're on the <a href="https://slack.com/downloads/" target="_blank">latest versions</a> of our Mac and Windows desktop apps (or use Google Chrome).</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/slack-calls-now-with-100-more-video-50bf365a0d98" class="whats_new_more" target="new">Learn more on our blog<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1479229200">
			<h5 class="subtle_silver capitalize">November 15, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/in-case-you-missed-it-music-movies-and-more-in-slack-704a9d33a281" target="new" class="indifferent_grey whats_new_content">In case you missed it</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">In case you missed some recent updates to Slack, we’ve summed them up for you in a lovely little list on our blog, because you deserve to know all the things!</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/in-case-you-missed-it-music-movies-and-more-in-slack-704a9d33a281" class="whats_new_more" target="new">Read the recap<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1476900230">
			<h5 class="subtle_silver capitalize">October 19, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/google-drive-slack-79c862fa5e55#.eggn7547e" target="new" class="indifferent_grey whats_new_content">+ More Google Drive</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content html">See that + button just there to the left of your message box? Now, if your team has Google Drive installed, this handy button packs even more punch. Click the + button to create Google Docs, Slides, and Sheets right where you’re working. You can also use it to import any file from Google Drive and  share with your team in Slack, all without switching apps or juggling tabs. <br><br> Don’t see these options, but want to use them? Just <a href="https://slack.com/apps/A0F7YS32P-google-drive" target="_blank">install or request Google Drive</a> for your team, and the + menu is your oyster.</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/google-drive-slack-79c862fa5e55#.eggn7547e" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1473854401">
			<h5 class="subtle_silver capitalize">September 14, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/a-new-way-to-catch-up-in-slack-148857029091#.e4jzwiqzn" target="new" class="indifferent_grey whats_new_content">Get all caught up</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Meet All Unreads — a new way to catch up on a myriad of Slack conversations in one, simple sweep. With all your unread messages in one spot, you can quickly scan what’s new, review what you need to, and clear the rest. With just a scroll and a click, you’re all caught up!<span class="para_break"><i class="copy_only"><br></i></span>Don't see it in your sidebar? Head to <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">Preferences &gt; Advanced &gt; Channel List &gt; Turn on All Unreads.</b></p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/a-new-way-to-catch-up-in-slack-148857029091#.e4jzwiqzn" class="whats_new_more" target="new">Learn more on our blog<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1466531318">
			<h5 class="subtle_silver capitalize">June 21, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/get-more-done-with-message-buttons-5fa5b283a59" target="new" class="indifferent_grey whats_new_content">Do more of your work from Slack</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">We’ve built a new way to interact with the apps you use in Slack. Message buttons: little bonny buttons services can add to your apps. You can click to accept invites, approve things, and hold proper polls, all within Slack. A dozen apps with buttons are live today, with many more to come.</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/get-more-done-with-message-buttons-5fa5b283a59" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1465214400">
			<h5 class="subtle_silver capitalize">June 6, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/calls-come-to-slack-ad333ce98acf#.o7s7dwh6u" target="new" class="indifferent_grey whats_new_content">Calls: Out of beta and open to all</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">You can now jump on a call whenever you feel the need to talk out loud, directly within Slack. &nbsp;Call anyone on your team simply by clicking the telephone icon in the message menu, or clicking “Call” from their user profile.</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/calls-come-to-slack-ad333ce98acf#.o7s7dwh6u" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1463590800">
			<h5 class="subtle_silver capitalize">May 18, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/learning-to-share-in-slack-d6e4fcff01b8" target="new" class="indifferent_grey whats_new_content">As a wise person on this team once said…</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Sharing messages. The perfect way to loop people in, restart a discussion in a better channel, or revisit an old conversation. Hover over any message and click the “Share message…” icon to share a message, add context and get everyone up to speed.</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/learning-to-share-in-slack-d6e4fcff01b8" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1461348113">
			<h5 class="subtle_silver capitalize">April 22, 2016</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">A better way to navigate your message history</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Hop back to any date in your message history with the handy new <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">Jump to date</b> feature. You can find it in the settings menu for channels and direct messages. Huzzah! <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:32.5% 42.5%;background-size:4100%" title="rabbit">:rabbit:</span></p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1461326400">
			<h5 class="subtle_silver capitalize">April 22, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slack-files.com/T024BE7LD-F116W8W2H-2b7cb856c1" target="new" class="indifferent_grey whats_new_content">Ringing in Calls for Android (beta)</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">What a glorious day: Now you can accept and join a call from your Android device (tho’ not start one, but soon!). Since you’re part of the beta for Calls on desktop, we thought you might want to try this out. Just make sure to update your mobile app to the latest version, please.</p></div>
							<p class="no_bottom_margin"><a href="https://slack-files.com/T024BE7LD-F116W8W2H-2b7cb856c1" class="whats_new_more" target="new">See the Known Issues list for Calls on Android<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1460660400">
			<h5 class="subtle_silver capitalize">April 14, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slackhq.com/getting-things-done-with-reminders-9bdb7686b57a" target="new" class="indifferent_grey whats_new_content">A friendly reminder about reminders</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Perhaps you use <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">/remind</b> to set reminders for yourself, other teammates, or even entire channels. As of today, you can also set reminders for any message in Slack, to remind yourself to come back to it. (We set a reminder to remind ourselves to tell you that. It worked!)</p></div>
							<p class="no_bottom_margin"><a href="https://slackhq.com/getting-things-done-with-reminders-9bdb7686b57a" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1460046764">
			<h5 class="subtle_silver capitalize">April 7, 2016</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slack-files.com/T024BE7LD-F0XUU5RGU-b4fec434f8" target="new" class="indifferent_grey whats_new_content">Say Hello to Calls for iOS</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">We just released Calls for iOS devices. Since you already use Calls, you get instant access when you update to Slack for iOS 2.90. But there may be some issues. If you want to see whether we know about one before you report it, we've created a handy list for you.</p></div>
							<p class="no_bottom_margin"><a href="https://slack-files.com/T024BE7LD-F0XUU5RGU-b4fec434f8" class="whats_new_more" target="new">See the Known Issues list for Calls on iOS<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1458164614">
			<h5 class="subtle_silver capitalize">March 17, 2016</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">JUMBOMOJI</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Ever feel regular-sized emoji aren’t enough to express your inner <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 55%;background-size:4100%" title="joy">:joy:</span>? Us too. So we made JUMBOMOJI. Now, messages containing emoji only (up to 23 at a time) are displayed jumbo-sized. Regular terms and conditions may apply. If emoji have those. We feel like they probably don’t. <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:30% 85%;background-size:4100%" title="elephant">:elephant:</span></p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1453245140">
			<h5 class="subtle_silver capitalize">January 20, 2016</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">A faster, smarter Quick Switcher</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">The Quick Switcher just got much much quicker, and smarter to boot. It now remembers the conversations you switch to most frequently and recently, and gets better the more you use it. If it’s not fixed in your muscle memory yet, now’s the perfect time to start: press cmd+k on Mac or ctrl+k on Windows and Linux to give it a try.</p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1450462640">
			<h5 class="subtle_silver capitalize">December 18, 2015</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">Allow others to edit your Posts</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Have a Post you want to work on with other people? Now, you can! Just check “Let others edit this Post” when sharing your Post, or, after sharing, use the toggle in the ellipsis menu. Done editing? Click “Done Editing” and let the next person take over.</p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1450367764">
			<h5 class="subtle_silver capitalize">December 17, 2015</h5>
			<h3 class="no_bottom_margin">
				<a href="http://slackhq.com/post/135387122640/do-not-disturb" target="new" class="indifferent_grey whats_new_content">Introducing Do Not Disturb</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Need time to yourself? Want to send someone a message after hours without bothering them? Go ahead! With Do Not Disturb, you can snooze notifications (including sounds) on any device for up to 24 hours. <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:50% 40%;background-size:4100%" title="zzz">:zzz:</span></p></div>
							<p class="no_bottom_margin"><a href="http://slackhq.com/post/135387122640/do-not-disturb" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1450313139">
			<h5 class="subtle_silver capitalize">December 17, 2015</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">A bigger, better image viewer</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Our cramped image previews have been replaced with a new full-size view which includes zoom capability. View images as they are meant to be viewed: bigly.</p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1450288800">
			<h5 class="subtle_silver capitalize">December 16, 2015</h5>
			<h3 class="no_bottom_margin">
				<a href="http://slackhq.com/post/134878632730/launch-platform" target="new" class="indifferent_grey whats_new_content">Find New Apps for Your Team</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">We’ve launched Slack’s App Directory with over 150 apps in categories from design to customer support to productivity. Find the products you already use every day and connect them to your Slack team for an instant lift in team productivity and mirth.</p></div>
							<p class="no_bottom_margin"><a href="http://slackhq.com/post/134878632730/launch-platform" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1447376659">
			<h5 class="subtle_silver capitalize">November 13, 2015</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">Do More with Messages</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">We’ve done away with that (nearly invisible) gear icon to bring you a new, more visible, more robust message actions menu. Hover over a message to quickly and instantly: add a reaction, edit your message, mark a message as unread, or copy the link to a message so you can reference it later.</p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1446494106">
			<h5 class="subtle_silver capitalize">November 2, 2015</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">Turn off this red dot thing</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">For those who don’t need or want to see what’s new in this What’s New section, you can now untick the checkbox above, and this latest red dot will be the last you’ll ever see. <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:35% 95%;background-size:4100%" title="wave">:wave:</span></p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1446248015">
			<h5 class="subtle_silver capitalize">October 31, 2015</h5>
			<h3 class="no_bottom_margin">
				<a href="http://slackhq.com/post/132116511325/customprofiles" target="new" class="indifferent_grey whats_new_content">Customizable, Bigger, Better Profiles</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Which department does Mo work in? Who does Shabnam report to? What’s Bill’s favorite emoji? Now available to admins and owners on paid plans, Custom Profiles lets you set up a profile unique to your team and how you work. We’ve also made the profile a little more <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:7.5% 97.5%;background-size:4100%" title="sparkles">:sparkles:</span> for everyone.</p></div>
							<p class="no_bottom_margin"><a href="http://slackhq.com/post/132116511325/customprofiles" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1446152418">
			<h5 class="subtle_silver capitalize">October 30, 2015</h5>
			<h3 class="no_bottom_margin">
				<a href="http://slackhq.com/post/132108708810/usergroups" target="new" class="indifferent_grey whats_new_content">User Groups and Default Channels</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Want to get the attention of some people without bugging anyone else? Now available for teams on paid plans, User Groups allow you to create <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">@windows-users</b> or <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">@trekkies</b> or <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">@interns</b> (or anything you like!) AND to add anyone joining that group to a designated set of channels.</p></div>
							<p class="no_bottom_margin"><a href="http://slackhq.com/post/132108708810/usergroups" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1446033601">
			<h5 class="subtle_silver capitalize">October 28, 2015</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">What’s New</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">We added a <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">What’s New</b> section with a natty red badge, for more expediently and efficiently letting you know what’s new. You’re looking at it. <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span></p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1446033600">
			<h5 class="subtle_silver capitalize">October 28, 2015</h5>
			<h3 class="no_bottom_margin">
				<span class="whats_new_content">Preference for Channel List Display</span>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Don’t want your public and private channels mixed? They don’t have to be. In your user preferences, choose <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">List public and private channels separately</b> in <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">Advanced Options</b> to keep them separated.</p></div>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1445929200">
			<h5 class="subtle_silver capitalize">October 27, 2015</h5>
			<h3 class="no_bottom_margin">
				<a href="http://slackhq.com/post/131956541795/groupmessages" target="new" class="indifferent_grey whats_new_content">Group Messages</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Pull up to 8 people into a private conversation without needing to create a channel for it. Use <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">cmd+shift+k</b> on the Mac App, <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">ctrl+shift+k</b> on Windows/Linux, or click the <b data-stringify-prefix="*" data-stringify-suffix="*" data-stringify-requires-siblings="">+</b> next to the Direct Message header to bring up the DM screen and create or view DMs and Group Messages.</p></div>
							<p class="no_bottom_margin"><a href="http://slackhq.com/post/131956541795/groupmessages" class="whats_new_more" target="new">Read the blog post<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
			<div class="bottom_border bottom_margin bottom_padding" data-whats-new-id="1445410800">
			<h5 class="subtle_silver capitalize">October 21, 2015</h5>
			<h3 class="no_bottom_margin">
				<a href="https://slack.zendesk.com/hc/en-us/articles/212221668-Team-wide-two-factor-authentication" target="new" class="indifferent_grey whats_new_content">Mandatory Two-Factor Authentication and Backup Codes</a>			</h3>
			<div class="whats_new_description"><p class="small_bottom_margin whats_new_content">Need to make sure everyone on your team is safe and secure? Teams on paid plans can now turn on Mandatory Two-Factor Authentication. Because you should always trust your team to be themselves.</p></div>
							<p class="no_bottom_margin"><a href="https://slack.zendesk.com/hc/en-us/articles/212221668-Team-wide-two-factor-authentication" class="whats_new_more" target="new">Learn about two-factor authentication<i class="ts_icon ts_icon_chevron_medium_right ts_icon_inherit align_bottom"></i></a></p>
					</div>
	</div>				</div>
			</div>
						<div class="panel active" id="convo_tab" style="height: 609px;">
									<div class="heading" tabindex="-1">
						<div class="heading_row">
							<span id="convo_tab_back_container" class="hidden"><button id="convo_tab_back" class="btn_link" aria-label="Back"><ts-icon class="ts_icon_chevron_medium_left"></ts-icon></button></span>
							<h2 id="convo_tab_header" class="heading_text overflow_ellipsis">
								Thread								<span class="thread_participants overflow_ellipsis">aramjam, aghasi.lorsabyan, and 1 other</span>
							</h2>
							<div id="convo_tab_btns">
								<button class="close_flexpane btn_link" title="Close Flexpane" type="button">
									<ts-icon class="ts_icon_times"></ts-icon>
								</button>
							</div>
						</div>
					</div>
								<div id="convo_scroller" class="flex_content_scroller" style="height: 524px;">
					<div class="lato">
	<div id="convo_container"><ts-conversation data-model-ob-id="G3B6Z0Y81" data-thread-ts="1485181718.000013" class="has_replies">
	<ts-message id="msg_1485181718_000013_conversation" data-ts="1485181718.000013" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first selected" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485181718000013">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="open_in_channel" class="ts_icon ts_icon_jump ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Open in channel"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	


	<div class="message_content feature_message_replies format_for_thread_root">
		<div class="message_content_header">
			<div class="message_content_header_left">
									<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
					
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<a href="/archives/betconstruct_backend/p1485181718000013" target="new_1485198992132" class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300 no_wrap"><i class="copy_only">[</i>Today at 6:28 PM<i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:28:38 PM</span></span></span></a>
					

		<a class="show_replies light_only" title="Show conversation" href="/archives/betconstruct_backend/p1485181718000013" target="new_1485198992132">5 replies</a>
 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485181718.000013" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					

	<a href="/archives/betconstruct_backend/p1485181718000013" target="new_1485198992132" class="thread_channel_link">in betconstruct_backend</a>
 
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="https://enhancv.com/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fenhancv.com%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fenhancv.com%2F&quot;]" data-referer-original-href="https://enhancv.com/" rel="noreferrer" target="_blank">https://enhancv.com/</a>

	
	<div class="attachment_group has_border has_link">
		

<div class="inline_attachment standalone can_delete" data-attachment-id="1" data-real-src="https://enhancv.com/">


		<div class="msg_inline_attachment_column column_border">
		</div>

	

	<div class="msg_inline_attachment_column column_content">


			<div class="msg_inline_attachment_row attachment_flush_text attachment_source">

					<span class="attachment_source_icon"><img class="attachment_source_icon" src="https://slack-imgs.com/?c=1&amp;o1=wi16.he16&amp;url=https%3A%2F%2Fenhancv.com%2Fimg%2Ffavicon.29f993c1.png" alt=""></span>

					<span class="attachment_source_name">enhancv.com</span>



				
			</div>

			<div class="msg_inline_attachment_row attachment_flush_text">
					<div class="attachment_title">
							<a href="https://enhancv.com/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fenhancv.com%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fenhancv.com%2F&quot;]" data-referer-original-href="https://enhancv.com/" rel="noreferrer" target="_blank">
						Enhancv</a>
						
					</div>

						Enhancv helps you create compelling human-centric resumes that unveil the real person behind.
					<span class="media_caret"></span>
			</div>





	</div>

	

		<div class="delete_attachment_link" data-attachment-id="1"><ts-icon class="ts_icon_times_small"></ts-icon></div>

	

</div>

 
	</div>
	
<span class="constrain_triple_clicks"></span></span>

				

		<a class="show_replies dense_only" title="Show conversation" href="/archives/betconstruct_backend/p1485181718000013" target="new_1485198992132">5 replies</a>
 





						<div class="rxn_panel rxns_key_message-1485181718_000013-G3B6Z0Y81 " data-rxn-key="message-1485181718.000013-G3B6Z0Y81"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300  ts_tip_hidden">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
<span class="ts_tip_tip"><span class="ts_tip_multiline_inner">@aramjam and @gayane <span class="subtle_silver">reacted with :+1::skin-tone-2:</span></span></span></span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 ts_tip_hidden">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		<span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Add reaction...</span></span></span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485181718_000013_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="https://enhancv.com/" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=https%3A%2F%2Fenhancv.com%2F&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;https%3A%2F%2Fenhancv.com%2F&quot;]" data-referer-original-href="https://enhancv.com/" rel="noreferrer" target="_blank">https://enhancv.com/</a>.
						5 replies
			5 replies
			six twenty-eight PM.
		</span>

	</div>

</ts-message>
	<div class="convo_flexpane_divider"><span class="reply_count">5 replies</span></div>
	<ts-relatives class="descendants">

<ts-message id="msg_1485181832_000017_conversation" data-ts="1485181832.000017" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files first" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="U3B5F2125">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485181832000017?thread_ts=1485181718.000013&amp;cid=G3B6Z0Y81">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Add reaction …"></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485181832.000017" data-really-short="true">5h</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:30:32 PM</span></span></span></span>
			<span class="message_star_holder">

<button data-msg-id="1485181832.000017" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485181832.000017" data-really-short="false">5 hours ago</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Today&nbsp;at&nbsp;6:30:32&nbsp;PM</span></span></span>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485181832.000017" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><span class="mention">vanhakobyan</span>: thanks, it'd be better to listen to <a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> 's point of view<span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485181832_000017-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485181832_000017_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			<span class="mention">vanhakobyan</span>: thanks, it'd be better to listen to <a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" data-member-name="aghasi.lorsabyan" data-stringify-text="@U0U59721F" class="internal_member_link">@aghasi.lorsabyan</a> 's point of view.
			NaN replies
			six thirty PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485181892_000019_conversation" data-ts="1485181892.000019" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="U3B5F2125">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485181892000019?thread_ts=1485181718.000013&amp;cid=G3B6Z0Y81">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485181892.000019" data-really-short="true">5h</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 6:31:32 PM</span></span></span></span>
			<span class="message_star_holder">

<button data-msg-id="1485181892.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485181892.000019" data-really-short="false">5 hours ago</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Today&nbsp;at&nbsp;6:31:32&nbsp;PM</span></span></span>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485181892.000019" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>ok <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 72.5%;background-size:4100%" title="wink">:wink:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485181892_000019-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485181892_000019_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			ok <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 72.5%;background-size:4100%" title="wink">:wink:</span>.
			NaN replies
			six thirty-one PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485185623_000023_conversation" data-ts="1485185623.000023" data-model-ob-id="G3B6Z0Y81" data-member-id="U0U59721F" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="U3B5F2125">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485185623000023?thread_ts=1485181718.000013&amp;cid=G3B6Z0Y81">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class=" member_preview_link member_image thumb_36" data-member-id="U0U59721F" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U0U59721F-389563add683-48')" aria-hidden="true"></a>
				
			</div>
			<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485185623.000023" data-really-short="true">4h</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 7:33:43 PM</span></span></span></span>
			<span class="message_star_holder">

<button data-msg-id="1485185623.000023" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aghasi.lorsabyan" target="/team/aghasi.lorsabyan" class="message_sender color_U0U59721F color_9f69e7 member member_preview_link " data-member-id="U0U59721F">aghasi.lorsabyan</a>
				<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485185623.000023" data-really-short="false">4 hours ago</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Today&nbsp;at&nbsp;7:33:43&nbsp;PM</span></span></span>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485185623.000023" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>I would suggest to prepare a very simple CV for BetConstruct and beautiful CV like Vanik's CV for fun or for creativ companies. Remember, you are a backend developers, not frontend, your CV should be brutal and dry <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485185623_000023-G3B6Z0Y81 " data-rxn-key="message-1485185623.000023-G3B6Z0Y81"><span data-emoji="+1::skin-tone-2" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 user_reacted" title="You and @gayane <span class=&quot;subtle_silver&quot;>reacted with :+1::skin-tone-2:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:37.5% 25%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485185623_000023_label" class="message_aria_label hidden">
			<strong>aghasi.lorsabyan</strong>.
			I would suggest to prepare a very simple CV for BetConstruct and beautiful CV like Vanik's CV for fun or for creativ companies. Remember, you are a backend developers, not frontend, your CV should be brutal and dry <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:70% 10%;background-size:4100%" title="slightly_smiling_face">:slightly_smiling_face:</span>.
			NaN replies
			seven thirty-three PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485186328_000026_conversation" data-ts="1485186328.000026" data-model-ob-id="G3B6Z0Y81" data-member-id="U3CD6J85V" class="message feature_fix_files dirty_hover_container first" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="U3B5F2125">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485186328000026?thread_ts=1485181718.000013&amp;cid=G3B6Z0Y81">
		</div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
				
			</div>
			<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485186328.000026" data-really-short="true">4h</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 7:45:28 PM</span></span></span></span>
			<span class="message_star_holder">

<button data-msg-id="1485186328.000026" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a>
				<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485186328.000026" data-really-short="false">4 hours ago</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Today&nbsp;at&nbsp;7:45:28&nbsp;PM</span></span></span>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485186328.000026" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span>yeah, &nbsp;real tough men's CVs must be brutal, they must hurt the eyes of the reader <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:50% 57.5%;background-size:4100%" title="muscle">:muscle::skin-tone-2:</span> <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485186328_000026-G3B6Z0Y81"></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485186328_000026_label" class="message_aria_label hidden">
			<strong>aramjam</strong>.
			yeah, &nbsp;real tough men's CVs must be brutal, they must hurt the eyes of the reader <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:50% 57.5%;background-size:4100%" title="muscle">:muscle::skin-tone-2:</span> <span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 60%;background-size:4100%" title="smile">:smile:</span>.
			NaN replies
			seven forty-five PM.
		</span>

	</div>

</ts-message>
 

<ts-message id="msg_1485186624_000028_conversation" data-ts="1485186624.000028" data-model-ob-id="G3B6Z0Y81" data-member-id="U3B5F2125" class="message feature_fix_files first" data-selectable="true" data-thread-ts="1485181718.000013" data-parent-user-id="U3B5F2125">
		<div class="action_hover_container stretch_btn_heights" data-show_rxn_action="true" data-show_reply_action="false" data-show_comment_action="" data-abs_permalink="https://micarmenia.slack.com/archives/betconstruct_backend/p1485186624000028?thread_ts=1485181718.000013&amp;cid=G3B6Z0Y81">
<a data-action="reaction" class="ts_icon ts_icon_small_reaction ts_tip ts_tip_top ts_tip_float ts_tip_delay_60 ts_tip_hidden"><span class="ts_tip_tip">Add reaction …</span></a><a data-action="actions_menu" class="ts_icon ts_icon_small_ellipsis ts_tip ts_tip_top ts_tip_float ts_tip_delay_60" title="Show message actions"></a></div>

	<span class="is_pinned_holder"></span>

	

		<div class="message_gutter">
			<div class="message_icon">
								<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
				
			</div>
			<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485186624.000028" data-really-short="true">4h</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Today at 7:50:24 PM</span></span></span></span>
			<span class="message_star_holder">

<button data-msg-id="1485186624.000028" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
		</div>

	<div class="message_content feature_message_replies">
		<div class="message_content_header">
			<div class="message_content_header_left">
						<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
				<span class="timestamp ts_tip ts_tip_top ts_tip_float ts_tip_hidden ts_tip_multiline ts_tip_delay_300"><i class="copy_only">[</i><span class="relative_ts" data-ts="1485186624.000028" data-really-short="false">4 hours ago</span><i class="copy_only">]</i><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Today&nbsp;at&nbsp;7:50:24&nbsp;PM</span></span></span>
					

 
				

					
					<span class="message_star_holder">

<button data-msg-id="1485186624.000028" data-c-id="G3B6Z0Y81" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_message ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this message">
		Star this message
	</span>
</button>
 </span>
					
			</div>
				
		</div>


			<span class="message_body"><span class="constrain_triple_clicks"></span><a href="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;]" data-referer-original-href="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" rel="noreferrer" target="_blank">http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852</a><span class="inline_img_bytes "> (77KB)</span><i data-real-src="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" class="msg_inline_img_collapser ts_icon ts_icon_caret_down "></i><i data-real-src="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" class="msg_inline_img_expander ts_icon ts_icon_caret_right hidden"></i> <div data-real-src="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" class="clear_both msg_inline_img_holder msg_inline_holder msg_inline_holder_rounded" style="width:768px;"><a style="width:768px;" href="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;]" data-referer-original-href="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" rel="noreferrer" target="_blank" title="" class="file_viewer_external_link" data-src="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" data-link-url="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" data-width="768" data-height="1090"><div class="msg_inline_img_container"><div class="file_preview_preserve_aspect_ratio" style="padding-top: -moz-calc(1090 / 768 * 100% ); padding-top: -webkit-calc(1090 / 768 * 100% ); padding-top: calc(1090 / 768 * 100% );"><figure class="msg_inline_img msg_inline_child" data-real-background-image="https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852" style="background-image: url(&quot;https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;);"><img data-real-src="https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852" src="https://slack-imgs.com/?c=1&amp;url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852"></figure></div></div></a></div><span class="constrain_triple_clicks"></span></span>

				

 





						<div class="rxn_panel rxns_key_message-1485186624_000028-G3B6Z0Y81 " data-rxn-key="message-1485186624.000028-G3B6Z0Y81"><span data-emoji="sweat_smile" class="rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300 " title="@aramjam and @gayane <span class=&quot;subtle_silver&quot;>reacted with :sweat_smile:</span>">
	<span class="emoji-outer emoji-sizer" style="background: url(https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png);background-position:65% 62.5%;background-size:4100%"></span><span class="emoji_rxn_count" aria-label="2"></span>
</span><span class="rxn_hover_container">
		<span class="rxn menu_rxn ts_tip ts_tip_top ts_tip_float ts_tip_multiline ts_tip_delay_300" title="Add reaction...">
			<span class="emoji-outer emoji-sizer">
			<i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_add_reaction"></i>
			</span>
		</span></span></div>
						





		<i class="copy_only"><br></i>


		<span id="msg_1485186624_000028_label" class="message_aria_label hidden">
			<strong>vanhakobyan</strong>.
			<a href="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" data-referer-safe="1" onclick="this.href=&quot;https://slack-redir.net/link?url=http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;" onmouseover="this.href=TS.utility.referer_safe_url_map[&quot;http%3A%2F%2Fcdn.slidesharecdn.com%2Fss_thumbnails%2Fcvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg%3Fcb%3D1442416852&quot;]" data-referer-original-href="http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852" rel="noreferrer" target="_blank">http://cdn.slidesharecdn.com/ss_thumbnails/cvthemarketingwaymeuleman-120906183154-phpapp01-thumbnail-4.jpg?cb=1442416852</a>.
			NaN replies
			seven fifty PM.
		</span>

	</div>

</ts-message>
 </ts-relatives>
</ts-conversation></div>
	<div id="reply_container" class="">	<span class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></span>
<div class="inline_message_input_container">
	<form>
			<textarea class="message_input" placeholder="Reply..." style="overflow: hidden; word-wrap: break-word; height: 36px;"></textarea>

		<a class="emo_menu"><i class="ts_icon ts_icon_circle_fill"></i><i class="ts_icon ts_icon_smile_o"></i><i class="ts_icon ts_icon_happy_smile"></i></a>

		<span class="mini float_right edit_controls">
		<span class="candy_red hidden edit_warning">text is too long!</span></span>
	</form>
</div>
<div class="reply_broadcast_buttons_container">
	<div class="reply_broadcast_label_container">
		<label class="checkbox" for="reply_broadcast_toggle_1485181718.000013_convo">
			<input type="checkbox" id="reply_broadcast_toggle_1485181718.000013_convo" class="reply_broadcast_toggle">
				Also send to <ts-icon class="ts_icon_lock ts_icon_inherit"></ts-icon><span class="bold">betconstruct_backend</span>
					</label>
		<ts-icon class="ts_icon_question_circle ts_icon_inherit ts_tip ts_tip_top">
			<span class="ts_tip_tip">
					Send important info <br> back to the channel
							</span>
		</ts-icon>
	</div>
	<button class="reply_send btn btn_small btn btn_outline " type="button">Send</button>
</div> </div>
	<div id="convo_loading_indicator" class="hidden"></div>
</div>				</div>
			</div>
									<div id="app_profile_tab" class="panel" data-js="app_profile_tab" style="height: 609px;">
				<div class="heading" tabindex="-1">
											<div class="heading_row">
							<h2 id="app_profile_tab_header" class="heading_text overflow_ellipsis" data-js="app_profile_header">About this app</h2>
							<button type="button" class="btn_link close_flexpane" title="Close Flexpane"><i class="ts_icon ts_icon_times"></i></button>
						</div>
									</div>
				<div class="flex_content_scroller" data-js="app_profile_scroller">
				</div>
			</div>
					</div>

	</div>

	</div>

			</div>
	</div>
	


</div>

<script type="text/javascript">

	function vvv(v) {

		var vvv_warning = 'You cannot use vvv on dynamic values. Please make sure you only pass in static file paths.';
		if (TS && TS.warn) {
			TS.warn(vvv_warning);
		} else {
			console.warn(vvv_warning);
		}

		return v;
	}

	var cdn_url = "https:\/\/slack.global.ssl.fastly.net";
	var inc_js_setup_data = {
		emoji_sheets: {
			apple: 'https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_apple_64_indexed_256colors.png',
			google: 'https://cdx.slack-edge.com/f360/img/emoji_2016_06_08/sheet_google_64_indexed_128colors.png',
			twitter: 'https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_twitter_64_indexed_128colors.png',
			emojione: 'https://cdx.slack-edge.com/bfaba/img/emoji_2016_06_08/sheet_emojione_64_indexed_128colors.png',
		},
	};
</script>

		
 	


		






<script>window.ts_before_core_js = Date.now();</script>
<!-- output_js "core" -->
<script type="text/javascript" src="https://cdx.slack-edge.com/a34f1/js/rollup-core_required_libs.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/72fe0/js/rollup-core_required_ts.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/7eaf/js/libs/bootstrap-client.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>

<script>window.ts_after_core_js = Date.now();</script>

<script type="text/javascript">
<!--
	// common boot_data
	var boot_data = {
		start_ms: Date.now(),
		app: 'client',
		user_id: 'U3B5F2125',
		no_login: false,
		version_ts: '1485198458',
		version_uid: '0c70f773c2eac630bd23a4d7dc85afd8cb4528ad',
		cache_version: "v15-koala",
		cache_ts_version: "v1-cat",
		redir_domain: 'slack-redir.net',
		signin_url: 'https://slack.com/signin',
		abs_root_url: 'https://slack.com/',
		api_url: '/api/',
		team_url: 'https://micarmenia.slack.com/',
		image_proxy_url: 'https://slack-imgs.com/',
		beacon_timing_url: "https:\/\/slack.com\/beacon\/timing",
		beacon_error_url: "https:\/\/slack.com\/beacon\/error",
		clog_url: "clog\/track\/",
		api_token: 'xoxs-28165220340-113185069073-113906074946-6241eb6f80',
		ls_disabled: false,

		notification_sounds: [{"value":"b2.mp3","label":"Ding","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/b2.mp3"},{"value":"animal_stick.mp3","label":"Boing","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/animal_stick.mp3"},{"value":"been_tree.mp3","label":"Drop","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/been_tree.mp3"},{"value":"complete_quest_requirement.mp3","label":"Ta-da","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/complete_quest_requirement.mp3"},{"value":"confirm_delivery.mp3","label":"Plink","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/confirm_delivery.mp3"},{"value":"flitterbug.mp3","label":"Wow","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/flitterbug.mp3"},{"value":"here_you_go_lighter.mp3","label":"Here you go","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/here_you_go_lighter.mp3"},{"value":"hi_flowers_hit.mp3","label":"Hi","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/hi_flowers_hit.mp3"},{"value":"item_pickup.mp3","label":"Yoink","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/item_pickup.mp3"},{"value":"knock_brush.mp3","label":"Knock Brush","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/knock_brush.mp3"},{"value":"save_and_checkout.mp3","label":"Woah!","url":"https:\/\/slack.global.ssl.fastly.net\/dfc0\/sounds\/push\/save_and_checkout.mp3"},{"value":"hummus.mp3","label":"Hummus","url":"https:\/\/slack.global.ssl.fastly.net\/7fa9\/sounds\/push\/hummus.mp3"},{"value":"none","label":"None"}],
		alert_sounds: [{"value":"frog.mp3","label":"Frog","url":"https:\/\/slack.global.ssl.fastly.net\/a34a\/sounds\/frog.mp3"}],
		call_sounds: [{"value":"call\/alert_v2.mp3","label":"Alert","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/alert_v2.mp3"},{"value":"call\/incoming_ring_v2.mp3","label":"Incoming ring","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/incoming_ring_v2.mp3"},{"value":"call\/outgoing_ring_v2.mp3","label":"Outgoing ring","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/outgoing_ring_v2.mp3"},{"value":"call\/pop_v2.mp3","label":"Incoming reaction","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/pop_v2.mp3"},{"value":"call\/they_left_call_v2.mp3","label":"They left call","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/they_left_call_v2.mp3"},{"value":"call\/you_left_call_v2.mp3","label":"You left call","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/you_left_call_v2.mp3"},{"value":"call\/they_joined_call_v2.mp3","label":"They joined call","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/they_joined_call_v2.mp3"},{"value":"call\/you_joined_call_v2.mp3","label":"You joined call","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/you_joined_call_v2.mp3"},{"value":"call\/confirmation_v2.mp3","label":"Confirmation","url":"https:\/\/slack.global.ssl.fastly.net\/08f7\/sounds\/call\/confirmation_v2.mp3"}],
		call_sounds_version: "v2",
		max_team_handy_rxns: 5,
		max_channel_handy_rxns: 5,
		max_poll_handy_rxns: 7,
		max_handy_rxns_title_chars: 30,
				slack_timezones: [["(UTC-11:00) Midway Island, American Samoa","Pacific\/Midway",true,"Samoa Standard Time",null],["(UTC-10:00) Aleutian Islands","America\/Adak",false,"Hawaii-Aleutian Standard Time","Hawaii-Aleutian Daylight Time"],["(UTC-10:00) Hawaii","Pacific\/Honolulu",true,"Hawaii-Aleutian Standard Time",null],["(UTC-09:30) Marquesas Islands","Pacific\/Marquesas",true,"Marquesas Time",null],["(UTC-09:00) Alaska","America\/Anchorage",false,"Alaska Standard Time","Alaska Daylight Time"],["(UTC-08:00) Baja California","America\/Tijuana",false,"Pacific Standard Time","Pacific Daylight Time"],["(UTC-08:00) Pacific Time (US and Canada)","America\/Los_Angeles",true,"Pacific Standard Time","Pacific Daylight Time"],["(UTC-07:00) Arizona","America\/Phoenix",false,"Mountain Standard Time","Mountain Daylight Time"],["(UTC-07:00) Chihuahua, La Paz, Mazatlan","America\/Chihuahua",false,"Mountain Standard Time","Mountain Daylight Time"],["(UTC-07:00) Mountain Time (US and Canada)","America\/Denver",true,"Mountain Standard Time","Mountain Daylight Time"],["(UTC-06:00) Central America","America\/Belize",false,"Central Standard Time",null],["(UTC-06:00) Central Time (US and Canada)\t","America\/Chicago",true,"Central Standard Time","Central Daylight Time"],["(UTC-06:00) Easter Island","Pacific\/Easter",false,"Easter Island Standard Time","Easter Island Summer Time"],["(UTC-06:00) Guadalajara, Mexico City, Monterrey","America\/Mexico_City",false,"Central Standard Time","Central Daylight Time"],["(UTC-06:00) Saskatchewan","America\/Regina",true,"Central Standard Time","Central Daylight Time"],["(UTC-05:00) Bogota, Lima, Quito","America\/Bogota",false,"South America Pacific Standard Time",null],["(UTC-05:00) Chetumal","America\/Cancun",false,"Eastern Standard Time",null],["(UTC-05:00) Eastern Time (US and Canada)","America\/New_York",true,"Eastern Standard Time","Eastern Daylight Time"],["(UTC-05:00) Haiti","America\/Port-au-Prince",false,"Eastern Standard Time",null],["(UTC-05:00) Havana","America\/Havana",false,"Cuba Standard Time","Cuba Daylight Time"],["(UTC-05:00) Indiana (East)","America\/Indiana\/Indianapolis",false,"Eastern Standard Time","Eastern Daylight Time"],["(UTC-04:00) Asuncion","America\/Asuncion",false,"Paraguay Time","Paraguay Summer Time"],["(UTC-04:00) Atlantic Time (Canada)","America\/Halifax",false,"Atlantic Standard Time","Atlantic Daylight Time"],["(UTC-04:00) Caracas","America\/Caracas",false,"Venezuelan Standard Time",null],["(UTC-04:00) Cuiaba","America\/Cuiaba",false,"Amazon Time","Amazon Summer Time"],["(UTC-04:00) Georgetown, La Paz, Manaus, San Juan","America\/Manaus",true,"Atlantic Standard Time",null],["(UTC-04:00) Santiago","America\/Santiago",true,"Chile Standard Time","Chile Summer Time"],["(UTC-04:00) Turks and Caicos","America\/Grand_Turk",false,"Atlantic Standard Time",null],["(UTC-03:30) Newfoundland","America\/St_Johns",false,"Newfoundland Standard Time","Newfoundland Daylight Time"],["(UTC-03:00) Araguaina","America\/Fortaleza",false,"Brasilia Time",null],["(UTC-03:00) Brasilia","America\/Sao_Paulo",true,"Brasilia Time","Brasilia Summer Time"],["(UTC-03:00) Cayenne, Fortaleza","America\/Cayenne",false,"French Guiana Time",null],["(UTC-03:00) City of Buenos Aires","America\/Buenos_Aires",true,"Argentina Time",null],["(UTC-03:00) Greenland","America\/Godthab",false,"West Greenland Time","Western Greenland Summer Time"],["(UTC-03:00) Montevideo","America\/Montevideo",false,"Uruguay Time","Uruguay Summer Time"],["(UTC-03:00) Saint Pierre and Miquelon","America\/Miquelon",false,"Pierre & Miquelon Standard Time","Pierre & Miquelon Daylight Time"],["(UTC-03:00) Salvador","America\/Bahia",false,"Brasilia Time","Brasilia Summer Time"],["(UTC-02:00) Fernando de Noronha","America\/Noronha",true,"Fernando de Noronha Time",null],["(UTC-01:00) Azores","Atlantic\/Azores",false,"Azores Time","Azores Summer Time"],["(UTC-01:00) Cabo Verde Islands","Atlantic\/Cape_Verde",false,"Cape Verde Time",null],["(UTC) Casablanca","Africa\/Casablanca",false,"Western European Time","Western European Summer Time"],["(UTC) Dublin, Edinburgh, Lisbon, London","Europe\/London",false,"Greenwich Mean Time","British Summer Time"],["(UTC) Monrovia, Reykjavik","Africa\/Monrovia",false,"Greenwich Mean Time",null],["(UTC+01:00) Amsterdam, Berlin, Bern, Rome, Stockholm, Vienna","Europe\/Amsterdam",true,"Central European Time","Central European Summer Time"],["(UTC+01:00) Belgrade, Bratislava, Budapest, Ljubljana, Prague","Europe\/Belgrade",false,"Central European Time","Central European Summer Time"],["(UTC+01:00) Brussels, Copenhagen, Madrid, Paris","Europe\/Brussels",false,"Central European Time","Central European Summer Time"],["(UTC+01:00) Sarajevo, Skopje, Warsaw, Zagreb","Europe\/Warsaw",false,"Central European Time","Central European Summer Time"],["(UTC+01:00) West Central Africa","Africa\/Algiers",false,"Central European Time",null],["(UTC+01:00) Windhoek","Africa\/Windhoek",false,"West Africa Time","West Africa Summer Time"],["(UTC+02:00) Amman","Asia\/Amman",false,"Arabia Standard Time","Arabia Standard Time"],["(UTC+02:00) Athens, Bucharest","Europe\/Athens",false,"Eastern European Time","Eastern European Summer Time"],["(UTC+02:00) Beirut","Asia\/Beirut",false,"Eastern European Time","Eastern European Summer Time"],["(UTC+02:00) Cairo","Africa\/Cairo",false,"Eastern European Time","Eastern European Summer Time"],["(UTC+02:00) Damascus","Asia\/Damascus",false,"Eastern European Time","Eastern European Summer Time"],["(UTC+02:00) Gaza, Hebron","Asia\/Gaza",false,"Eastern European Time","Eastern European Summer Time"],["(UTC+02:00) Harare, Pretoria","Africa\/Harare",false,"Central Africa Time",null],["(UTC+02:00) Helsinki, Kiev, Riga, Sofia, Tallinn, Vilnius","Europe\/Helsinki",false,"Eastern European Time","Eastern European Summer Time"],["(UTC+02:00) Jerusalem","Asia\/Jerusalem",false,"Israel Standard Time","Israel Daylight Time"],["(UTC+02:00) Kaliningrad","Europe\/Kaliningrad",false,"Eastern European Time",null],["(UTC+02:00) Tripoli","Africa\/Tripoli",false,"Eastern European Time",null],["(UTC+03:00) Baghdad","Asia\/Baghdad",false,"Arabia Standard Time",null],["(UTC+03:00) Istanbul","Asia\/Istanbul",false,"Turkey Time",null],["(UTC+03:00) Kuwait, Riyadh","Asia\/Kuwait",true,"Arabia Standard Time",null],["(UTC+03:00) Minsk","Europe\/Minsk",false,"Further-eastern European Time",null],["(UTC+03:00) Moscow, St. Petersburg, Volgograd","Europe\/Moscow",true,"Moscow Time",null],["(UTC+03:00) Nairobi","Africa\/Nairobi",false,"East Africa Time",null],["(UTC+03:30) Tehran","Asia\/Tehran",false,"Iran Standard Time","Iran Daylight Time"],["(UTC+04:00) Abu Dhabi, Muscat","Asia\/Muscat",true,"Gulf Standard Time",null],["(UTC+04:00) Astrakhan, Ulyanovsk","Europe\/Astrakhan",false,"Moscow Standard Time","Moscow Standard Time +1"],["(UTC+04:00) Baku","Asia\/Baku",true,"Azerbaijan Time","Azerbaijan Summer Time"],["(UTC+04:00) Izhevsk, Samara","Europe\/Samara",false,"Samara Time",null],["(UTC+04:00) Port Louis","Indian\/Mauritius",false,"Mauritius Time",null],["(UTC+04:00) Tbilisi","Asia\/Tbilisi",false,"Georgia Standard Time",null],["(UTC+04:00) Yerevan","Asia\/Yerevan",false,"Armenia Time","Armenia Summer Time"],["(UTC+04:30) Kabul","Asia\/Kabul",false,"Afghanistan Time",null],["(UTC+05:00) Tashkent, Ashgabat","Asia\/Tashkent",true,"Uzbekistan Time",null],["(UTC+05:00) Ekaterinburg","Asia\/Yekaterinburg",false,"Yekaterinburg Time",null],["(UTC+05:00) Islamabad, Karachi","Asia\/Karachi",false,"Pakistan Standard Time",null],["(UTC+05:30) Chennai, Kolkata, Mumbai, New Delhi","Asia\/Kolkata",false,"India Standard Time",null],["(UTC+05:30) Sri Jayawardenepura","Asia\/Colombo",false,"ISri Lanka Standard Time",null],["(UTC+05:45) Kathmandu","Asia\/Katmandu",false,"Nepal Time",null],["(UTC+06:00) Astana","Asia\/Almaty",false,"Alma-Ata Time",null],["(UTC+06:00) Dhaka","Asia\/Dhaka",true,"Bangladesh Standard Time",null],["(UTC+06:00) Novosibirsk","Asia\/Novosibirsk",false,"Novosibirsk Time",null],["(UTC+06:30) Yangon (Rangoon)","Asia\/Rangoon",false,"Myanmar Time",null],["(UTC+07:00) Bangkok, Hanoi, Jakarta","Asia\/Bangkok",false,"Indochina Time",null],["(UTC+07:00) Barnaul, Gorno-Altaysk","Asia\/Barnaul",false,"Moscow Standard Time +4",null],["(UTC+07:00) Hovd","Asia\/Hovd",false,"Hovd Time","Hovd Summer Time"],["(UTC+07:00) Krasnoyarsk","Asia\/Krasnoyarsk",false,"Krasnoyarsk Time",null],["(UTC+07:00) Tomsk","Asia\/Tomsk",false,"Moscow Standard Time +4",null],["(UTC+08:00) Beijing, Chongqing, Hong Kong SAR, Urumqi","Asia\/Chongqing",true,"China Standard Time",null],["(UTC+08:00) Irkutsk","Asia\/Irkutsk",false,"Irkutsk Time",null],["(UTC+08:00) Kuala Lumpur, Singapore","Asia\/Kuala_Lumpur",false,"Singapore Standard Time",null],["(UTC+08:00) Perth","Australia\/Perth",false,"Australian Western Standard Time",null],["(UTC+08:00) Taipei","Asia\/Taipei",false,"Taiwan Standard Time",null],["(UTC+08:00) Ulaanbaatar","Asia\/Ulaanbaatar",true,"Ulaanbaatar Time",null],["(UTC+08:30) Pyongyang","Asia\/Pyongyang",false,"Pyongyang Time",null],["(UTC+08:45) Eucla","Australia\/Eucla",false,"Australian Central Western Standard Time",null],["(UTC+09:00) Chita","Asia\/Chita",false,"Yakutsk Time",null],["(UTC+09:00) Osaka, Sapporo, Tokyo","Asia\/Tokyo",true,"Japan Standard Time",null],["(UTC+09:00) Seoul","Asia\/Seoul",false,"Korea Standard Time",null],["(UTC+09:00) Yakutsk","Asia\/Yakutsk",false,"Yakutsk Time",null],["(UTC+09:30) Adelaide","Australia\/Adelaide",false,"Australian Central Standard Time","Australian Central Daylight Time"],["(UTC+09:30) Darwin","Australia\/Darwin",false,"Australian Central Standard Time","Australian Central Daylight Time"],["(UTC+10:00) Brisbane","Australia\/Brisbane",true,"Australian Eastern Standard Time","Australian Eastern Daylight Time"],["(UTC+10:00) Canberra, Melbourne, Sydney","Australia\/Canberra",true,"Australian Eastern Standard Time","Australian Eastern Daylight Time"],["(UTC+10:00) Guam, Port Moresby","Pacific\/Guam",false,"West Pacific Standard Time",null],["(UTC+10:00) Hobart","Australia\/Hobart",false,"Australian Eastern Standard Time","Australian Eastern Daylight Time"],["(UTC+10:00) Vladivostok","Asia\/Vladivostok",false,"Vladivostok Time",null],["(UTC+10:30) Lord Howe Island","Australia\/Lord_Howe",false,"Lord Howe Standard Time","Lord Howe Daylight Time"],["(UTC+11:00) Bougainville Island","Pacific\/Bougainville",false,"Bougainville Standard Time",null],["(UTC+11:00) Chokirdakh","Asia\/Srednekolymsk",false,"Srednekolymsk Time",null],["(UTC+11:00) Magadan","Asia\/Magadan",false,"Magadan Time",null],["(UTC+11:00) Norfolk Island","Pacific\/Norfolk",false,"Norfolk Time",null],["(UTC+11:00) Sakhalin","Asia\/Sakhalin",false,"Sakhalin Time",null],["(UTC+11:00) Solomon Islands, New Caledonia","Pacific\/Guadalcanal",false,"Central Pacific Standard Time",null],["(UTC+12:00) Anadyr, Petropavlovsk-Kamchatsky","Asia\/Anadyr",false,"Kamchatka Time",null],["(UTC+12:00) Auckland, Wellington","Pacific\/Auckland",false,"New Zealand Standard Time","New Zealand Daylight Time"],["(UTC+12:00) Fiji Islands","Pacific\/Fiji",false,"Fiji Time","Fiji Summer Time"],["(UTC+12:45) Chatham Islands","Pacific\/Chatham",false,"Chatham Island Standard Time","Chatham Island Daylight Time"],["(UTC+13:00) Nuku'alofa","Pacific\/Tongatapu",false,"Tonga Standard Time",null],["(UTC+13:00) Samoa","Pacific\/Apia",false,"West Samoa Time",null],["(UTC+14:00) Kiritimati Island","Pacific\/Kiritimati",false,"Line Islands Time",null]],
				default_tz: "America\/Los_Angeles",
				dst_offsets: {"Pacific\/Midway":{"tz_offset":-39600},"America\/Adak":{"tz_offset":-36000},"Pacific\/Honolulu":{"tz_offset":-36000},"Pacific\/Marquesas":{"tz_offset":-34200},"America\/Anchorage":{"tz_offset":-32400},"America\/Tijuana":{"tz_offset":-28800},"America\/Los_Angeles":{"tz_offset":-28800},"America\/Phoenix":{"tz_offset":-25200},"America\/Chihuahua":{"tz_offset":-25200},"America\/Denver":{"tz_offset":-25200},"America\/Belize":{"tz_offset":-21600},"America\/Chicago":{"tz_offset":-21600},"Pacific\/Easter":{"tz_offset":-18000},"America\/Mexico_City":{"tz_offset":-21600},"America\/Regina":{"tz_offset":-21600},"America\/Bogota":{"tz_offset":-18000},"America\/Cancun":{"tz_offset":-18000},"America\/New_York":{"tz_offset":-18000},"America\/Port-au-Prince":{"tz_offset":-18000},"America\/Havana":{"tz_offset":-18000},"America\/Indiana\/Indianapolis":{"tz_offset":-18000},"America\/Asuncion":{"tz_offset":-10800},"America\/Halifax":{"tz_offset":-14400},"America\/Caracas":{"tz_offset":-14400},"America\/Cuiaba":{"tz_offset":-10800},"America\/Manaus":{"tz_offset":-14400},"America\/Santiago":{"tz_offset":-10800},"America\/Grand_Turk":{"tz_offset":-14400},"America\/St_Johns":{"tz_offset":-12600},"America\/Fortaleza":{"tz_offset":-10800},"America\/Sao_Paulo":{"tz_offset":-7200},"America\/Cayenne":{"tz_offset":-10800},"America\/Buenos_Aires":{"tz_offset":-10800},"America\/Godthab":{"tz_offset":-10800},"America\/Montevideo":{"tz_offset":-10800},"America\/Miquelon":{"tz_offset":-10800},"America\/Bahia":{"tz_offset":-10800},"America\/Noronha":{"tz_offset":-7200},"Atlantic\/Azores":{"tz_offset":-3600},"Atlantic\/Cape_Verde":{"tz_offset":-3600},"Africa\/Casablanca":{"tz_offset":0},"Europe\/London":{"tz_offset":0},"Africa\/Monrovia":{"tz_offset":0},"Europe\/Amsterdam":{"tz_offset":3600},"Europe\/Belgrade":{"tz_offset":3600},"Europe\/Brussels":{"tz_offset":3600},"Europe\/Warsaw":{"tz_offset":3600},"Africa\/Algiers":{"tz_offset":3600},"Africa\/Windhoek":{"tz_offset":7200},"Asia\/Amman":{"tz_offset":7200},"Europe\/Athens":{"tz_offset":7200},"Asia\/Beirut":{"tz_offset":7200},"Africa\/Cairo":{"tz_offset":7200},"Asia\/Damascus":{"tz_offset":7200},"Asia\/Gaza":{"tz_offset":7200},"Africa\/Harare":{"tz_offset":7200},"Europe\/Helsinki":{"tz_offset":7200},"Asia\/Jerusalem":{"tz_offset":7200},"Europe\/Kaliningrad":{"tz_offset":7200},"Africa\/Tripoli":{"tz_offset":7200},"Asia\/Baghdad":{"tz_offset":10800},"Asia\/Istanbul":{"tz_offset":10800},"Asia\/Kuwait":{"tz_offset":10800},"Europe\/Minsk":{"tz_offset":10800},"Europe\/Moscow":{"tz_offset":10800},"Africa\/Nairobi":{"tz_offset":10800},"Asia\/Tehran":{"tz_offset":12600},"Asia\/Muscat":{"tz_offset":14400},"Europe\/Astrakhan":{"tz_offset":14400},"Asia\/Baku":{"tz_offset":14400},"Europe\/Samara":{"tz_offset":14400},"Indian\/Mauritius":{"tz_offset":14400},"Asia\/Tbilisi":{"tz_offset":14400},"Asia\/Yerevan":{"tz_offset":14400},"Asia\/Kabul":{"tz_offset":16200},"Asia\/Tashkent":{"tz_offset":18000},"Asia\/Yekaterinburg":{"tz_offset":18000},"Asia\/Karachi":{"tz_offset":18000},"Asia\/Kolkata":{"tz_offset":19800},"Asia\/Colombo":{"tz_offset":19800},"Asia\/Katmandu":{"tz_offset":20700},"Asia\/Almaty":{"tz_offset":21600},"Asia\/Dhaka":{"tz_offset":21600},"Asia\/Novosibirsk":{"tz_offset":25200},"Asia\/Rangoon":{"tz_offset":23400},"Asia\/Bangkok":{"tz_offset":25200},"Asia\/Barnaul":{"tz_offset":25200},"Asia\/Hovd":{"tz_offset":25200},"Asia\/Krasnoyarsk":{"tz_offset":25200},"Asia\/Tomsk":{"tz_offset":25200},"Asia\/Chongqing":{"tz_offset":28800},"Asia\/Irkutsk":{"tz_offset":28800},"Asia\/Kuala_Lumpur":{"tz_offset":28800},"Australia\/Perth":{"tz_offset":28800},"Asia\/Taipei":{"tz_offset":28800},"Asia\/Ulaanbaatar":{"tz_offset":28800},"Asia\/Pyongyang":{"tz_offset":30600},"Australia\/Eucla":{"tz_offset":31500},"Asia\/Chita":{"tz_offset":32400},"Asia\/Tokyo":{"tz_offset":32400},"Asia\/Seoul":{"tz_offset":32400},"Asia\/Yakutsk":{"tz_offset":32400},"Australia\/Adelaide":{"tz_offset":37800},"Australia\/Darwin":{"tz_offset":34200},"Australia\/Brisbane":{"tz_offset":36000},"Australia\/Canberra":{"tz_offset":39600},"Pacific\/Guam":{"tz_offset":36000},"Australia\/Hobart":{"tz_offset":39600},"Asia\/Vladivostok":{"tz_offset":36000},"Australia\/Lord_Howe":{"tz_offset":39600},"Pacific\/Bougainville":{"tz_offset":39600},"Asia\/Srednekolymsk":{"tz_offset":39600},"Asia\/Magadan":{"tz_offset":39600},"Pacific\/Norfolk":{"tz_offset":39600},"Asia\/Sakhalin":{"tz_offset":39600},"Pacific\/Guadalcanal":{"tz_offset":39600},"Asia\/Anadyr":{"tz_offset":43200},"Pacific\/Auckland":{"tz_offset":46800},"Pacific\/Fiji":{"tz_offset":43200},"Pacific\/Chatham":{"tz_offset":49500},"Pacific\/Tongatapu":{"tz_offset":46800},"Pacific\/Apia":{"tz_offset":50400},"Pacific\/Kiritimati":{"tz_offset":50400},"ttl_seconds":604752,"expiration_timestamp":1485803683},
				
		feature_tinyspeck: false,
		feature_i18n: false,
		feature_create_team_google_auth: false,
		feature_api_extended_2fa_backup: false,
		feature_flannel_fe: false,
		feature_thin_channel_membership: false,
		feature_frecency_normalization: true,
		feature_frecency_im_browser: false,
		feature_batch_file_deleted_event: false,
		feature_sales_tax: true,
		feature_message_replies: true,
		feature_message_replies_rewrite_864: false,
		feature_message_replies_inline: false,
		feature_message_replies_temp_msgs: false,
		feature_a11y_keyboard_shortcuts: false,
		feature_email_ingestion: false,
		feature_msg_consistency: false,
		feature_sli_channel_priority: false,
		feature_sli_clog_selections: true,
		feature_thanks: false,
		feature_attachments_inline: false,
		feature_fix_files: true,
		feature_files_list: true,
		feature_channel_eventlog_client: true,
		feature_elide_closed_dms: true,
		feature_no_redirects_in_ssb: true,
		feature_referer_policy: true,
		feature_calls: true,
		feature_integrations_message_preview: true,
		feature_paging_api: false,
		feature_promote_org_po: false,
		feature_enterprise_api: true,
		feature_enterprise_create: true,
		feature_enterprise_api_auth: true,
		feature_enterprise_profile: true,
		feature_enterprise_search: true,
		feature_enterprise_locked_settings: false,
		feature_frecency_migration: false,
		feature_enterprise_frecency: false,
		feature_enterprise_team_overview_page: false,
		feature_enterprise_conditional_team_removal: true,
		feature_enterprise_move_channels: false,
		feature_dunning: false,
		feature_enterprise_mandatory_2fa: true,
		feature_basic_analytics: false,
		feature_enterprise_user_account_settings: true,
		feature_enterprise_security_auth_refactor: false,
		feature_enterprise_profile_menu_deactivate_2fa: false,
		feature_enterprise_billing_section: true,
		feature_sso_sandbox: false,
		feature_mpim_restrictions: false,
		feature_js_raf_queue: false,
		feature_channel_highlights: false,
		feature_shared_channels: false,
		feature_external_shared_channels_ui: false,
		feature_you_autocomplete_me: false,
		feature_allow_shared_general: false,
		feature_fast_files_flexpane: true,
		feature_custom_saml_signin_button_label: true,
		feature_admin_approved_apps: true,
		feature_winssb_beta_channel: false,
		feature_inline_media_playback: true,
		feature_clog_whats_new: true,
		feature_presence_sub: false,
		feature_live_support_free_plan: false,
		feature_dm_yahself: true,
		feature_slackbot_goes_to_college: false,
		feature_newxp_enqueue_message: true,
		feature_lato_2_ssb: true,
		feature_focus_mode: false,
		feature_star_shortcut: false,
		feature_omit_localstorage_users_bots: false,
		feature_disable_ls_compression: false,
		feature_force_ls_compression: false,
		feature_sign_in_with_slack: true,
		feature_sign_in_with_slack_ui_elements: true,
		feature_fix_unstarrables: true,
		feature_app_review_scope_error: true,
		feature_zendesk_app_submission_improvement: false,
		feature_react_emoji_picker: false,
		feature_ignore_code_mentions: false,
		feature_better_msg_copying: true,
		feature_name_tagging_client: false,
		feature_name_tagging_client_extras: false,
		feature_name_tagging_client_search: false,
		feature_browse_date: true,
		feature_use_imgproxy_resizing: false,
		feature_always_active_bots: true,
		feature_slash_command_link_names: true,
		feature_single_team_apps: false,
		feature_update_message_file: true,
		feature_custom_clogs: true,
		feature_a11y_pref_text_size: false,
		feature_share_mention_comment_cleanup: false,
		feature_unread_view: true,
		feature_external_files: false,
		feature_min_web: false,
		feature_electron_memory_logging: false,
		feature_no_tokenless_ms_connections: false,
		feature_devrel_try_it_now: false,
		feature_wait_for_all_mentions_in_client: false,
		feature_prev_next_button: false,
		feature_free_inactive_domains: true,
		feature_platform_calls: true,
		feature_a11y_tab: false,
		feature_admin_billing_refactor: true,
		feature_wrapped_mention_parsing: false,
		feature_measure_css_usage: false,
		feature_take_profile_photo: false,
		feature_ajax_billing_history: true,
		feature_update_coachmarks_cta: true,
		feature_update_coachmarks_copy: true,
		feature_multnomah: false,
		feature_texty: false,
		feature_texty_takes_over: false,
		feature_texty_copy_paste: false,
		feature_sales_tax_address: true,
		feature_toggle_id_translation: false,
		feature_can_edit_app: true,
		feature_gdrive_1_dot_5: true,
		feature_mention_non_members: false,
		feature_hide_email_pref: true,
		feature_tos_oct2016: true,
		feature_flexbox_client: true,
		feature_emoji_menu_tuning: false,
		feature_discoverable_teams: false,
		feature_discoverable_teams_v1: false,
		feature_discoverable_teams_v2: false,
		feature_discoverable_teams_client_v1: false,
		feature_discoverable_teams_client_v2: false,
		feature_discoverable_teams_client_metrics: false,
		feature_thin_shares: false,
		feature_reveal_channel_renames: true,
		feature_claim_email_domain: true,
		feature_app_info_youtube_url: false,
		feature_api_metadata_token_allow: true,
		feature_app_cards_and_profs_frontend: true,
		feature_user_removed_from_team: true,
		feature_user_added_to_team: true,
		feature_a11y_ui_zoom: false,
		feature_message_menus: false,
		feature_contact_us_form: true,
		feature_app_cards_and_profs_set_card_color: false,
		feature_sli_recaps: false,
		feature_cdn_load_tracking: true,
		feature_searchable_member_list: false,
		feature_team_to_org_directory: true,
		feature_user_custom_status: false,
		feature_app_cards_app_label: false,
		feature_platform_metrics: true,
		feature_sales_contact_inquiry: true,
		feature_hide_join_leave: false,
		feature_show_drafts: true,
		feature_slim_scrollbar: false,
		feature_flexpane_redesign: true,
		feature_console_log_redactor: true,
		feature_ent_dash_new_modal: false,
		feature_trials_checkout_flow: false,
		feature_intl_channel_names: false,

	client_logs: {"0":{"numbers":[0],"whitelisted":false},"@scott":{"numbers":[2,4,37,58,67,141,142,389,390,481,488,529,667,773,888,999],"owner":"@scott"},"@eric":{"numbers":[2,23,47,48,65,66,72,73,82,91,93,96,222,365,438,528,552,777,794],"owner":"@eric"},"2":{"owner":"@scott \/ @eric","numbers":[2],"whitelisted":false},"4":{"owner":"@scott","numbers":[4],"whitelisted":false},"5":{"channels":"#dhtml","numbers":[5],"whitelisted":false},"23":{"owner":"@eric","numbers":[23],"whitelisted":false},"sounds":{"owner":"@scott","name":"sounds","numbers":[37]},"37":{"owner":"@scott","name":"sounds","numbers":[37],"whitelisted":true},"47":{"owner":"@eric","numbers":[47],"whitelisted":false},"48":{"owner":"@eric","numbers":[48],"whitelisted":false},"58":{"owner":"@scott","numbers":[58],"whitelisted":false},"65":{"owner":"@eric","numbers":[65],"whitelisted":false},"66":{"owner":"@eric","numbers":[66],"whitelisted":false},"67":{"owner":"@scott","numbers":[67],"whitelisted":false},"72":{"owner":"@eric","numbers":[72],"whitelisted":false},"73":{"owner":"@eric","numbers":[73],"whitelisted":false},"82":{"owner":"@eric","numbers":[82],"whitelisted":false},"@shinypb":{"owner":"@shinypb","numbers":[88,1000,1989,1996]},"88":{"owner":"@shinypb","numbers":[88],"whitelisted":false},"91":{"owner":"@eric","numbers":[91],"whitelisted":false},"93":{"owner":"@eric","numbers":[93],"whitelisted":false},"96":{"owner":"@eric","numbers":[96],"whitelisted":false},"@steveb":{"owner":"@steveb","numbers":[99]},"99":{"owner":"@steveb","numbers":[99],"whitelisted":false},"Channel Marking (MS)":{"owner":"@scott","name":"Channel Marking (MS)","numbers":[141]},"141":{"owner":"@scott","name":"Channel Marking (MS)","numbers":[141],"whitelisted":true},"Channel Marking (Client)":{"owner":"@scott","name":"Channel Marking (Client)","numbers":[142]},"142":{"owner":"@scott","name":"Channel Marking (Client)","numbers":[142],"whitelisted":true},"222":{"owner":"@eric","numbers":[222],"whitelisted":false},"365":{"owner":"@eric","numbers":[365],"whitelisted":false},"389":{"owner":"@scott","numbers":[389],"whitelisted":false},"390":{"owner":"@scott","numbers":[390],"whitelisted":false},"438":{"owner":"@eric","numbers":[438],"whitelisted":false},"@rowan":{"numbers":[444,666],"owner":"@rowan"},"444":{"owner":"@rowan","numbers":[444],"whitelisted":false},"481":{"owner":"@scott","numbers":[481],"whitelisted":false},"488":{"owner":"@scott","numbers":[488],"whitelisted":false},"528":{"owner":"@eric","numbers":[528],"whitelisted":false},"529":{"owner":"@scott","numbers":[529],"whitelisted":false},"552":{"owner":"@eric","numbers":[552],"whitelisted":false},"dashboard":{"owner":"@ac \/ @bruce \/ @kylestetz \/ @nic \/ @rowan","channels":"#devel-enterprise-fe, #feat-enterprise-dash","name":"dashboard","numbers":[666]},"@ac":{"channels":"#devel-enterprise-fe, #feat-enterprise-dash","name":"dashboard","numbers":[666],"owner":"@ac"},"@bruce":{"channels":"#devel-enterprise-fe, #feat-enterprise-dash","name":"dashboard","numbers":[666],"owner":"@bruce"},"@kylestetz":{"channels":"#devel-enterprise-fe, #feat-enterprise-dash","name":"dashboard","numbers":[666],"owner":"@kylestetz"},"@nic":{"channels":"#devel-enterprise-fe, #feat-enterprise-dash","name":"dashboard","numbers":[666],"owner":"@nic"},"666":{"owner":"@ac \/ @bruce \/ @kylestetz \/ @nic \/ @rowan","channels":"#devel-enterprise-fe, #feat-enterprise-dash","name":"dashboard","numbers":[666],"whitelisted":false},"667":{"owner":"@scott","numbers":[667],"whitelisted":false},"773":{"owner":"@scott","numbers":[773],"whitelisted":false},"777":{"owner":"@eric","numbers":[777],"whitelisted":false},"794":{"owner":"@eric","numbers":[794],"whitelisted":false},"888":{"owner":"@scott","numbers":[888],"whitelisted":false},"999":{"owner":"@scott","numbers":[999],"whitelisted":false},"1000":{"owner":"@shinypb","numbers":[1000],"whitelisted":false},"flannel":{"owner":"@shinypb","features":["feature_flannel_fe"],"channels":"#devel-flannel","name":"flannel","numbers":[1989]},"1989":{"owner":"@shinypb","features":["feature_flannel_fe"],"channels":"#devel-flannel","name":"flannel","numbers":[1989],"whitelisted":true},"ms":{"owner":"@shinypb","name":"ms","numbers":[1996]},"1996":{"owner":"@shinypb","name":"ms","numbers":[1996],"whitelisted":true},"@patrick":{"owner":"@patrick","channels":"#dhtml","numbers":[2001,2002,2003,2004]},"2001":{"owner":"@patrick","channels":"#dhtml","numbers":[2001],"whitelisted":false},"dnd":{"owner":"@patrick","channels":"dhtml","name":"dnd","numbers":[2002]},"2002":{"owner":"@patrick","channels":"dhtml","name":"dnd","numbers":[2002],"whitelisted":true},"2003":{"owner":"@patrick","channels":"dhtml","numbers":[2003],"whitelisted":false},"2004":{"owner":"@patrick","channels":"#feature_message_replies, #feat-threads","numbers":[2004],"whitelisted":false},"mc_sibs":{"name":"mc_sibs","numbers":[9999]},"9999":{"name":"mc_sibs","numbers":[9999],"whitelisted":false},"@fearon":{"owner":"@fearon","numbers":[98765]},"98765":{"owner":"@fearon","numbers":[98765],"whitelisted":false}},


		img: {
			app_icon: 'https://cdx.slack-edge.com/272a/img/slack_growl_icon.png'
		},
		page_needs_custom_emoji: false,
		page_needs_team_profile_fields: false,
		page_needs_enterprise: false,
				slackbot_help_enabled: true
	};

	
			boot_data.hbs_templates_version = "7a7b_c038";
	
			boot_data.ms_connect_url = "wss:\/\/mpmulti-40Rh.slack-msgs.com\/?flannel=1&token=xoxs-28165220340-113185069073-113906074946-6241eb6f80";
	
	
	
	// client boot data
	
				boot_data.logout_url = "https:\/\/slack.com\/"+'signout/'+"28165220340"+'?crumb=s-1485198931-83fd1f4900-%E2%98%83';
		boot_data.async_api_url = 'https://upload.slack.com/api/';
		boot_data.other_accounts = [];
		boot_data.codemirror_types = [{"type":"text","label":"Plain Text"},{"type":"-","label":"-"},{"type":"applescript","label":"AppleScript"},{"type":"boxnote","label":"BoxNote"},{"type":"c","label":"C"},{"type":"csharp","label":"C#"},{"type":"cpp","label":"C++"},{"type":"css","label":"CSS"},{"type":"csv","label":"CSV"},{"type":"clojure","label":"Clojure"},{"type":"coffeescript","label":"CoffeeScript"},{"type":"cfm","label":"Cold Fusion"},{"type":"crystal","label":"Crystal"},{"type":"cypher","label":"Cypher"},{"type":"d","label":"D"},{"type":"dart","label":"Dart"},{"type":"diff","label":"Diff"},{"type":"dockerfile","label":"Docker"},{"type":"erlang","label":"Erlang"},{"type":"fsharp","label":"F#"},{"type":"fortran","label":"Fortran"},{"type":"gherkin","label":"Gherkin"},{"type":"go","label":"Go"},{"type":"groovy","label":"Groovy"},{"type":"html","label":"HTML"},{"type":"handlebars","label":"Handlebars"},{"type":"haskell","label":"Haskell"},{"type":"haxe","label":"Haxe"},{"type":"java","label":"Java"},{"type":"javascript","label":"JavaScript\/JSON"},{"type":"julia","label":"Julia"},{"type":"kotlin","label":"Kotlin"},{"type":"latex","label":"LaTeX\/sTeX"},{"type":"lisp","label":"Lisp"},{"type":"lua","label":"Lua"},{"type":"matlab","label":"MATLAB"},{"type":"mumps","label":"MUMPS"},{"type":"markdown","label":"Markdown (raw)"},{"type":"ocaml","label":"OCaml"},{"type":"objc","label":"Objective-C"},{"type":"php","label":"PHP"},{"type":"pascal","label":"Pascal"},{"type":"perl","label":"Perl"},{"type":"pig","label":"Pig"},{"type":"post","label":"Post"},{"type":"powershell","label":"PowerShell"},{"type":"puppet","label":"Puppet"},{"type":"python","label":"Python"},{"type":"r","label":"R"},{"type":"ruby","label":"Ruby"},{"type":"rust","label":"Rust"},{"type":"sql","label":"SQL"},{"type":"sass","label":"Sass"},{"type":"scala","label":"Scala"},{"type":"scheme","label":"Scheme"},{"type":"shell","label":"Shell"},{"type":"smalltalk","label":"Smalltalk"},{"type":"swift","label":"Swift"},{"type":"tsv","label":"TSV"},{"type":"vb","label":"VB.NET"},{"type":"vbscript","label":"VBScript"},{"type":"velocity","label":"Velocity"},{"type":"verilog","label":"Verilog"},{"type":"xml","label":"XML"},{"type":"yaml","label":"YAML"}];
		boot_data.help_url = '/help/';
		boot_data.box_js_url = "https:\/\/app.box.com\/js\/static\/select.js";
		boot_data.box_app_key = "7qb0upkmzej553p5c70ppb2b0kvtrc43";
		boot_data.dropbox_js_url = "https:\/\/www.dropbox.com\/static\/api\/2\/dropins.js";
		boot_data.dropbox_app_key = "rciq3gnem9oirk6";
		
		boot_data.exp_cdn = "slack_cedexis_cdn";
					boot_data.incremental_boot_data = {"team":{"avatar_base_url":"https:\/\/ca.slack-edge.com\/","domain":"micarmenia","id":"T0U4V6GA0","name":"MIC","prefs":{"default_channels":["28174384311","28174414901"],"invites_only_admins":false,"allow_calls":true,"seen_invites_only_admins_warning":true,"image_34":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_34.png","image_44":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_44.png","image_68":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_68.png","image_88":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_88.png","image_102":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_102.png","image_132":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_132.png","image_230":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_230.png","image_original":"https:\/\/s3-us-west-2.amazonaws.com\/slack-files2\/avatars\/2016-12-07\/113799768547_48c67abf97615cf05e34_original.png","gdrive_enabled_team":true,"hide_referers":true,"msg_edit_window_mins":-1,"allow_message_deletion":true,"calling_app_name":"Slack","display_real_names":false,"who_can_at_everyone":"regular","who_can_at_channel":"ra","who_can_create_channels":"regular","who_can_archive_channels":"regular","who_can_create_groups":"ra","who_can_post_general":"ra","who_can_kick_channels":"admin","who_can_kick_groups":"regular","retention_type":0,"retention_duration":0,"group_retention_type":0,"group_retention_duration":0,"dm_retention_type":0,"dm_retention_duration":0,"file_retention_duration":0,"file_retention_type":0,"allow_retention_override":true,"require_at_for_mention":false,"default_rxns":["simple_smile","thumbsup","white_check_mark","heart","eyes"],"team_handy_rxns":{"restrict":false,"list":[{"name":"slightly_smiling_face","title":"I'm happy!"},{"name":"+1","title":"good!"},{"name":"white_check_mark","title":"done!"},{"name":"heart","title":"love it!"},{"name":"eyes","title":"looking..."}]},"channel_handy_rxns":null,"compliance_export_start":0,"warn_before_at_channel":"always","disallow_public_file_urls":false,"who_can_create_delete_user_groups":"admin","who_can_edit_user_groups":"admin","who_can_change_team_profile":"admin","allow_shared_channels":false,"display_email_addresses":true,"who_has_team_visibility":"ra","disable_file_uploads":"allow_all","disable_file_editing":false,"disable_file_deleting":false,"who_can_create_shared_channels":"admin","who_can_manage_shared_channels":{"type":["admin"]},"who_can_post_in_shared_channels":{"type":["regular","ra"]},"allow_shared_channel_perms_override":false,"no_primary_billing":false,"trial_eligible":1,"billing_email_daily":true,"billing_email_monthly":false,"has_compliance_export":false,"sso_signup_restrictions":1,"sso_sync_with_provider":true,"sso_disable_emails":false,"scheduled_exports_type":0,"scheduled_exports_user":0,"two_factor_auth_required":null,"session_duration":-1,"skip_mail_tls_certificate_verification":false,"change_gateways":false,"invites_limit":false,"has_shared_invites":false,"moved_old_emoji":false,"calls_sent_welcome_to_admins":false,"test_team":false,"spaces_opt_in":false,"has_enhanced_export":false,"two_factor_required":false,"has_setup_organization":false,"who_can_create_delete_auto_user_groups":"admin","disable_builtin_loading":false,"allow_dlp_access":false,"allow_dlp_exports_from_day_0":false,"display_email_addresses_auto":false,"enable_welcome_post":true,"app_whitelist_requests_enabled":true,"app_whitelist_requests_require_comment_enabled":false,"app_whitelist_requests_notify_slackbot":true,"sign_in_with_slack_disabled":false,"dnd_enabled":true,"dnd_start_hour":"22:00","dnd_end_hour":"08:00","sso_choose_username":true,"sso_change_email":null,"auth_mode":"normal","who_can_manage_integrations":{"type":["regular"]},"app_whitelist_enabled":false,"disabled_loading_categories":"28739679876"}},"self":{"prefs":{"highlight_words":"","user_colors":"","color_names_in_list":true,"growls_enabled":true,"tz":"Asia\/Yerevan","push_dm_alert":true,"push_mention_alert":true,"msg_replies":"{ \"flexpane\":false }","push_everything":false,"push_show_preview":true,"push_idle_wait":2,"push_sound":"b2.mp3","push_loud_channels":"","push_mention_channels":"","push_loud_channels_set":"","threads_everything":false,"email_alerts":"none","email_alerts_sleep_until":0,"email_misc":true,"email_weekly":true,"welcome_message_hidden":false,"all_channels_loud":false,"loud_channels":"","never_channels":"","loud_channels_set":"","search_sort":"timestamp","expand_inline_imgs":true,"expand_internal_inline_imgs":true,"expand_snippets":false,"posts_formatting_guide":true,"seen_welcome_2":true,"seen_ssb_prompt":false,"spaces_new_xp_banner_dismissed":false,"search_only_my_channels":false,"search_only_current_team":false,"emoji_mode":"default","emoji_use":"{\"+1\":7,\"slightly_smiling_face\":1,\"grinning\":12,\"smiley\":5,\"grin\":3,\"+1::skin-tone-2\":16,\"white_check_mark\":4,\"joy\":3,\"upside_down_face\":1,\"tada\":1,\"wink\":2,\"writing_hand::skin-tone-2\":1}","has_invited":false,"has_uploaded":true,"has_created_channel":false,"has_searched":false,"search_exclude_channels":"","messages_theme":"default","webapp_spellcheck":true,"no_joined_overlays":false,"no_created_overlays":false,"dropbox_enabled":false,"seen_domain_invite_reminder":false,"seen_member_invite_reminder":false,"mute_sounds":false,"arrow_history":false,"tab_ui_return_selects":true,"obey_inline_img_limit":true,"new_msg_snd":"knock_brush.mp3","require_at":true,"ssb_space_window":"","mac_ssb_bounce":"","mac_ssb_bullet":true,"expand_non_media_attachments":true,"show_typing":true,"pagekeys_handled":true,"last_snippet_type":"html","display_real_names_override":0,"display_preferred_names":true,"time24":false,"enter_is_special_in_tbt":false,"graphic_emoticons":false,"convert_emoticons":true,"ss_emojis":true,"sidebar_behavior":"","seen_onboarding_start":true,"onboarding_cancelled":false,"seen_onboarding_slackbot_conversation":false,"seen_onboarding_channels":false,"seen_onboarding_direct_messages":false,"seen_onboarding_invites":false,"seen_onboarding_search":false,"seen_onboarding_recent_mentions":false,"seen_onboarding_starred_items":false,"seen_onboarding_private_groups":false,"onboarding_slackbot_conversation_step":1,"dnd_enabled":true,"dnd_start_hour":"22:00","dnd_end_hour":"08:00","ent_teams":null,"unread_collapsed_channels":null,"mark_msgs_read_immediately":true,"start_scroll_at_oldest":true,"snippet_editor_wrap_long_lines":false,"ls_disabled":false,"sidebar_theme":"default","sidebar_theme_custom_values":"","f_key_search":false,"k_key_omnibox":true,"speak_growls":false,"mac_speak_voice":"com.apple.speech.synthesis.voice.Alex","mac_speak_speed":250,"at_channel_suppressed_channels":"","push_at_channel_suppressed_channels":"","prompted_for_email_disabling":false,"full_text_extracts":false,"no_text_in_notifications":false,"muted_channels":"","no_macelectron_banner":false,"no_macssb1_banner":false,"no_macssb2_banner":false,"no_winssb1_banner":true,"no_invites_widget_in_sidebar":false,"no_omnibox_in_channels":false,"k_key_omnibox_auto_hide_count":0,"prev_next_btn":false,"hide_user_group_info_pane":false,"mentions_exclude_at_user_groups":false,"privacy_policy_seen":true,"enterprise_migration_seen":true,"last_tos_acknowledged":"tos_oct2016","api_tos_consented":0,"api_tos_notified":0,"app_directory_tos_consented":false,"app_directory_channel":"","app_directory_channel_time":0,"search_exclude_bots":false,"load_lato_2":false,"fuller_timestamps":false,"last_seen_at_channel_warning":1484582306386,"msg_preview":false,"msg_preview_persistent":true,"emoji_autocomplete_big":false,"winssb_run_from_tray":true,"winssb_window_flash_behavior":"idle","two_factor_auth_enabled":false,"two_factor_type":null,"two_factor_backup_type":null,"hide_hex_swatch":false,"client_logs_pri":"","enhanced_debugging":false,"flannel_server_pool":"random","mentions_exclude_at_channels":true,"confirm_clear_all_unreads":true,"confirm_user_marked_away":true,"box_enabled":false,"seen_single_emoji_msg":true,"confirm_sh_call_start":true,"preferred_skin_tone":"2","show_all_skin_tones":false,"separate_private_channels":false,"whats_new_read":1484071200,"hotness":false,"frecency_jumper":"{\"c\":{\"id\":\"BKchannel\",\"count\":4,\"visits\":[1481308668463,1481398693048,1481723566775,1482405747310]},\"BKchannel\":{\"id\":\"BKchannel\",\"count\":8,\"visits\":[1481308668463,1481392217634,1481398693048,1481723566775,1482058126382,1482158910530,1482405747310,1484582227889],\"_reduced\":true},\"\":[{\"id\":\"U3CD6J85V\",\"count\":12,\"visits\":[1481312682882,1481312716855,1481395213151,1481564271899,1481565051240,1481820551151,1481891785956,1482325278230,1482671283191,1484931015749]},{\"id\":\"U3CCUK1JA\",\"count\":2,\"visits\":[1481395730120,1481478615230]},{\"id\":\"U3BS7F6H0\",\"count\":5,\"visits\":[1481401903590,1481463159740,1481820556477,1484584315769,1485108858191]},{\"id\":\"U3B7NFX8R\",\"count\":4,\"visits\":[1481654894983,1481654925764,1481654968332,1481738656831]},{\"id\":\"U3BTJ0H5K\",\"count\":2,\"visits\":[1481658011980,1482600677143]},{\"id\":\"U3BSURBNW\",\"count\":1,\"visits\":[1481918097992]},{\"id\":\"U3BR8V9PE\",\"count\":2,\"visits\":[1482059562537,1482060013427]},{\"id\":\"U0U59721F\",\"count\":4,\"visits\":[1482068907003,1482162018117,1482675285160,1482676872268]},{\"id\":\"U3B4Q1S8Y\",\"count\":2,\"visits\":[1482083761017,1482084989679]},{\"id\":\"U3B45EY1E\",\"count\":2,\"visits\":[1482339146063,1482343046180]},{\"id\":\"U3BEMJGFK\",\"count\":1,\"visits\":[1484242378003]}],\"U3CD6J85V\":{\"id\":\"U3CD6J85V\",\"count\":28,\"visits\":[1482671283191,1483082834226,1484507778557,1484507801528,1484507938223,1484508093081,1484508625925,1484931015750,1484931213479,1485189361995],\"_reduced\":true},\"ar\":{\"id\":\"U3CD6J85V\",\"count\":7,\"visits\":[1481313556949,1481397704492,1481820710699,1484507801528,1484507938223,1484508093081,1484508625925]},\"ch\":{\"id\":\"BKchannel\",\"count\":3,\"visits\":[1481392217634,1482058126382,1482158910530]},\"a\":{\"id\":\"U3CD6J85V\",\"count\":6,\"visits\":[1481394671057,1481738101003,1481820070227,1481820410534,1482068430501,1484931213479]},\"U3CCUK1JA\":{\"id\":\"U3CCUK1JA\",\"count\":5,\"visits\":[1481395730120,1481395933263,1481478615230,1481655313617,1481820708093],\"_reduced\":true},\"anu\":{\"id\":\"U3B7NFX8R\",\"count\":1,\"visits\":[1481395749841]},\"U3B7NFX8R\":{\"id\":\"U3B7NFX8R\",\"count\":5,\"visits\":[1481395749841,1481654894983,1481654925764,1481654968332,1481738656831],\"_reduced\":true},\"nar\":{\"id\":\"U3CCUK1JA\",\"count\":1,\"visits\":[1481395933262]},\"tig\":{\"id\":\"U3BEMJGFK\",\"count\":1,\"visits\":[1481400920938]},\"U3BEMJGFK\":{\"id\":\"U3BEMJGFK\",\"count\":5,\"visits\":[1481400920938,1484242378003,1484242901250,1484595147914,1485012334250],\"_reduced\":true},\"U3BS7F6H0\":{\"id\":\"U3BS7F6H0\",\"count\":7,\"visits\":[1481401903590,1481463159741,1481820556477,1481820704784,1484584315769,1485108858191,1485194428315],\"_reduced\":true},\"na\":{\"id\":\"U3CCUK1JA\",\"count\":1,\"visits\":[1481655313617]},\"U3BTJ0H5K\":{\"id\":\"U3BTJ0H5K\",\"count\":5,\"visits\":[1481658011980,1481914404804,1481914408082,1482600677143,1484584299834],\"_reduced\":true},\"t\":{\"id\":\"U3BS7F6H0\",\"count\":1,\"visits\":[1481820704784]},\"n\":{\"id\":\"U3CCUK1JA\",\"count\":1,\"visits\":[1481820708093]},\"h\":{\"id\":\"U3BTJ0H5K\",\"count\":2,\"visits\":[1481914404804,1481914408082]},\"U3BSURBNW\":{\"id\":\"U3BSURBNW\",\"count\":1,\"visits\":[1481918097992],\"_reduced\":true},\"U3BR8V9PE\":{\"id\":\"U3BR8V9PE\",\"count\":3,\"visits\":[1482059562537,1482060013428,1484677646530],\"_reduced\":true},\"U0U59721F\":{\"id\":\"U0U59721F\",\"count\":7,\"visits\":[1482068907003,1482070711364,1482162018117,1482250896211,1482675285160,1482676872268,1482765430487],\"_reduced\":true},\"ag\":{\"id\":\"U0U59721F\",\"count\":3,\"visits\":[1482070711364,1482250896211,1482765430487]},\"U3B4Q1S8Y\":{\"id\":\"U3B4Q1S8Y\",\"count\":2,\"visits\":[1482083761018,1482084989679],\"_reduced\":true},\"U3B45EY1E\":{\"id\":\"U3B45EY1E\",\"count\":4,\"visits\":[1482339146063,1482340076043,1482342113325,1482343046180],\"_reduced\":true},\"su\":{\"id\":\"U3B45EY1E\",\"count\":2,\"visits\":[1482340076043,1482342113325]},\"ara\":{\"id\":\"U3CD6J85V\",\"count\":3,\"visits\":[1483082834226,1484507778556,1485189361995]},\"s\":{\"id\":\"U3BEMJGFK\",\"count\":2,\"visits\":[1484242901250,1485012334250]},\"cha\":{\"id\":\"BKchannel\",\"count\":1,\"visits\":[1484582227889]},\"ho\":{\"id\":\"U3BTJ0H5K\",\"count\":1,\"visits\":[1484584299834]},\"sh\":{\"id\":\"U3BEMJGFK\",\"count\":1,\"visits\":[1484595147914]},\"ha\":{\"id\":\"U3BR8V9PE\",\"count\":1,\"visits\":[1484677646530]},\"ti\":{\"id\":\"U3BS7F6H0\",\"count\":1,\"visits\":[1485194428315]}}","frecency_ent_jumper":"","jumbomoji":true,"newxp_seen_last_message":"1","attachments_with_borders":false,"show_memory_instrument":false,"enable_unread_view":false,"seen_unread_view_coachmark":false,"seen_calls_video_beta_coachmark":false,"seen_calls_video_ga_coachmark":true,"seen_calls_ss_window_coachmark":false,"measure_css_usage":false,"enable_react_emoji_picker":true,"seen_replies_coachmark":true,"seen_custom_status_badge":false,"all_unreads_sort_order":"alphabetical","locale":"en_US","gdrive_authed":true,"gdrive_enabled":true,"seen_gdrive_coachmark":true,"channel_sort":"{\"is_custom_sorted\":false, \"priority_display\":false, \"priority_type\":\"\", \"sorts\":[]}","overloaded_message_time":0,"overloaded_message_type":"","overloaded_message_enabled":true,"overloaded_message_prev_channels":"{}","seen_highlights_coachmark":false,"a11y_font_size":"normal","a11y_animations":true,"greeting_step":"","intro_step":"","onboarding_pause":"","last_newxp_message":"","two_factor_initialization_key":"","two_factor_backup_codes":"","push_disabled_email":true,"needs_notification_prompt":true,"dnd_seen_snooze_warn":6,"self_dm_initialized":false,"self_dm_and_slackbot_help_initialized":true,"newxp_slackbot_step":"","newxp_seen_check_signup_email":0,"newxp_handled_check_signup_email":0,"newxp_seen_allow_signup_domains":0,"newxp_handled_allow_signup_domains":0,"newxp_seen_allow_signup_domains_2":0,"newxp_handled_allow_signup_domains_2":0,"newxp_seen_shared_invite":0,"newxp_seen_help_message":"1","newxp_portal_has_started":false,"newxp_portal_onboarding_step":"newxp_portal_has_started","newxp_portal_onboarding_step_message_sent_time":0,"intro_to_apps_message_seen":false}}};
		
	
			boot_data.should_use_flannel = true;
		boot_data.flannel_api_url = "https"+'://'+"upload.slack.com";
		boot_data.page_has_incomplete_user_model = true;
		boot_data.flannel_server_pool = "random";
				boot_data.is_in_flannel_experiment = true;
	
												boot_data.experiment_assignments = {"handlebars_from_smarty_perf":{"experiment_id":"46172931351","type":"user","group":"","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"smartybars_perf":{"experiment_id":"77818061717","type":"user","group":"","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"logstash_calls_client_logs":{"experiment_id":"79365041859","type":"user","group":"logstash_enabled","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"exp_cdn_cedexis":{"experiment_id":"89658780816","type":"user","group":"slack_cedexis_cdn","trigger":"launch_user","log_exposures":false,"exposure_id":"113185069073"},"whats_new_header_icon":{"experiment_id":"90543013442","type":"user","group":"control","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"gdrive_1_5_coachmark_experiment":{"experiment_id":"94271365346","type":"user","group":"yes_coach_mark","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"video_calls_blur":{"experiment_id":"104487908068","type":"user","group":"blur_enabled","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"tcws_subjectline_accountinfo":{"experiment_id":"110993584417","type":"user","group":"old_sl","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"calls_janus_beta":{"experiment_id":"111633435522","type":"user","group":"calls_janus_beta","trigger":"finished","log_exposures":false,"exposure_id":"113185069073"},"tcws_subjectline_invite_remind":{"experiment_id":"112926270033","type":"user","group":"old_sl","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"tcws_subjectline_get_both":{"experiment_id":"114094141509","type":"user","group":"new_sl_1","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"search_best_matches":{"experiment_id":"114125394135","type":"user","group":"control","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"tcws_subjectline_more_channels":{"experiment_id":"115070588629","type":"user","group":"old_sl","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"mentions_storage_multi_no_union":{"experiment_id":"116012544304","type":"user","group":"sql_union","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"tcws_subjectline_invite2":{"experiment_id":"128824542226","type":"user","group":"new_sl_1","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"tcws_subjectline_invite_more2":{"experiment_id":"128900930276","type":"user","group":"new_sl","trigger":"hash_user","log_exposures":true,"exposure_id":"113185069073"},"free_trial_email_subject":{"experiment_id":"57071396899","type":"team","group":"classic_subject","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"social_nudge_v0":{"experiment_id":"57452636336","type":"team","group":"","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"video_calls":{"experiment_id":"57458324849","type":"team","group":"video_enabled_ss_disabled","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"free_trial_remind_email_subject":{"experiment_id":"57752860833","type":"team","group":"classic_subject","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"migrate_stats_to_cds":{"experiment_id":"70039090853","type":"team","group":"stats_cds","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"migrate_stats_enable_dark_reads":{"experiment_id":"70047028338","type":"team","group":"stats_mysql_and_cds_dark_reads","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"domain_signup_links_for_mobile":{"experiment_id":"70804845972","type":"team","group":"treatment","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"invite_team_directory_ios":{"experiment_id":"77275546387","type":"team","group":"add_button","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"update_invite_coachmarks_cta":{"experiment_id":"84280109270","type":"team","group":"invite_cm_got_ita","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"team_creator_welcome_series":{"experiment_id":"86771837555","type":"team","group":"treatment","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"onboarding_tips_ios":{"experiment_id":"86784061120","type":"team","group":"control","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"new_user_invites_ios":{"experiment_id":"90602474723","type":"team","group":"control","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"channel_icon_tooltip_ios":{"experiment_id":"91223363988","type":"team","group":"control","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"google_contacts_invite_existing":{"experiment_id":"93086200404","type":"team","group":"google_contacts","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"google_contacts_invite_new":{"experiment_id":"93096027173","type":"team","group":"","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"app_suggestions":{"experiment_id":"99344409638","type":"team","group":"no_suggestions","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"channel_card_ios":{"experiment_id":"100856215509","type":"team","group":"show_card","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"},"invite_prompt_android":{"experiment_id":"105729328277","type":"team","group":"disabled","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"all_purpose_push_first_teammate":{"experiment_id":"105752097684","type":"team","group":"copy_1","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"},"channel_tooltip_android_v2":{"experiment_id":"107879915808","type":"team","group":"enabled","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"},"drawer_invite_cta_android":{"experiment_id":"108160608736","type":"team","group":"enabled","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"},"team_joiner_welcome_series":{"experiment_id":"113506709110","type":"team","group":"control","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"},"flannel_lazy_loading":{"experiment_id":"115786915570","type":"team","group":"flannel","trigger":"launch_team","log_exposures":false,"exposure_id":"28165220340"},"targetted_mpim_search":{"experiment_id":"120085429362","type":"team","group":"groups_members","trigger":"finished","log_exposures":false,"exposure_id":"28165220340"},"instant_inv_v1_1":{"experiment_id":"125376268324","type":"team","group":"email_invite_first","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"},"google_contacts_ios":{"experiment_id":"125947833172","type":"team","group":"allow_google_contacts","trigger":"hash_team","log_exposures":true,"exposure_id":"28165220340"}};
			
//-->
</script>
<script type="text/javascript">

(function() {
	if (window.boot_data) {
		// check for CSS support of -webkit-mask-image / mask-image, which will enable the shimmer feature.
		// style check cribbed from Modernizr.
		var div = document.createElement('div');
		if (div && (div.style['-webkit-mask-image'] !== undefined || div.style['mask-image'] !== undefined)) {
			$('html').addClass('supports_css_mask_image');
		}
		div = null;
	}
}());

boot_data.page_needs_custom_cmds = true;
boot_data.page_needs_custom_emoji = true;
boot_data.page_needs_emoji_menu = true;
boot_data.locale = "en_US";
boot_data.can_add_ura = false;
boot_data.default_channels = [{"id":"C0U54BA95","team_id":"28165220340","date_create":"1458548543","creator_id":"28179240049","name":"general","topic":"Company-wide announcements and work-based matters","topic_user_id":"0","topic_date_set":"0","purpose":"This channel is for team-wide communication and announcements. All team members are in this channel.","purpose_user_id":"28179240049","purpose_date_set":"1481117499","date_delete":"0","deletor_id":"0","date_archived":"0","archiver_id":"0","is_general":"1","retention_type":"0","retention_duration":"0","is_shared":"0","is_moved":"0","is_default":true},{"id":"C0U54C6SH","team_id":"28165220340","date_create":"1458548543","creator_id":"28179240049","name":"random","topic":"Non-work banter and water cooler conversation","topic_user_id":"0","topic_date_set":"0","purpose":"A place for non-work-related flimflam, faffing, hodge-podge or jibber-jabber you'd prefer to keep out of more focused work-related channels.","purpose_user_id":"0","purpose_date_set":"0","date_delete":"0","deletor_id":"0","date_archived":"0","archiver_id":"0","is_general":"0","retention_type":"0","retention_duration":"0","is_shared":"0","is_moved":"0","is_default":true}];
boot_data.should_use_local_lato_2 = false;
boot_data.api_active_migration_error_response_type = 'allow_reload';
TS.boot(boot_data);
</script>

<!-- output_js "secondary" -->
<script type="text/javascript" src="https://cdx.slack-edge.com/1e662/js/rollup-secondary_a_required.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/60973/js/rollup-secondary_b_required.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/968be/js/rollup-client.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>

<!-- output_js "regular" -->
<script type="text/javascript" src="https://cdx.slack-edge.com/e8c3d/js/TS.ms.flannel.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/542a/js/TS.flannel.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/871a9/js/TS.selection_signal.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/fbcf/js/TS.utility.window.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>
<script type="text/javascript" src="https://cdx.slack-edge.com/a263/js/TS.files.gdrive.js" crossorigin="anonymous" onload="window._cdn &amp;&amp; _cdn.ok(this, arguments)" onerror="window._cdn &amp;&amp; _cdn.failed(this, arguments)"></script>



<script type="text/javascript">

if (TS && TS.client && TS.client.ui) {

	TS.client.ui.prefReset = function(pref) {
		TS.api.call('users.prefs.set', {
			name: pref,
			value: false
		});
	}

	function gongSound(autoload) {
		if (soundManager && soundManager.ok()) {
			var sound = soundManager.createSound({
				id: 'pp_gong',
				url: 'https://cdx.slack-edge.com/ec58/sounds/gong.mp3',
				volume: 100
			});
			if (autoload) {
				sound.load();
			}
			return sound;
		}
		return null;
	}

	function modalFactory(modal_config, pref) {
		return new Promise(function (resolve, reject) {
			var shift_key_pressed;

			// Override for testing
			if (TS.model.prefs[pref] && window.location.href.indexOf(pref) !== -1) {
				TS.model.prefs[pref] = false;
			}

			// Safety net: Exit if pref not defined
			if (typeof TS.model.prefs[pref] === 'undefined') return resolve();

			var new_config = Object.create(modal_config);

			new_config.onShow = function () {
				if (modal_config.onShow) {
					modal_config.onShow();
				}
				$('#fs_modal').addClass(pref + '_dialog');

				// preload watcher
				// saves state of the shift key so we don't have to modify generic modal's event handling
				$(document).on('keydown', function(e) {
					if (e.shiftKey) {
						shift_key_pressed = true;
						try {
							gongSound(true);
						} catch(e) {
							// oh well
						}
					}
				});

				$(document).on('keyup', function(e) {
					shift_key_pressed = false;
				});

				// Don't focus the textbox in the background
				TS.client.ui.$msg_input.blur();
			};

			// Modify onEnd, so we can DRYly update the api and resolve the promise
			// Also, gong. very important.
			new_config.onEnd = function () {
				if (modal_config.onEnd) {
					modal_config.onEnd();
				}

				var sound;

				TS.api.call('users.prefs.set', {
					name: pref,
					value: true
				});

				if (shift_key_pressed && soundManager && soundManager.ok()) {
					// Ring in this agreement - literally.
					sound = gongSound();
					if (sound) {
						sound.play();
					}
				}

				// release preload watcher
				$(document).off('keydown');
				$(document).off('keyup');

				TS.api.call('users.prefs.set', {
					name: pref,
					value: true
				});

				$('#fs_modal').one('webkitTransitionEnd otransitionend oTransitionEnd msTransitionEnd transitionend', function () {
					$('#fs_modal').removeClass(pref + '_dialog');
					return resolve();
				});
			};

			// Exit if already seen
			if (TS.model.prefs[pref]) {
				return resolve();
			} else {
				TS.client.ui.$msg_input.blur();
				TS.generic_dialog.start(new_config);
			}

			// watch for changes on the pref
			TS.prefs[pref + '_changed_sig'].add(function () {
				if (!TS.model.prefs[pref]) {
					TS.generic_dialog.start(new_config);
				} else if (TS.ui.fs_modal.is_showing) {
					TS.ui.fs_modal.close();
				} else if (TS.generic_dialog.is_showing) {
					TS.generic_dialog.cancel();
				}
			}, TS.client.ui);
		});
	}

	TS.client.login_sig.add(function() {
    if (!window.winssb) {
      return;
    }

		// Clog screen information for a11y
		Promise.delay(50).then(function () {
			var info = TSSSB.call('getDisplayInformation');

      if (info && info.displays && info.windowFrame) {
				var wf = info.windowFrame;
        var display_resolutions = [];
        var window_frame = [wf.size[0] || 0, wf.size[1] || 0, wf.position[0] || 0, wf.position[1] || 0];

        info.displays.forEach(function (d) {
          if (d && d.size && d.size.width && d.size.height) {
            display_resolutions.push(d.size.width);
            display_resolutions.push(d.size.height);
          }

          display_resolutions.push(d.scaleFactor || 1);
        });

        TS.clog.track('DISPLAY_INFO', {
          display_resolutions: display_resolutions,
          window_frame: window_frame
	      });
      }
		}).catch(function () {
			TS.warn('Oh no, something went wrong');
		});

	}, TS.client.ui);

}

</script>






<style>.color_9f69e7:not(.nuc) {color:#9F69E7;}.color_4bbe2e:not(.nuc) {color:#4BBE2E;}.color_e7392d:not(.nuc) {color:#E7392D;}.color_3c989f:not(.nuc) {color:#3C989F;}.color_674b1b:not(.nuc) {color:#674B1B;}.color_e96699:not(.nuc) {color:#E96699;}.color_e0a729:not(.nuc) {color:#E0A729;}.color_684b6c:not(.nuc) {color:#684B6C;}.color_5b89d5:not(.nuc) {color:#5B89D5;}.color_2b6836:not(.nuc) {color:#2B6836;}.color_99a949:not(.nuc) {color:#99A949;}.color_df3dc0:not(.nuc) {color:#DF3DC0;}.color_4cc091:not(.nuc) {color:#4CC091;}.color_9b3b45:not(.nuc) {color:#9B3B45;}.color_d58247:not(.nuc) {color:#D58247;}.color_bb86b7:not(.nuc) {color:#BB86B7;}.color_5a4592:not(.nuc) {color:#5A4592;}.color_db3150:not(.nuc) {color:#DB3150;}.color_235e5b:not(.nuc) {color:#235E5B;}.color_9e3997:not(.nuc) {color:#9E3997;}.color_53b759:not(.nuc) {color:#53B759;}.color_c386df:not(.nuc) {color:#C386DF;}.color_385a86:not(.nuc) {color:#385A86;}.color_a63024:not(.nuc) {color:#A63024;}.color_5870dd:not(.nuc) {color:#5870DD;}.color_ea2977:not(.nuc) {color:#EA2977;}.color_50a0cf:not(.nuc) {color:#50A0CF;}.color_d55aef:not(.nuc) {color:#D55AEF;}.color_d1707d:not(.nuc) {color:#D1707D;}.color_43761b:not(.nuc) {color:#43761B;}.color_e06b56:not(.nuc) {color:#E06B56;}.color_8f4a2b:not(.nuc) {color:#8F4A2B;}.color_902d59:not(.nuc) {color:#902D59;}.color_de5f24:not(.nuc) {color:#DE5F24;}.color_a2a5dc:not(.nuc) {color:#A2A5DC;}.color_827327:not(.nuc) {color:#827327;}.color_3c8c69:not(.nuc) {color:#3C8C69;}.color_8d4b84:not(.nuc) {color:#8D4B84;}.color_84b22f:not(.nuc) {color:#84B22F;}.color_4ec0d6:not(.nuc) {color:#4EC0D6;}.color_e23f99:not(.nuc) {color:#E23F99;}.color_e475df:not(.nuc) {color:#E475DF;}.color_619a4f:not(.nuc) {color:#619A4F;}.color_a72f79:not(.nuc) {color:#A72F79;}.color_7d414c:not(.nuc) {color:#7D414C;}.color_aba727:not(.nuc) {color:#ABA727;}.color_965d1b:not(.nuc) {color:#965D1B;}.color_4d5e26:not(.nuc) {color:#4D5E26;}.color_dd8527:not(.nuc) {color:#DD8527;}.color_bd9336:not(.nuc) {color:#BD9336;}.color_e85d72:not(.nuc) {color:#E85D72;}.color_dc7dbb:not(.nuc) {color:#DC7DBB;}.color_bc3663:not(.nuc) {color:#BC3663;}.color_9d8eee:not(.nuc) {color:#9D8EEE;}.color_8469bc:not(.nuc) {color:#8469BC;}.color_73769d:not(.nuc) {color:#73769D;}.color_b14cbc:not(.nuc) {color:#B14CBC;}</style>


<script>
var radarRequested = false;
function startRadar() {
	radarRequested = true;
}
function initRadar() {
	startRadar = function() {
		cedexis.start(1, 21464);
	}
	if (radarRequested) startRadar();
}
function slackRadar() {
	startRadar();
	// re-run every hour
	window.setTimeout(slackRadar, 1000 * 60 * 60);
}
slackRadar();
</script>
<script async="" onload="initRadar()" src="//radar.cedexis.com/1/21464/radar.js"></script>

	<script>if (window._cdn) _cdn.scanPageAssets();</script>


	


<script>(function() {

	'use strict';

	
	
	

	var log_prefix = '🐶 ';
	var ms = 2500;

	
	var data = {
		storage_key: 'reload_attempts',
		reload_count: 0,
		reload_count_max: 1
	}

	function warn(msg) {
		if (window.console && console.warn) return console.warn(log_prefix + msg);
	}

	function log(msg) {
		if (window.console && console.log) return console.log(log_prefix + msg);
	}

	function showTroubleLoading() {
		if (document.body) {
			document.body['className'] += ' has_loading_trouble';
			window.setTimeout(function() {
				document.body['className'] += ' loading_trouble_transition';
			}, 100);
			
			if (window.TSBeacon) {
				window.TSBeacon('client_load_trouble', 1);
			} else {
				log('No window.TSBeacon to log failure, boo.');
			}
		} else {
			warn('showTroubleLoading: WTF could not find document.body!?')
		}
	}

	
	
	var storage = {
		get: function() {
			var key = data.storage_key;
			try {
				return window.sessionStorage && sessionStorage.getItem(key);
			} catch(err) {
				warn('unable to get sessionStorage key "' + key + '".');
			}
		},
		set: function(value) {
			var key = data.storage_key;
			try {
				return window.sessionStorage && sessionStorage.setItem(key, value);
			} catch(err) {
				warn('unable to set sessionStorage key "' + key + ' = ' + value + '".');
			}
		},
		remove: function() {
			var key = data.storage_key;
			try {
				return window.sessionStorage && sessionStorage.removeItem(key);
			} catch(err) {
				warn('unable to remove sessionStorage key "' + key + '".');
			}
		}
	}

	if (!window.TS || !TS.client) {
		warn('CDN JS watchdog: No TS or TS.client in page? Possible client / network / CDN failure. May reload in ' + ms + ' ms.');

		window.setTimeout(function() {

			if (!window.TS || !TS.client) {
				
				data.reload_count = (parseInt(storage.get(), 10) || 0);
				
				storage.set(++data.reload_count);
				if (data.reload_count > data.reload_count_max) {
					
					warn('No TS or !TS.client after ' + ms + ' msec - giving up, showing load trouble screen.');
					storage.remove();
					data.reload_count = 0;
					showTroubleLoading();
					return;
				}
				warn('No TS or !TS.client after ' + ms + ' msec - reloading (attempt ' +  data.reload_count + '/' + data.reload_count_max + ')');
				var no_cache = true;
				return window.location.reload(no_cache);
			} else {
				log('TS and TS.client recovered after inline check failed, loaded within ' + ms + ' ms.');
			}

			
			if (data.reload_count) {
				log('Loaded OK after reload_count = ' + data.reload_count + '. Clearing count from sessionStorage.');
				storage.remove();
			}

		}, ms);

	}

}());</script>


<style>

#trouble_loading_overlay {
	position: fixed;
	top: 0px;
	left: 0px;
	width: 100%;
	height: 100%;
	pointer-events: none;
}
#trouble_loading,
#trouble_loading_overlay {
	z-index: 9999;
	display: none;
	opacity: 0;
	transition: transform 0.5s ease-out, opacity 0.5s ease-out;
}
#trouble_loading {
	position: absolute;
	top: 50%;
	left: 50%;
	width: 100%;
	max-width: 35rem;
	/* on-screen positioning */
	height: 85%;
	min-height: 15rem;
	/* may need fiddling to natural max-height of content. */
	max-height: 21.5rem;
	overflow: auto;
	background: #fff;
	padding: 1.5rem;
	padding-bottom: 0;
	background-clip: padding-box;
	z-index: 9999;
	/* restore the default */
	-webkit-user-select: text;
	user-select: text;
	/* and look nice */
	-webkit-font-smoothing: antialiased;
	/* just to be safe */
	pointer-events: auto;
	border: 1px solid rgba(0,0,0,0.05);
	border-radius: 8px;
	font-family: 'Slack-Lato', "Helvetica Neue", helvetica, "Segoe UI", tahoma, verdana, arial, sans-serif;
	font-size: 1rem;
	/* slightly under-size: difference in scale is halved in offset. */
	transform: scale(0.95) translateX(-52.75%) translateY(-52.75%);
	box-shadow: 0px 0px 16px 8px rgba(0,0,0,0.05);
}
#trouble_loading a {
	text-decoration: none;
	color: #0073C6;
}
#trouble_loading a:hover {
	text-decoration: underline;
}
#trouble_loading code {
	font-family: Consolas, monaco, "Ubuntu Mono", courier, monospace !important;
	font-size: 0.75rem;
	white-space: normal;
	padding: 0 2px;
	font-variant-ligatures: none;
	background-color: #f7f7f9;
	border: 1px solid #e1e1e8;
	color: #CC2255;
}
#trouble_loading h1 {
	font-size: 1.5rem;
	margin: 0 0 0.25rem 0;
}
#trouble_loading h3 {
	font-size: 1.2rem;
}
#trouble_loading hr {
	border: none;
	border-top: 1px solid #E8E8E8;
	margin: 1.5rem auto;
	clear: both;
}
#trouble_loading .trouble_loading_content li {
	margin-bottom: 0.5rem;
}
#trouble_loading,
#trouble_loading .trouble_loading_content li {
	line-height: 1.275rem;
}
#trouble_loading p {
	line-height: 1.5rem;
	margin: 0.75rem 0;
}
#trouble_loading h1 + p {
	margin-top: 0px;
}
body.has_loading_trouble #loading-zone {
	/* forget about space reserved for channel list. */
	left: 0px;
	margin-left: 0px;
}
body.has_loading_trouble #loading_message,
body.has_loading_trouble #loading_welcome,
body.has_loading_trouble #client-ui {
	/* hide SVG "black hole" elements and some other things causing scrollbars */
	display: none;
}
body.has_loading_trouble #trouble_loading,
body.has_loading_trouble #trouble_loading_overlay {
	display: block;
}
body.has_loading_trouble #trouble_loading_overlay {
	background: #ccc;
}
body.has_loading_trouble.loading_trouble_transition #trouble_loading {
	opacity: 1;
	transform: scale(1) translateX(-50%) translateY(-50%);
	transition-duration: 0.33s;
	transition-delay: 0.25s;
}
body.has_loading_trouble.loading_trouble_transition #trouble_loading_overlay {
	opacity: 0.75;
}

</style>

<div id="trouble_loading_overlay"></div>
<div id="trouble_loading">

	<h1>For some reason, Slack couldn’t load <span title="'Face With Cold Sweat' emoji">😓</span></h1>
							<p>We’re quite sorry about this! Before you try to troubleshoot, please do check <a href="https://status.slack.com/" title="Slack Service Status Site" target="_blank">http://status.slack.com</a> — the problem may be on our end.</p>
	
	<h3>Troubleshooting</h3>

	<div class="trouble_loading_content">

		<p>A few things to try:</p>

		<ul>
							<li><a href="#" onclick="window.location.reload(true);return false">Reload Slack</a>, or even restart your browser.</li>
						<li><a href="#" onclick="if (window.TSSSB) TSSSB.call('didFinishLoading'); document.location='/help/test'">Test your connection</a> to Slack’s servers.</li>
			<li>Make sure your security software isn’t blocking Slack.</li>
		</ul>

		<p><a href="/help" target="_blank">Check our Help Center</a> for more details, or <a href="/help/requests/new" target="_blank">drop us a line</a>.</p>

	</div>

</div>

<!-- slack-www-hhvm-09a1cb332ce574787 / 2017-01-23 11:15:31 / v0c70f773c2eac630bd23a4d7dc85afd8cb4528ad / B:H -->


<div id="chat_input_tab_ui" class="tab_complete_ui trap_menu_clicks hidden inactive" style="width: 476px; top: 597px; left: 280px;"> 					<div class="popover_mask"></div> 					<div class="tab_complete_ui_content"> 						<div id="chat_input_tab_ui_header" class="tab_complete_ui_header"> 							<span class="header_label"></span> 							<span class="header_search_term"></span> 							<span class="header_help"><strong>tab</strong>&nbsp; or &nbsp;<strong>↑</strong> <strong>↓</strong>&nbsp; to navigate <strong class="left_margin">↵</strong>&nbsp; to select <strong class="left_margin">esc</strong>&nbsp; to dismiss</span> 						</div> 					<div id="chat_input_tab_ui_scroller" class="tab_complete_ui_scroller"></div></div> 				</div><textarea tabindex="-1" style="position: absolute; top: -999px; left: 0px; right: auto; bottom: auto; border: 0px; padding: 0px; box-sizing: content-box; word-wrap: break-word; overflow: hidden; transition: none; height: 0px !important; min-height: 0px !important; font-family: Slack-Lato, appleLogo, sans-serif; font-size: 15px; font-weight: 400; font-style: normal; letter-spacing: 0px; text-transform: none; word-spacing: 0px; text-indent: 0px; line-height: 19.2px; width: 185px;" class="autosizejs" id="autosizejs" autocorrect="off" autocomplete="off" spellcheck="true"></textarea><div contenteditable="" class="offscreen"></div><div id="aria_live_announcer" role="status" aria-live="assertive">Private Channel betconstruct_backend</div><div style="position: absolute; top: -10000px; left: -10000px; width: 257px; font-size: 15px; font-family: Slack-Lato, appleLogo, sans-serif; font-weight: 400; line-height: 20px; resize: none; word-wrap: break-word;">...</div>
<ts-jumper>
	<ts-jumper-container>
		<ts-jumper-help aria-hidden="true">
			Jump to a conversation
			<span class="float_right">
				<strong>tab</strong>&nbsp; or &nbsp;<strong>↑</strong> <strong>↓</strong>&nbsp; to navigate <strong class="small_left_margin" aria-label="Return">↵</strong>&nbsp; to select <strong class="small_left_margin" aria-label="Escape">esc</strong>&nbsp; to dismiss
			</span>
		</ts-jumper-help>
		<input type="text" aria-label="Jump to a conversation. Up arrow and down arrow navigates results, return selects, escape closes." spellcheck="false" data-qa="jumper_input">
		<div id="" class="monkey_scroll_wrapper "><div class="monkey_scroll_bar  hidden" style="margin-left: 3.5px;"><div class="monkey_scroll_handle " style="left: 0px;">	<div class="monkey_scroll_handle_inner "></div></div></div><div class="monkey_scroll_hider" style="width: 100%;"><ts-jumper-results class="monkey_scroller"></ts-jumper-results></div></div>
	</ts-jumper-container>
</ts-jumper> 



<div id="inline_msg_input_tab_ui_0" class="tab_complete_ui trap_menu_clicks hidden inactive narrow"> 					<div class="popover_mask"></div> 					<div class="tab_complete_ui_content"> 						<div id="inline_msg_input_tab_ui_0_header" class="tab_complete_ui_header"> 							<span class="header_label"></span> 							<span class="header_search_term"></span> 							<span class="header_help"><strong>tab</strong>&nbsp; or &nbsp;<strong>↑</strong> <strong>↓</strong>&nbsp; to navigate <strong class="left_margin">↵</strong>&nbsp; to select <strong class="left_margin">esc</strong>&nbsp; to dismiss</span> 						</div> 					<div id="inline_msg_input_tab_ui_0_scroller" class="tab_complete_ui_scroller"></div></div> 				</div><div id="ts_tip_float_floater" style="width: 51px; height: 15px; left: 339.828px; top: 382.109px;" class="ts_tip ts_tip_top ts_tip_multiline ts_tip_delay_300 ts_tip_hidden"><span class="ts_tip_tip"><span class="ts_tip_multiline_inner">Open in archives<br><span class="subtle_silver no_wrap">Yesterday at 10:07:07 PM</span></span></span></div>

<div id="fs_modal_bg" class="active"></div>
<div id="fs_modal" class="fs_modal_file_viewer active">




	<div class="contents_container fs_modal_file_viewer_content">
		
		<div class="contents">
<header class="fs_modal_file_viewer_header">
		<div class="star_btn btn_icon btn star_file">
			

<button data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file">
		Star this file
	</span>
</button>
 
		</div>

	
	
	

<div class="file_header_detailed">
		<img class="member_image" src="https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48" alt="vanhakobyan">

	<h2 class="title no_jumbomoji">
		


		<span class="inline_edit inline_edit_editable" data-file-id="F3UD77DB3" aria-label="Rename this file’s title">
			<span class="inline_edit_inner">
				<span class="inline_edit_input" data-inline-edit-unformatted="VanikHakobyanResume 2017.pdf">VanikHakobyanResume 2017.pdf</span>
			</span>
		</span>

 
	</h2>

	<p class="file_meta">
			<a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a>
			<span class="bullet" aria-hidden="true">•</span>

		Today at 6:06 PM

		<span class="file_share_label" data-file-id="F3UD77DB3">in <span class="no_wrap"><a href="/archives/betconstruct_backend" target="/archives/betconstruct_backend" class="group_link" data-group-id="G3B6Z0Y81">betconstruct_backend</a>&nbsp;<a class="unshare_link ts_tip ts_tip_top ts_tip_float ts_tip_unshare_link" onclick="TS.files.promptForFileUnshare('F3UD77DB3', 'G3B6Z0Y81')"><span class="ts_tip_tip">Unshare from betconstruct_backend</span><i class="ts_icon ts_icon_minus_circle_small"></i></a></span></span>

	</p>
</div>
 
	 
	<div class="controls">

			<a href="https://files.slack.com/files-pri/T0U4V6GA0-F3UD77DB3/download/vanikhakobyanresume_2017.pdf" target="new_1485198992132" data-file-id="F3UD77DB3" class="download_btn control_btn btn_icon btn ts_icon ts_icon_cloud_download ts_tip ts_tip_bottom file_ssb_download_link">
				<div class="ts_tip_tip">Download
					<div class="muted_tooltip_info">131KB PDF</div>
				</div>
				<div class="flex_menu_download_circle"><canvas width="9" height="9"></canvas></div>
			</a>


			<button data-file-id="F3UD77DB3" class="more_btn control_btn btn_icon btn ts_icon ts_icon_ellipsis_o ts_tip ts_tip_bottom file_actions" data-include-view-public-link="true" data-exclude-rxn="true" data-exclude-edit-title="true" data-exclude-download="true" data-exclude-comment="true">
				<span class="ts_tip_tip">More actions</span>
			</button>

			<button class="comment_btn control_btn btn ts_tip ts_tip_bottom ">
				<ts-icon class="ts_icon ts_icon_comment_o"></ts-icon>
				<span class="comment_count">2</span>
				<span class="ts_tip_tip" data-tip-toggle-auto="Hide comments">View comments</span>
			</button>

		<button id="fs_modal_close_btn" class="close_btn control_btn btn_icon btn ts_icon ts_icon_times ts_tip ts_tip_bottom ts_tip_right">
			<div class="ts_tip_tip">Close
				<div class="muted_tooltip_info">(esc)</div>
			</div>
		</button>

	</div>
</header>

<div class="viewer">
		<div class="images">
			<div id="pdf_loading_spinner" class="hidden" title="Loading"><div class="infinite_spinner infinite_spinner_medium">
	<svg class="infinite_spinner_spinner infinite_spinner_fast " viewBox="0 0 100 100">
		<circle class="infinite_spinner_bg" cx="50%" cy="50%" r="35"></circle>
		<circle class="infinite_spinner_path infinite_spinner_blue " cx="50%" cy="50%" r="35"></circle>
	</svg>
	<svg class="infinite_spinner_spinner infinite_spinner_tail infinite_spinner_fast" viewBox="0 0 100 100">
		<circle class="infinite_spinner_path infinite_spinner_blue" cx="50%" cy="50%" r="35"></circle>
	</svg>
</div>
</div>
			<iframe id="pdf_display" src="https://slack.com/pdf-viewer?feature_pdf_viewer=1" style="width: 100%; height: 100%; border: none;"></iframe>
		</div>


</div>

<aside class="aside_panel">

	<div class="comments_container">
		
		
			<header class="comment_header">
				<button class="aside_close_btn">Close</button>
				<h4 class="comment_label">
						Comments
				</h4>
			</header>
		
			<div class="file_comments_F3UD77DB3 comments">

<div class="comment" data-timestamp="1485180411" data-comment-id="Fc3UD77GQZ">
	<a name="Fc3UD77GQZ"></a>
	<span class="no_print">	<a href="/team/vanhakobyan" target="/team/vanhakobyan" class=" member_preview_link member_image thumb_36" data-member-id="U3B5F2125" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-48')" aria-hidden="true"></a>
</span>
	<p class="comment_meta">
		<span class="no_print"><a href="/team/vanhakobyan" target="/team/vanhakobyan" class="message_sender color_U3B5F2125 color_d58247 member member_preview_link " data-member-id="U3B5F2125">vanhakobyan</a></span>
		<span class="print_only_inline"><strong>vanhakobyan</strong> • </span>
		<span class="comment_date_star_cog">
			Today at 6:06 PM
			<span class="no_print">

<button data-comment-id="Fc3UD77GQZ" data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
			<a class="comment_actions" data-file-id="F3UD77DB3" data-comment-id="Fc3UD77GQZ"><i class="comment_cog ts_icon ts_icon_cog ts_icon_inherit"></i></a>
		</span>
	</p>				
	<div class="comment_body">էս կանֆետի թուղթա?</div>
	<div class="rxn_panel rxns_key_file_comment-Fc3UD77GQZ-"></div>
</div>
 

<div class="comment" data-timestamp="1485181681" data-comment-id="Fc3UCPR2L8">
	<a name="Fc3UCPR2L8"></a>
	<span class="no_print">	<a href="/team/aramjam" target="/team/aramjam" class=" member_preview_link member_image thumb_36" data-member-id="U3CD6J85V" data-thumb-size="36" style="background-image: url('https://ca.slack-edge.com/T0U4V6GA0-U3CD6J85V-1bf45de8f7c0-48')" aria-hidden="true"></a>
</span>
	<p class="comment_meta">
		<span class="no_print"><a href="/team/aramjam" target="/team/aramjam" class="message_sender color_U3CD6J85V color_e0a729 member member_preview_link " data-member-id="U3CD6J85V">aramjam</a></span>
		<span class="print_only_inline"><strong>aramjam</strong> • </span>
		<span class="comment_date_star_cog">
			Today at 6:28 PM
			<span class="no_print">

<button data-comment-id="Fc3UCPR2L8" data-file-id="F3UD77DB3" class="star ts_icon ts_icon_star_o ts_icon_inherit ts_tip_top star_file_comment ts_tip ts_tip_float ts_tip_hidden btn_unstyle">
	<span class="ts_tip_tip" data-tip-toggle-auto="Unstar this file comment">
		Star this file comment
	</span>
</button>
 </span>
			<a class="comment_actions" data-file-id="F3UD77DB3" data-comment-id="Fc3UCPR2L8"><i class="comment_cog ts_icon ts_icon_cog ts_icon_inherit"></i></a>
		</span>
	</p>				
	<div class="comment_body">how did you do that?</div>
	<div class="rxn_panel rxns_key_file_comment-Fc3UCPR2L8-"></div>
</div>
 </div>
		
			<div class="no_comment">Be the first to leave a comment</div>
		
	</div>

	<div class="file_comment_form_container"><form action="" id="file_comment_form" class="comment_form clearfix" method="post">
			<a href="/team/vanhakobyan" class="member_preview_link" data-member-id="U3B5F2125" target="new">
			<span class="member_image thumb_36" style="background-image: url(https://ca.slack-edge.com/T0U4V6GA0-U3B5F2125-8dc5b1d2c719-72)" data-thumb-size="36" data-member-id="U3B5F2125"></span>
		</a>
		<input type="hidden" name="addcomment" value="1">
	<input type="hidden" name="crumb" value="s-1485198931-e359555c8b-☃">

	<textarea id="file_comment" data-el-id-to-keep-in-view="file_comment_submit_btn" class="small comment_input small_bottom_margin autogrow-short" name="comment" wrap="virtual" autocorrect="off" autocomplete="off" spellcheck="true" style="overflow: hidden; height: 38px;"></textarea>
	<span class="mini float_left indifferent_grey file_comment_tip">shift+enter to add a new line</span>	<button id="file_comment_submit_btn" type="submit" class="btn  btn_small float_right  ladda-button" data-style="expand-right"><span class="ladda-label">Add Comment</span></button>
</form><form id="file_edit_comment_form" class="edit_comment_form clearfix hidden" method="post">
		<textarea id="file_edit_comment" class="small comment_input small_bottom_margin" name="comment" wrap="virtual" autocorrect="off" autocomplete="off" spellcheck="true"></textarea><br>
	<input type="submit" class="save btn  btn_small float_right " value="Save">
	<button class="cancel btn btn_small btn_outline float_right small_right_margin ">Cancel</button>
</form></div>
</aside>
</div>
	</div>

</div>
</body>
