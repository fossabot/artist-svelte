<script lang="ts">
	import Accordion from '$lib/components/accordion';
	import AccordionItem from '$lib/components/accordionItem';
	import Paper from '$lib/components/paper';
	import more from '$lib/svg/icons/more';
	import SVGIcon from '$lib/utilities/svgParser/svg-parser.svelte';
</script>

<Paper shadow>
	<Accordion>
		<AccordionItem color="default" title="Default">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content default
		</AccordionItem>
		<AccordionItem variant="outline" color="primary" title="Primary">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>

			<Paper>
				<Accordion multiSelectable>
					<AccordionItem variant="fill" color="danger" title="Danger">
						<svelte:fragment slot="icon">
							<SVGIcon data={more} />
						</svelte:fragment>
						Content danger
					</AccordionItem>
					<AccordionItem variant="fill" color="success" title="Success">
						<svelte:fragment slot="icon">
							<SVGIcon data={more} />
						</svelte:fragment>
						Content success
						<Paper>
							<Accordion multiSelectable>
								<AccordionItem variant="fill" color="danger" title="Danger">
									<svelte:fragment slot="icon">
										<SVGIcon data={more} />
									</svelte:fragment>
									Content danger
								</AccordionItem>
								<AccordionItem variant="fill" color="success" title="Success">
									<svelte:fragment slot="icon">
										<SVGIcon data={more} />
									</svelte:fragment>
									Content success
								</AccordionItem>
							</Accordion>
						</Paper>
					</AccordionItem>
				</Accordion>
			</Paper>
		</AccordionItem>
		<AccordionItem color="secondary" title="Secondary">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content secondary
		</AccordionItem>
		<AccordionItem color="warning" title="Warning">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content warning
		</AccordionItem>
		<AccordionItem color="danger" title="Danger">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content danger
		</AccordionItem>
		<AccordionItem color="success" title="Success">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content success
		</AccordionItem>
		<AccordionItem color="info" title="Info">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content info
		</AccordionItem>
		<AccordionItem variant="fill" color="default" title="Default">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content default
		</AccordionItem>
		<AccordionItem variant="fill" color="primary" title="Primary">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content primary
		</AccordionItem>
		<AccordionItem variant="fill" color="secondary" title="Secondary">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content secondary
		</AccordionItem>
		<AccordionItem variant="fill" color="warning" title="Warning">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content warning
		</AccordionItem>
		<AccordionItem variant="fill" color="danger" title="Danger">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content danger
		</AccordionItem>
		<AccordionItem variant="fill" color="success" title="Success">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content success
		</AccordionItem>
		<AccordionItem variant="fill" color="info" title="Info">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content info
		</AccordionItem>

		<AccordionItem variant="gradient" color="default" title="Default">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content default
		</AccordionItem>

		<AccordionItem variant="gradient" color="primary" title="Primary">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content primary
		</AccordionItem>

		<AccordionItem variant="gradient" color="secondary" title="Secondary">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content secondary
		</AccordionItem>

		<AccordionItem variant="gradient" color="warning" title="Warning">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content warning
		</AccordionItem>

		<AccordionItem variant="gradient" color="danger" title="Danger">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content danger
		</AccordionItem>

		<AccordionItem variant="gradient" color="success" title="Success">
			<svelte:fragment slot="icon">
				<SVGIcon data={more} />
			</svelte:fragment>
			Content success
		</AccordionItem>
	</Accordion>
</Paper>
