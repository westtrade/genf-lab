<div class="spot">
	<div class="spot__cover">
		<img src="" alt="" class="spot__image" />
		<div class="spot__title">
			<slot name="title" />
		</div>

		<div class="spot__location">
			<slot name="location" />
		</div>
	</div>

	<div class="spot__caption">
		<div class="spot__title-bottom">
			<slot name="title" />
		</div>
		<div class="spot__location-bottom">
			<slot name="location" />
		</div>
	</div>
</div>
