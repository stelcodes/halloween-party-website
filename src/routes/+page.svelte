<script lang="ts">
	import '../reset.css';
</script>

<div class="app-container">
	<header>
		<div class="presents">
			<img class="skull" alt="skull" src="./images/skull-spin.gif" />
			<img class="tcwp" alt="the collective womb presents" src="./images/tcwp.gif" />
			<img class="skull" alt="skull" src="./images/skull-spin.gif" />
		</div>
		<!-- <img class="divider" alt="barbed wire" src="./images/barbed-wire-divider.png" /> -->
		<img class="hell" alt="hell" src="./images/hell.gif" />
		<div class="abh">@ bitch house</div>
		<img class="bones-divider" src="./images/bones-divider.png" alt="bones" />
	</header>
	<main>
		<h1>hell at bitch house</h1>
		<div class="date">
			<p>Saturday, October 26th</p>
			<p>8 PM - ???</p>
		</div>
	</main>
	<footer>
		<div class="text">
			<p>made by stel clementine</p>
			<span>🎀</span>
		</div>
	</footer>
</div>

<style lang="scss">
	@use 'sass:color';
	@use 'sass:math';
	@function rem($pxValue) {
		@return math.div($pxValue, 16px) * 1rem;
	}
	@font-face {
		font-family: 'crystopia';
		src: url('./fonts/crystopia.ttf');
		font-weight: 400;
		font-style: normal;
		font-display: swap;
	}
	@font-face {
		font-family: 'mr-monstar';
		src: url('./fonts/mr-monstar.ttf');
		font-weight: 400;
		font-style: normal;
		font-display: swap;
	}
	.app-container {
		display: flex;
		flex-direction: column;
		background: rgba(0, 0, 0, 0.3) url('./images/ghosts.png');
		background-blend-mode: darken;
		min-height: 100vh;
		color: white;
		cursor: url('https://cur.cursors-4u.net/holidays/hol-4/hol333.png'), pointer;
		font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;

		header,
		main,
		footer {
			display: flex;
			flex-direction: column;
			align-items: center;
		}

		header {
			flex: 0 1 auto;
			display: flex;
			flex-direction: column;
			align-items: center;

			.presents {
				max-width: 100%;
				display: flex;
				align-items: center;
				.skull {
					// max-width: 80px;
					height: 80px;
					flex: 0 1 80px;

					@media (max-width: 600px) {
						& {
							flex: 0 1 60px;
							height: 60px;
						}
					}
				}
				.tcwp {
					flex: 1 1 auto;
					width: 100%;
					max-width: 700px;
					padding: rem(10px);
					// height: auto;
				}
			}

			.hell {
				max-width: 100%;
			}

			.abh {
				font-family: cursive;
				font-size: rem(22px);
				padding: rem(16px) 0 0 0;
        margin-bottom: -10px;
			}

      .bones-divider {
        max-width: 100%;
      }
		}

		main {
			flex: 1 1 auto;

			h1 {
				visibility: hidden;
				display: none;
			}

      .date {
        width: 700px;
        max-width: 100%;
        background: rgba(0, 0, 0, 0.5);
        margin: 0 rem(32px) rem(32px);
        padding: rem(16px);

        p {
          font-size: rem(30px);
          text-align: center;
          padding: rem(4px) 0;
        }
      }
		}
		footer {
			flex: 0 0 auto;
			padding: rem(6px);
			background: rgba(0, 0, 0, 0.5);
			color: white;
			font-family: crystopia;
			font-size: rem(24px);

			.text {
				display: flex;
				align-items: center;

				p {
					padding: 0 rem(8px) rem(8px) 0;
				}
			}
		}
	}
</style>
