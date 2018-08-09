<template>
	<div id="sample">
		<!-- FAB(Floating Action Button) -->
		<template>
			<h2>FAB(Floating Action Button)</h2>
			<div>
				<div>
					<small>Regular</small>
					<md-button class="md-fab">
						<md-icon>menu</md-icon>
					</md-button>
					<md-button class="md-fab md-primary">
						<md-icon>add</md-icon>
					</md-button>
					<md-button class="md-fab md-plain">
						<md-icon>edit</md-icon>
					</md-button>
				</div>

				<div>
					<small>Mini/Dense</small>
					<md-button class="md-fab md-mini">
						<md-icon>menu</md-icon>
					</md-button>
					<md-button class="md-fab md-mini md-primary">
						<md-icon>add</md-icon>
					</md-button>
					<md-button class="md-fab md-mini md-plain">
						<md-icon>edit</md-icon>
					</md-button>
				</div>
			</div>
		</template>
		<!--// FAB(Floating Action Button) -->
		<br>
		<!-- Bottom Bar(Shift effect) -->
		<template>
			<h2>Bottom Bar(Shift effect)</h2>
			<div>
				<div class="phone-viewport">
					<md-bottom-bar md-type="shift">
						<md-bottom-bar-item id="bottom-bar-item-home" md-label="Home" md-icon="home"></md-bottom-bar-item>
						<md-bottom-bar-item id="bottom-bar-item-pages" md-label="Pages" md-icon="pages"></md-bottom-bar-item>
						<md-bottom-bar-item id="bottom-bar-item-posts" md-label="Posts" md-icon="whatshot"></md-bottom-bar-item>
						<md-bottom-bar-item id="bottom-bar-item-favorites" md-label="Favorites" md-icon="favorite"></md-bottom-bar-item>
					</md-bottom-bar>
				</div>

				<div class="phone-viewport">
					<md-bottom-bar class="md-accent" md-type="shift">
						<md-bottom-bar-item id="bottom-bar-item-home" md-label="Home" md-icon="home"></md-bottom-bar-item>
						<md-bottom-bar-item id="bottom-bar-item-pages" md-label="Pages" md-icon="pages"></md-bottom-bar-item>
						<md-bottom-bar-item id="bottom-bar-item-posts" md-label="Posts" md-icon="whatshot"></md-bottom-bar-item>
						<md-bottom-bar-item id="bottom-bar-item-favorites" md-label="Favorites" md-icon="favorite"></md-bottom-bar-item>
					</md-bottom-bar>
				</div>
			</div>
		</template>
		<!--// Bottom Bar(Shift effect) -->
		<br>
		<!-- Datepicker -->
		<template>
			<h2>Datepicker</h2>
			<div>
				<md-field>
					<label for="movie">First day of a week</label>
					<md-select v-model="firstDayOfAWeek">
						<md-option value="0">Sunday</md-option>
						<md-option value="1">Monday</md-option>
					</md-select>
					<span class="md-helper-text">This config is global.</span>
				</md-field>
			</div>
			<div>
				<md-datepicker v-model="selectedDate">
					<label>Select date</label>
				</md-datepicker>
			</div>
		</template>
		<!--// Datepicker -->
		<br>
		<!-- Dialog -->
		<template>
			<h2>Dialog</h2>
			<div>
				<md-dialog :md-active.sync="showDialog">
					<md-dialog-title>Preferences</md-dialog-title>

					<md-tabs md-dynamic-height>
						<md-tab md-label="General">
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
						</md-tab>

						<md-tab md-label="Activity">
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
						</md-tab>

						<md-tab md-label="Account">
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
							<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam mollitia dolorum dolores quae commodi impedit possimus qui, atque at voluptates cupiditate. Neque quae culpa suscipit praesentium inventore ducimus ipsa aut.</p>
						</md-tab>
					</md-tabs>

					<md-dialog-actions>
						<md-button class="md-primary" @click="showDialog = false">Close</md-button>
						<md-button class="md-primary" @click="showDialog = false">Save</md-button>
					</md-dialog-actions>
				</md-dialog>

				<md-button class="md-primary md-raised" @click="showDialog = true">Show Dialog</md-button>
			</div>
		</template>
		<!--// Dialog -->
		<br>
		<!-- Confirms -->
		<template>
			<h2>Confirms</h2>
			<div>
				<md-dialog-confirm
						:md-active.sync="active"
						md-title="Use Google's location service?"
						md-content="Let Google help apps determine location. <br> This means sending <strong>anonymous</strong> location data to Google, even when no apps are running."
						md-confirm-text="Agree"
						md-cancel-text="Disagree"
						@md-cancel="onCancel"
						@md-confirm="onConfirm" />

				<md-button class="md-primary md-raised" @click="active = true">Confirm</md-button>
				<span v-if="value">Value: {{ value }}</span>
			</div>
		</template>
		<!--// Confirms -->
		<br>
		<!-- Forms -->
		<template>
			<h2>Forms</h2>
			<div>
				<md-field>
					<label>Initial Value</label>
					<md-input v-model="initial"></md-input>
				</md-field>

				<md-field>
					<label>Initial Value (Read Only)</label>
					<md-input v-model="initial" readonly></md-input>
				</md-field>

				<md-field>
					<label>Type here!</label>
					<md-input v-model="type"></md-input>
					<span class="md-helper-text">Helper text</span>
				</md-field>

				<md-field>
					<label>With label</label>
					<md-input v-model="withLabel" placeholder="A nice placeholder"></md-input>
				</md-field>

				<md-field md-inline>
					<label>Inline</label>
					<md-input v-model="inline"></md-input>
				</md-field>

				<md-field>
					<label>Number</label>
					<md-input v-model="number" type="number"></md-input>
				</md-field>

				<md-field>
					<label>Textarea</label>
					<md-textarea v-model="textarea"></md-textarea>
				</md-field>

				<md-field>
					<label>Textarea with Autogrow</label>
					<md-textarea v-model="autogrow" md-autogrow></md-textarea>
				</md-field>

				<md-field>
					<label>Disabled</label>
					<md-input v-model="disabled" disabled></md-input>
				</md-field>
			</div>
		</template>
		<br>
		<template>
			<h2>Radio</h2>
			<div>
				<md-radio v-model="radio" :value="false">Boolean</md-radio>
				<md-radio v-model="radio" value="my-radio">String</md-radio>
				<md-radio v-model="radio">No Value</md-radio>
				<md-radio v-model="radio" disabled>Disabled</md-radio>

				<small>Model value: {{ radio }}</small>
			</div>
		</template>
		<br>
		<template>
			<h2>Select</h2>
			<div class="md-layout-item">
				<md-field>
					<label for="font">Font</label>
					<md-select v-model="font" name="font" id="font">
						<md-option value="arial">Arial</md-option>
						<md-option value="calibri">Calibri</md-option>
						<md-option value="cambria">Cambria</md-option>
						<md-option value="comic-sans">Comic Sans</md-option>
						<md-option value="consolas">Consolas</md-option>
						<md-option value="courier">Courier</md-option>
						<md-option value="droid-sans">Droid Sans</md-option>
						<md-option value="georgia">Georgia</md-option>
						<md-option value="helvetica">Helvetica</md-option>
						<md-option value="impact">Impact</md-option>
						<md-option value="roboto">Roboto</md-option>
						<md-option value="segoe-ui">Segoe UI</md-option>
						<md-option value="times-new-roman">Times New Roman</md-option>
						<md-option value="ubuntu">Ubuntu</md-option>
						<md-option value="verdana">Verdana</md-option>
					</md-select>
				</md-field>
			</div>
		</template>
		<br>
		<template>
			<h2>Switch</h2>
			<div>
				<md-switch v-model="array" value="1">Array</md-switch>
				<md-switch v-model="array" value="2">Array</md-switch>
				<md-switch v-model="boolean">Boolean</md-switch>
				<md-switch v-model="string" value="my-switch">String</md-switch>
				<md-switch v-model="novalue">No Value</md-switch>
				<md-switch v-model="disabled" disabled>Disabled</md-switch>

				<table>
					<tr>
						<th>Array</th>
						<th>Boolean</th>
						<th>String</th>
						<th>No Value</th>
					</tr>

					<tr>
						<td>{{ array }}</td>
						<td>{{ boolean }}</td>
						<td>{{ string }}</td>
						<td>{{ novalue }}</td>
					</tr>
				</table>
			</div>
		</template>
		<br>
		<template>
			<h2>Checkbox</h2>
			<div>
				<md-checkbox v-model="array" value="1">Array</md-checkbox>
				<md-checkbox v-model="array" value="2">Array</md-checkbox>
				<md-checkbox v-model="boolean">Boolean</md-checkbox>
				<md-checkbox v-model="string" value="my-checkbox">String</md-checkbox>
				<md-checkbox v-model="novalue">No Value</md-checkbox>
				<md-checkbox v-model="disabled" disabled>Disabled</md-checkbox>
				<md-checkbox v-model="obj" :value="obj1">Object 1</md-checkbox>
				<md-checkbox v-model="obj" :value="obj2">Object 2</md-checkbox>

				<md-checkbox v-model="indeterminate" indeterminate>Indeterminate</md-checkbox>

				<table>
					<tr>
						<th>Array</th>
						<th>Boolean</th>
						<th>String</th>
						<th>No Value</th>
						<th>Object</th>
					</tr>

					<tr>
						<td>{{ array }}</td>
						<td>{{ boolean }}</td>
						<td>{{ string }}</td>
						<td>{{ novalue }}</td>
						<td>{{ obj }}</td>
					</tr>
				</table>
			</div>
		</template>
		<!--// Forms -->
		<br>
		<!-- Progress -->
		<template>
			<h2>Progress</h2>
			<div>
				<md-progress-bar md-mode="indeterminate"></md-progress-bar>
				<md-progress-bar class="md-accent" md-mode="indeterminate"></md-progress-bar>
			</div>
		</template>
		<br>
		<template>
			<div>
				<md-progress-spinner md-mode="indeterminate"></md-progress-spinner>
				<md-progress-spinner class="md-accent" md-mode="indeterminate"></md-progress-spinner>
			</div>
		</template>
		<!--// Progress -->
	</div>
</template>


<script>
	export default {
		name: 'sample',
		data: () => ({
			selectedDate: null,
			showDialog: false,
			active: false,
			value: null,
			initial: 'Initial Value',
			type: null,
			withLabel: null,
			inline: null,
			number: null,
			textarea: null,
			autogrow: null,
			radio: false,
			font: null,
			array: [],
			boolean: false,
			string: null,
			novalue: null,
			disabled: true,
			obj1: {name: 'obj1'},
			obj2: {name: 'obj2'},
			obj: null,
			indeterminate: true
		}),
		methods: {
			onConfirm () {
				this.value = 'Agreed'
			},
			onCancel () {
				this.value = 'Disagreed'
			}
		},
		computed: {
			firstDayOfAWeek: {
				get () {
					return this.$material.locale.firstDayOfAWeek
				},
				set (val) {
					this.$material.locale.firstDayOfAWeek = val
				}
			}
		}
	}
</script>

<style>
	small{display:block;}
	.phone-viewport {
		width: 322px;
		height: 200px;
		display: inline-flex;
		align-items: flex-end;
		overflow: hidden;
		border:1px solid rgba(0,0,0,.26);
		background:rgba(0,0,0,.06);
	}
	.md-dialog {
		max-width: 768px;
	}
	.md-switch {
		display: flex;
	}
	.md-checkbox {
		display: flex;
	}

	table{
		width:100%;
		table-layout:fixed;
	}

	th {
		text-align: left;
	}
	.md-progress-bar {
		margin: 24px;
	}
	.md-progress-spinner {
		margin: 24px;
	}

</style>