<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Teacher-first thinking",
			description: "Every feature starts with real teacher workflows, not boardroom assumptions."
		},
		{
			title: "Classroom empowerment",
			description: "Building tools that help educators do what they do best—inspire and teach."
		},
		{
			title: "Educational impact",
			description: "Measuring success by the time we give back to teachers and their students."
		}
	];
</script>

<SecondaryHero
	title="Solving world hunger"
	subtitle="one step at a time"
	imageSrc="https://www.unc.mn/image-placeholder.svg"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Dedicated to empowering educators."
	stakeholders={[
		{
			name: "Matt Sornson",
			position: "CEO",
			bio: "Passionate about transforming education through AI-powered tools that give teachers their time back.",
			image: "/generated/image-warm-professional-ceo-headshot-of-a-conf.webp"
		},
		{
			name: "Aaron Rasmussen",
			position: "President",
			bio: "Dedicated to building technology that understands teacher workflows and reduces administrative burden.",
			image: "/generated/image-professional-executive-headshot-of-a-con.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to reclaim your time?"
	subtitle="Join 100,000+ teachers who've made the switch"
	description="Stop drowning in lesson plans and grading. Teacher's Assistant handles the admin work so you can focus on what matters most—your students."
	imageSrc="/generated/image-a-warm-naturally-lit-elementary-classroo.webp"
/>
