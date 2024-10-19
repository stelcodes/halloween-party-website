<script lang="ts">
	import '../reset.css';
	import '98.css';
</script>

<svelte:head>
	<title>HELL @ bitch house</title>
</svelte:head>

<div class="app-container">
	<header>
		<div class="presents">
			<img class="skull" alt="skull" src="/images/skull-spin.gif" />
			<img class="tcwp" alt="the collective womb presents" src="/images/tcwp.gif" />
			<img class="skull" alt="skull" src="/images/skull-spin.gif" />
		</div>
		<!-- <img class="divider" alt="barbed wire" src="/images/barbed-wire-divider.png" /> -->
		<img class="hell" alt="hell" src="/images/hell.gif" />
		<div class="abh">@ bitch house</div>
		<img class="bones-divider" src="/images/bones-divider.png" alt="bones" />
	</header>
	<main>
		<h1>hell at bitch house</h1>
		<div class="date">
			<img src="/images/doll-orb.gif" alt="doll with orb" />
			<p>Saturday October 26th<br />8 PM - ???</p>
		</div>
		<img class="chain-divider" src="/images/chain-divider.gif" alt="chain" />
		<div class="attire">
			<p>Be a devil or a demon...<br />...or an angel if you dare!</p>
			<img src="/images/doll-candles.gif" alt="doll with candles" />
		</div>
		<!-- <img class="blood-divider" src="/images/blood-divider.gif" alt="chain" /> -->
		<div class="candles">
			<img src="/images/candle.gif" alt="candle" />
			<img src="/images/candle.gif" alt="candle" />
			<img src="/images/candle.gif" alt="candle" />
			<img src="/images/candle.gif" alt="candle" />
			<img src="/images/candle.gif" alt="candle" />
		</div>
		<div class="quiz">
			<img class="dancing" src="/images/dress.gif" alt="girl dancing" />
			<div class="win98 window" style="width: 300px">
				<div class="title-bar">
					<div class="title-bar-text">Friendship Test</div>
					<div class="title-bar-controls">
						<button aria-label="Minimize"></button>
						<button aria-label="Maximize"></button>
						<button aria-label="Close"></button>
					</div>
				</div>
				<div class="window-body">
					<p>Are you coming to the party???</p>
					<section class="field-row">
						<a href="https://youtu.be/_xJUCsyMQes?feature=shared&t=42" target="_blank">
							<button>Ofc</button>
						</a>
						<a href="https://www.youtube.com/watch?v=O04nsyB8gqA" target="_blank">
							<button>FUCK NO</button>
						</a>
					</section>
				</div>
			</div>
		</div>
	</main>
	<footer>
		<div class="text">
			<p>codes by <a href="mailto:hello@stelclementine.com">stel clementine</a></p>
			<img src="/images/skull-sprite.gif" alt="pink skull" />
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
		font-family: 'old-english-gothic';
		src: url('/fonts/old-english-gothic.otf');
		font-weight: 400;
		font-style: normal;
		font-display: swap;
	}
	* {
		cursor: url('https://cur.cursors-4u.net/holidays/hol-4/hol333.png'), pointer !important;
	}
	a {
		color: ghostwhite;
	}
	.app-container {
		display: flex;
		flex-direction: column;
		background: rgba(0, 0, 0, 0.3) url('/images/ghosts.png');
		background-blend-mode: darken;
		min-height: 100vh;
		color: ghostwhite;
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
				font-family: old-english-gothic;
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

			.chain-divider {
				max-width: 100%;
				padding: 0 rem(8px);
			}

			.date,
			.attire {
				width: 600px;
				max-width: 100%;
				margin: rem(16px) rem(32px) rem(16px);
				padding: rem(16px);
				display: flex;
				align-items: center;
				justify-content: space-evenly;
				font-family: old-english-gothic;

				p {
					font-size: rem(36px);
					text-align: center;
					padding-left: rem(4px);
				}
			}

			.candles {
				margin-top: rem(24px);
				width: 800px;
				max-width: 100%;
				display: flex;
				justify-content: space-around;

				img {
					display: block;
					width: 40px;
				}
			}

			.quiz {
				padding: 0 rem(16px);
				width: 800px;
				max-width: 100%;
				display: flex;
				justify-content: center;

				img.dancing {
					object-fit: contain;
					width: 70px;
					margin-right: rem(12px);
				}

				.win98 {
					margin: rem(64px) 0;
					flex: 0 1 300px;
					max-width: 100%;
					.title-bar {
						background: linear-gradient(90deg, #400, #a60000);
					}
					.window-body {
						color: black;

						p {
							font-size: rem(12px);
							line-height: 1.5;
							margin: rem(16px) 0;
						}

						.field-row {
							justify-content: flex-end;

							a {
								color: inherit;
								text-decoration: none;
								cursor: default;

								button {
									font-size: rem(12px);
								}
							}
						}
					}
				}
			}
		}
		footer {
			flex: 0 0 auto;
			padding: rem(6px);
			background: rgba(0, 0, 0, 0.5);
			color: white;
			font-family: old-english-gothic;
			font-size: rem(20px);

			.text {
				display: flex;
				align-items: center;

				p {
					padding: 0 rem(8px) rem(8px) 0;
				}
			}

			img {
				padding-bottom: rem(6px);
			}
		}
	}
</style>
