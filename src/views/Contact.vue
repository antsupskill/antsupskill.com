<template>
	<div>
		<div class="bg-ants-purple">
			<b-row no-gutters>
				<b-col
					align-self="center"
					class="text-white mx-7rem"
					style="font-family: 'Rajdhani', sans-serif"
				>
					<h1>Contact Us</h1>
					<h2>How can we help you out?</h2>
				</b-col>
				<b-col class="my-2 d-flex justify-content-center">
					<b-img
						fluid
						:src="
							require('/src/assets/img/contact-header-right.png')
						"
					></b-img>
				</b-col>
			</b-row>
		</div>
		<div style="background-color: #eeeeee">
			<b-row no-gutters>
				<b-col cols="6">
					<b-form
						@submit="onSubmit"
						class="form-spl p-5 my-5 mx-7rem"
					>
						<b-form-group
							id="input-group-1"
							label="Email Address:"
							label-for="input-1"
							description="We'll never share your email with anyone else."
						>
							<b-form-input
								id="input-1"
								v-model="form.email"
								type="email"
								class="inp-spl"
								placeholder="Enter email"
								required
							></b-form-input>
						</b-form-group>

						<b-form-group
							id="input-group-2"
							label="Subject:"
							label-for="input-2"
						>
							<b-form-input
								id="input-2"
								class="inp-spl"
								v-model="form.subject"
								placeholder="Enter subject"
								required
							></b-form-input>
						</b-form-group>

						<b-form-group
							id="input-group-3"
							label="Full Description:"
							label-for="input-3"
						>
							<b-form-textarea
								id="input-3"
								class="inp-spl"
								v-model="form.desc"
								placeholder="Enter the description"
								required
							>
							</b-form-textarea>
						</b-form-group>

						<b-button
							type="submit"
							variant="ants-purple"
							class="btn-spl"
							>Submit</b-button
						>
					</b-form>
				</b-col>
				<b-col align-self="center" class="text-center" cols="6">
					<div class="div-spl mx-7rem">
						<p class="font-weight-bold">
							We're here to help you out.
						</p>
						<p>
							If you have any questions, just reach out to us and
							we’ll respond as soon as we can. Please provide as
							much information as possible.
						</p>
					</div>
					<br />
					<br />
					<br />
					<div class="div-spl mx-7rem">
						<p class="font-weight-bold">
							You can also contact us through:
						</p>
						<p class="h6 font-weight-bold text-ants-purple">
							info@antsupskill.com <br />+91 97718 39439
						</p>
					</div>
				</b-col>
			</b-row>
		</div>
	</div>
</template>

<style scoped>
.form-spl {
	background-color: white;
	border-radius: 5px;
	font-family: 'Rajdhani', sans-serif;
}
.btn-spl {
	margin: 0 auto;
	display: block;
	padding-inline: 2rem;
}
.mx-7rem {
	margin-left: 7rem;
	margin-right: 7rem;
}
.inp-spl {
	background-color: #eeeeee;
	border-color: #eeeeee;
}
.div-spl {
	border: 2px solid #5d56c3;
	padding: 1rem;
}
</style>

<script>
export default {
	name: 'Contact',
	data() {
		return {
			form: {
				email: '',
				subject: '',
				desc: ''
			}
		};
	},
	methods: {
		onSubmit(event) {
			event.preventDefault();
			alert(JSON.stringify(this.form));
		}
	}
};
</script>
