<div class="tile-group">
  <div class="tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-camera-retro"></i>
      </div>
      <div class="title">
        Photos
      </div>
    </div>
  </div>
  <div class="tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-chess-knight"></i>
      </div>
      <div class="title">
        Games
      </div>
    </div>
  </div>
  <div class="tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-code"></i>
      </div>
      <div class="title">
        Code
      </div>
    </div>
  </div>
  <div class="tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-music"></i>
      </div>
      <div class="title">
        Music
      </div>
    </div>
  </div>
  <div class="tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-book"></i>
      </div>
      <div class="title">
        Books
      </div>
    </div>
  </div>
  <div class="tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-cogs"></i>
      </div>
      <div class="title">
        Settings
      </div>
    </div>
  </div>
</div>
<code class="title">Colorful Menu</code>
<div class="tile-group colorful">
  <div class="tile spotify">
    <div class="content">
      <div class="icon">
        <i class="fab fa-spotify"></i>
      </div>
    </div>
  </div>
  <div class="tile discord">
    <div class="content">
      <div class="icon">
        <i class="fab fa-discord"></i>
      </div>
    </div>
  </div>
  <div class="tile bandcamp">
    <div class="content">
      <div class="icon">
        <i class="fab fa-bandcamp"></i>
      </div>
    </div>
  </div>
  <div class="tile steam">
    <div class="content">
      <div class="icon">
        <i class="fab fa-steam"></i>
      </div>
    </div>
  </div>
  <div class="tile whatsapp">
    <div class="content">
      <div class="icon">
        <i class="fab fa-whatsapp"></i>
      </div>
    </div>
  </div>
  <div class="tile youtube">
    <div class="content">
      <div class="icon">
        <i class="fab fa-youtube"></i>
      </div>
    </div>
  </div>
</div>
<code class="title">Message Menu</code>
<div class="tile-group">
  <div class="tile msg-tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-skull"></i>
      </div>
      <div class="title">
        Death List
      </div>
      <div class="msg">
        If you don't know what a death list is, you shouldn't click on it.
      </div>
    </div>
  </div>
  <div class="tile msg-tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-question-circle"></i>
      </div>
      <div class="msg">
        You got question, we got answers.
      </div>
    </div>
  </div>
  <div class="tile msg-tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-dna"></i>
      </div>
      <div class="title">
        Experiment
      </div>
      <div class="msg">
        No, we are not Umbrella Corp.
      </div>
    </div>
  </div>
  <div class="tile msg-tile">
    <div class="content">
      <div class="icon">
        <i class="fab fa-old-republic"></i>
      </div>
      <div class="msg">
        The Old Republic was the Republic of legend, greater than distance or time.
      </div>
    </div>
  </div>
  <div class="tile msg-tile">
    <div class="content">
      <div class="icon">
        <i class="fa fa-newspaper"></i>
      </div>
      <div class="title">
        News
      </div>
      <div class="msg">
        Extra! Extra! Read All About It!
      </div>
    </div>
  </div>
</div>

<style>
body {
  font-family 			: sans-serif;
	
	code {
		font-size: 1.2em;
		display: block;
		
		&.title {
			font-size: 1.6em;
		}
	}
}

@tile-size          : 250px;
@border-outline     : 1px solid #333;

.tile-group {
  font-size         : 0;
	margin 						: 30px 0; //Just for presentarion. Feel free to omit it.
  
  .tile {
    position        : relative;
    display         : inline-flex;
    align-items     : center;
    justify-content : center;
    width           : @tile-size;
    height          : @tile-size;
    border          : @border-outline;
    outline         : @border-outline;
    font-size       : 20px;
    overflow        : hidden;
    vertical-align  : top;
    transition      : background-color 150ms, border 150ms, outline 150ms;
    cursor          : pointer;
    
    .content {
      text-align    : center;
      user-select   : none;
      
      .icon {
        position    : relative;
        font-size   : 2.5em;
				top 				: 0;
				transition  : top 150ms, font-size 150ms;
      }
    
      .title {
				position    : relative;
        font-size   : 1.2em;
				opacity     : 1;
				transition  : opacity 150ms;
				letter-spacing : 2px;
      }
			
			.msg {
				position 		: absolute;
				top 				: @tile-size;
				left 				: 0;
				width 			: 100%;
				transition  : top 150ms;
				font-family : monospace;
				font-size 	: 0.8em;
			}
    }
		
		&:hover {
      background-color : #333;
      color            : white;
			
			&.msg-tile {
				.icon {
					font-size    : 1.8em;
					top 				 : -(@tile-size * 0.25);
				}
				.title {
					opacity      : 0;
				}
				.msg {
					top 				 : (@tile-size * 0.5);
				}
			}
    }
  }
	
	
	@less-bg : #1d365d;
	@sass-bg : #c6538c;
	@disc-bg : #7289da;
	@spot-bg : #1ed760;
	@band-bg : #639aa9;
	@wapp-bg : #5ed054;
	@tube-bg : #f00;
	
	&.colorful {
		.tile {
			&.spotify:hover {
				background-color 		: @spot-bg;
				border-color 				: @spot-bg;
				outline 						: 1px solid @spot-bg;
			}
			&.less:hover {
				background-color 		: @less-bg;
				border-color 				: @less-bg;
				outline 						: 1px solid @less-bg;
			}
			&.discord:hover {
				background-color 		: @disc-bg;
				border-color 				: @disc-bg;
				outline 						: 1px solid @disc-bg;
			}	
			&.bandcamp:hover {
				background-color 		: @band-bg;
				border-color 				: @band-bg;
				outline 						: 1px solid @band-bg;
			}
			&.whatsapp:hover {
				background-color 		: @wapp-bg;
				border-color 				: @wapp-bg;
				outline 						: 1px solid @wapp-bg;
			}
			&.youtube:hover {
				background-color 		: @tube-bg;
				border-color 				: @tube-bg;
				outline 						: 1px solid @tube-bg;
			}
		}
	}
}
</style>

