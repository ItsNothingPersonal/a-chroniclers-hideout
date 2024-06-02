<script lang="ts">
	import Icon from '@iconify/svelte';
</script>

<h1 class="h1">Wer spielt wen? (Standard-Gruppe)</h1>
<div class="table-container mt-4">
	<table class="table table-hover">
		<tbody>
			<tr>
				<td class="table-cell-fit !whitespace-nowrap">Zwei offensive Kämpfer</td>
				<td>
					Sie schützen die Gruppe vor Bedrohungen, denen nicht anders beizukommen ist als mit
					Gewalt. Zwar hat jeder Kult seinen kriegerischen Zweig. Doch am besten geeignet sind
					Hellvetiker, Richter, Geißler, Wiedertäufer, Jehammedaner und Sipplinge. Im späteren
					Spielverlauf bietet ein Spitalier-Preservist eine radikale Stärkung der Kampfkraft.
				</td>
			</tr>

			<tr>
				<td class="table-cell-fit whitespace-nowrap text-nowrap">
					<span class="whitespace-nowrap text-nowrap">Mindestens ein Unterstützer</span>
				</td>
				<td>
					Er stärkt die Frontreihe mit Sonderfertigkeiten oder schwächt den Gegner aus der Distanz.
					Chronisten könnten das übernehmen, oder auch Spitalier.
				</td>
			</tr>

			<tr>
				<td class="table-cell-fit !whitespace-nowrap">
					<span class="whitespace-nowrap text-nowrap"> Spion oder Attentäter </span>
				</td>
				<td>
					Er agiert aus dem Verborgenen und nähert sich unbemerkt dem Feind. Er kennt sich mit
					Fallen aus und kann sie überwinden. Bleicher, Schrotter oder Apokalyptiker.
				</td>
			</tr>

			<tr>
				<td class="table-cell-fit !whitespace-nowrap">Heiler</td>
				<td>
					Gruppen, die kriegerische Auseinandersetzungen suchen, geraten ohne einen Heilkundigen
					schnell an die Grenze ihrer Kräfte. Ein Spitalier wäre die offensichtliche Wahl, aber auch
					ein Wiedertäufer-Elysier oder ein Anubier könnten in die Bresche springen.
				</td>
			</tr>

			<tr>
				<td class="table-cell-fit !whitespace-nowrap">Silberzunge</td>
				<td>
					Wächter müssen abgelenkt, Anführer überzeugt, Gegner überstimmt und Händler
					heruntergehandelt werden. Neolibyer, Richter und Apokalyptiker sind verdammt gut darin.
				</td>
			</tr>
		</tbody>
	</table>
</div>

<h2 class="h2 mt-6">Primal und Fokus</h2>
<p>
	Das Grollen des Tiers im Herzen und einen Schrei auf den Lippen, der den Kämpfer durch die
	Zeitalter hinweg mit seinen Ahnen verbindet - oder ein kühler Kopf, der jede Situation bemisst,
	sie ihrer Gefühle entkleidet und auf das wahrhaftige Skelett der Realität blickt, der jede
	Hintertür erkennt und Finesse schwitzender Wildheit vorzieht. Zwei Lebenswege, die nicht
	unterschiedlicher sein können, und die sich gegenseitig ausschließen. Ein Charakter muss sich für
	einen dieser Wege entscheiden: Mit Primal lässt er Emotionen zu, die ihn verzehren und vorwärts
	treiben. Das Gegenstück ist Fokus. Es weckt den rationalen Teil in ihm und kühlt ihm das Blut.
	Primal und Fokus sind Fertigkeiten: Primal gehört zum Attribut Instinkt, Fokus zum Attribut
	Verstand. Ein Charakter kann sich nur eine dieser Fertigkeiten aneignen, die jeweils andere
	verkümmert und kann nicht gesteigert werden.
</p>
<p>
	Aus Primal oder Fokus wird der Höchstwert der Egopunkte abgeleitet. Ego steht zum einen für die
	seelische Stärke, zum anderen werden die Punkte eingesetzt, um (vor allem im Kampf) verborgene
	Reserven zu aktivieren. Soziale oder mentale Attacken zehren am Ego. Sinkt es auf Null, geht der
	Charakter demoralisiert und erschöpft zu Boden. Mehr dazu im Kapitel „Kampf“.
</p>
<p>
	Die Entscheidung für Primal oder Fokus bestimmt zu einem großen Teil, wie ein Charakter Probleme
	löst: Mit dem Kopf oder mit dem Herzen. Dies wird vorwiegend ausgespielt und nicht ausgewürfelt.
	Die Regelkomponente dieser Entscheidung umfasst leichteren Zugang zu Attributen und Fertigkeiten,
	die Primal oder Fokus zugeschrieben werden (siehe Kapitel „Erfahrung“). Zudem setzen einige
	besondere Fähigkeiten, Potenziale genannt, auf Primal oder Fokus auf.
</p>

<aside class="alert variant-filled mt-2">
	<div>
		<Icon icon="material-symbols:info" class="h-10 w-10 self-center" />
	</div>
	<div class="alert-message">
		<ul>
			<li>Entweder VER+Fokus oder INS+Primal</li>
			<li>Maximale Egopunkte = VER+Fokus x 2 oder INS+Primal x 2</li>
		</ul>
	</div>
</aside>

<h2 class="h2 mt-6">Glaube und Wille</h2>
<p>
	Ähnlich wie Primal und Fokus sind auch Glaube und Wille die zwei Seiten derselben Medaille.
	Entscheidet sich ein Charakter für das eine, verschließt sich das andere vor ihm. Glaube/Wille
	wird hauptsächlich genutzt, um mentale Angriffe abzuwehren.
</p>
<aside class="alert variant-filled mt-2">
	<div>
		<Icon icon="material-symbols:info" class="h-10 w-10 self-center" />
	</div>
	<div class="alert-message">
		<p>Entweder PSY+Glaube oder PSY+Wille</p>
	</div>
</aside>

<h2 class="h2 mt-6">Charaktererschaffung im Überblick</h2>
<ul>
	<li>
		<span class="font-bold">Kultur, Konzept und Kult:</span> Notieren Sie sich die Fertigkeiten- und
		Attribut-Boni auf dem Charakterbogen.
	</li>
	<li>
		<span class="font-bold">Punkte verteilen:</span> Verteilen Sie 10 Punkte auf die Attribute und 28
		Punkte auf die Fertigkeiten. Das Maximum pro Attribut oder Fertigkeit liegt bei 2 Punkten; eventuelle
		Boni aus Kultur, Konzept und Kult erweitern dieses Maximum um jeweils +1.
	</li>
	<li>
		<span class="font-bold">Punkte auf Hintergründe verteilen:</span> Insgesamt werden 4 Punkte auf die
		sechs Hintergründe verteilt. Kein Wert darf größer als 3 werden.
	</li>
	<li>
		<span class="font-bold">Rang bestimmen:</span> Der Charakter durchläuft die Ranghierarchie seines
		Kults, bis er die Voraussetzungen für den folgenden Rang nicht mehr erfüllen kann. Eingesammelte
		Ausrüstung und eventuelle Boni werden auf dem Charakterbogen vermerkt.
	</li>
	<li>
		<span class="font-bold">Potenzial wählen:</span> Der Charakter eignet sich ein kultspezifisches oder
		allgemeines Potenzial auf Stufe 1 an.
	</li>
	<li>
		<span class="font-bold">Der letzte Schliff:</span> Definiere den Namen, das Geschlecht und andere
		Rollenspiel-Eigenschaften deiner Figur.
	</li>
</ul>

<h2 class="h2 mt-6">Konzept</h2>
<ul>
	<li>Konzept für den Charakter wählen</li>
	<li>Attributs- und Fertigkeitenbonus vermerken</li>
	<li>Konzept gibt in der passenden Situation +2W (einmal am Tag)</li>
</ul>

<h2 class="h2 mt-6">Kult</h2>
<ul>
	<li>Der Charakter schließt sich einem Kult an</li>
	<li>Der Spieler notiert die Fertigkeitenboni</li>
	<li>Bestimme Fertigkeiten und Hintergründe eröffnen dem Charakter höhere Ränge</li>
</ul>

<h2 class="h2 mt-6">Hintergründe</h2>
<ul>
	<li>Hintergründe bestimmen neben Fertigkeiten den Rang im Kult</li>
	<li>Keine Steigerung durch Erfahrungspunkte</li>
	<li>4 Punkte für die Charaktererschaffung, nicht mehr als 3 Punkte auf einen Hintergrund</li>
</ul>

<h2 class="h2 mt-6">Potenziale</h2>
<ul>
	<li>Neue Charaktere erhalten ein Potenzial auf Stufe 1</li>
</ul>

<h2 class="h2 mt-6">Ränge</h2>
<ul>
	<li>
		<span class="font-bold"> Start:</span> Beginnt unabhängig von den Werten auf Rang 1
	</li>
	<li>
		<span class="font-bold"> Fertigkeitenvoraussetzung: </span> Immer Attribut + Fertigkeit, niemals
		Fertigkeitsstufe alleine
	</li>
	<li>
		<span class="font-bold"> Aufstieg: </span>
	</li>
	<ul>
		<li>Rangvoraussetzung muss erreicht werden.</li>
		<li>Der Rang gewährt Sonderregeln und Boni.</li>
		<li>Der Charakter erhält Kultausrüstung.</li>
		<li>Bedingungen werden nur einmalig geprüft.</li>
		<li>Soviele Ränge aufsteigen, wie möglich.</li>
		<li>Ränge dürfen nicht übersprungen werden.</li>
		<li>Ausrüstung darf behalten werden.</li>
		<li>Sonderregeln gelten meist nur für aktuellen Rang</li>
	</ul>
</ul>

<h2 class="h2 mt-6">Der letzte Schliff</h2>
<h3 class="h3">Ego</h3>
<ul>
	<li>Entweder VER+Fokus oder INS+Primal</li>
	<li>Maximale Egopunkte = VER+Fokus x 2 oder INS+Primal x 2</li>
</ul>
<h3 class="h3">Versporung</h3>
<ul>
	<li>Entweder PSY+Glaube oder PSY+Wille</li>
	<li>Maximale Versporung = PSY+Glaube/Wille x 2</li>
</ul>
<h3 class="h3">Fleischwunden</h3>
<ul>
	<li>Maximale Fleischwunden = KÖR+Härte x 2</li>
</ul>
<h3 class="h3">Trauma</h3>
<ul>
	<li>Maximaler Traumaschaden = Körper + Psyche</li>
</ul>
<h3 class="h3">Verteidigung</h3>
<ul>
	<li>Passive Verteidigung = 1</li>
	<li>Kann durch besondere Ausrüstung oder Potenziale steigen</li>
</ul>
<h3 class="h3">Dinare und Chronistenwechsel</h3>
<ul>
	<li>Grundwert = Rangstufe + Ressourcen</li>
	<li>Startgeld = Grundwert x Faktor für Kult</li>
	<li>Umrechnungskurs von Preisen: 1:1</li>
</ul>
<div class="table-container">
	<table class="table table-hover">
		<thead>
			<tr>
				<th>Kult</th>
				<th>Faktor</th>
			</tr>
		</thead>

		<tbody>
			<tr>
				<td>Spitalier</td>
				<td>x100 Wechsel</td>
			</tr>

			<tr>
				<td>Chronisten</td>
				<td>x128 Wechsel</td>
			</tr>

			<tr>
				<td>Hellvetiker</td>
				<td>x50 Wechsel</td>
			</tr>

			<tr>
				<td>Richter</td>
				<td>x50 Wechsel</td>
			</tr>

			<tr>
				<td>Schrotter</td>
				<td>x50 Wechsel</td>
			</tr>

			<tr>
				<td>Sipplinge</td>
				<td>x50 Wechsel</td>
			</tr>

			<tr>
				<td>Neolibyer</td>
				<td>x1000 Dinare</td>
			</tr>

			<tr>
				<td>Geißler</td>
				<td>x100 Dinare</td>
			</tr>

			<tr>
				<td>Anubier</td>
				<td>x100 Dinare</td>
			</tr>

			<tr>
				<td>Jehammedaner</td>
				<td>x100 Wechsel</td>
			</tr>

			<tr>
				<td>Apokalyptiker</td>
				<td>x200 Wechsel</td>
			</tr>

			<tr>
				<td>Wiedertäufer</td>
				<td>x50 Wechsel</td>
			</tr>

			<tr>
				<td>Bleicher</td>
				<td>x50 Wechsel</td>
			</tr>
		</tbody>
	</table>
</div>

<h2 class="h2 mt-6">Kosten fürs Steigern</h2>
<h3 class="h3">Attribute/Fähigkeiten</h3>
<ul>
	<li>Primal-Attribute: KÖR, CHA, INS</li>
	<li>Fokus-Attribute: VER, GES, PSY</li>
</ul>

<div class="table-container">
	<table class="table table-hover">
		<thead>
			<tr>
				<th>Art</th>
				<th>Preis</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>Attribut</td>
				<td>Neuer Wert x12 EP</td>
			</tr>

			<tr>
				<td>Bevorzugtes Attribut</td>
				<td>Neuer Wert x 10 EP</td>
			</tr>

			<tr>
				<td>Fertigkeit</td>
				<td>Neuer Wert x 5 EP</td>
			</tr>

			<tr>
				<td>Bevorzugte Fertigkeit</td>
				<td>Neuer Wert x 4 EP</td>
			</tr>
		</tbody>
	</table>
</div>
<h3 class="h3 mt-2">Potenziale</h3>
<ul>
	<li>EP Kosten für Potenzialsteigerung = Stufe aller Potenziale x 10</li>
</ul>
