<script lang="ts">
	import Terminal from '$lib/Terminal.svelte';
	import type { TerminalEntry } from '$lib/terminalEntry';

	const pageContent: TerminalEntry[] = [
		{ type: 'command', text: 'login: fragmentModus' },
		{
			type: 'result',
			text: 'fragmentModus login: ***************************************************************'
		},
		{ type: 'result', text: 'Authentifizierung erfolgreich, willkommen Fragment Modus!' },
		{ type: 'result', text: 'Letzter Login: Mittwoch, 25. Februar 2595' },
		{ type: 'command', text: './listHistory.sh -excludeminor -preEshaton' },
		{ type: 'result', text: 'Einen Moment bitte, die Daten werden aus dem Stream geladen!' },
		{
			type: 'result',
			text: 'Ladevorgang erfolgreich, Daten für wichtige Ereignisse vor dem Eshaton werden ausgegeben...'
		},
		{ type: 'result', text: '**WARNUNG:** Daten können aufgrund des Eshatons unvollständig sein!' },
		{
			type: 'result',
			text: '**2043-2045:** Die UNO zerbricht aufgrund der Spannungen zwischen seinen Mitgliedern, es bilden sich kleinere Nachfolgeorganisationen wie z.B. die UEO (United Europe Organization) oder die UAO (United Africa Organization)'
		},
		{
			type: 'result',
			text: '**2046:** In Helsinki wird im Dezember ein in einer Elefantenkuh eingepflanztes Mammutkalb der Gattung Mammuthus primigenius geboren dessen DNA zuvor aus einer hervorragend erhaltenen Mammutleiche entnommen wurde.'
		},
		{
			type: 'result',
			text: '**2051:** Genetisch angepasste Implantate und Prothesen sind Alltag und erste Versuche der Rcombination Group mit Naniten versprechen einen Quantensprung in der Medizin.'
		},
		{
			type: 'result',
			text: '**2053:** Der Stream wird für einen Großteil der Bevölkerung der Industrienationen zur Ersatzrealität. Über implantierte Chips mit gespeicherter Sozialversicherungsnummer, Retina- und DNS-Abgleich, Krankendaten und Kontoverbindungen beschweren sich nur noch wenige.'
		},
		{
			type: 'result',
			text: '**2055:** AIDS, die alte Geißel der Menschheit, ist faktisch besiegt: Ein von der WHO ausgearbeiteter Plan sieht vor, die Welt in den nächsten zwanzig Jahren von der Seuche zu befreien.'
		},
		{
			type: 'result',
			text: '**2057:** Das Jahr der Sekten: Neben den zahlreichen Esoterikauswüchsen wie Templerorden, New- und Old-Age-Bewegungen und technophilen Streamer-Auswüchsen kämpfen vorallem zwei Männer um Anhänger: In der einen Ecke der selbsternannte Messias Jehammed mit einem Gemisch aus allen drei Buchreligionen, gegenüber der ebenso charismatische wie dogmatische Televangelist und Mitbegründer der Recombination Group Gerome Getrell.'
		},
		{
			type: 'result',
			text: '**2064:** An der Elfenbeinküste sterben Seeleute eines amerikanischen Kreuzers an einem bislang unbekannten Virus. Die seltsame Krankheit breitet sich rasant aus und hat bald ganz Abidjan in ihrem eisigen Griff. Viele halten den Virus für ein "Geschenk" der USA um den Kontinent nach dem Sieg über AIDS weiterhin schwach zu halten. Als im August 2064 das Institut Pasteur in Paris bekannt gibt, dass es sich bei der mysteriösen Seemannskrankheit um einen neuartigen und äußerst aggressiven AIDS-Stamm handelt, ist es Wasser auf den Mühlen der Antiamerikanisten. Es kommt zu Aufständen und Plünderungen amerikanischer Einrichtungen.'
		},
		{
			type: 'result',
			text: '**2065:** HIV-E, das Virus von der Elfenbeinküste, hat den ganzen Kontinent erfasst. Es verbreitet sich über die Luft, kaum jemand geht ohne zumindest einen Mundschutz oder einen Ganzkörperschutzanzug auf die Straße.'
		},
		{
			type: 'result',
			text: '**2066:** Die Recombination Group vermeldet erste Erfolge bei der Bekämpfung von HIV-E und ist zuversichtlich bald ein Serum gegen die Seuche anbieten zu können. Die vor der Seuche fliehenden Völkermassen in Afrika steuern jetzt den Norden an, Hunderttausende strömen in Agadez zusammen, einer Stadt im zentralafrikanischen Niger. Der Flüchtlingsstrom bläht Agadez zu einer Millionenstadt, die jeden Augenblick kollabieren kann.'
		},
		{
			type: 'result',
			text: '**2067-2069:** Nach dem Fall Algeriens bricht der Kontinent nahezu zusammen. Die UEO verlegt auf Bitten Libyens ihre Kriegsflotte ins Mittelmeer um ein Überspringen des HIV-E Virus auf den europäischen Kontinent durch eine Blockade zu verhindern. Tausende Flüchtlinge sterben bei dem vergeblichen Versuch der Überquerung des Mittelmeers, ertrinken oder werden von der Flotte direkt erschossen bzw. samt ihrer Boote versenkt. Tausende sterben auch direkt in Afrika, im Kugelhagel verängstigter UEO Truppen oder bewaffneter Gangs. AMSUMOs, für den Polizeieinsatz konstruierte, zweibeinige autonome Robot-Systeme, werden erstmals in Kampf-Einsätze geschickt. Die UEO setzt auf Abschreckung, doch sie unterschätzt die Verzweiflung der Flüchtlinge.'
		},
		{
			type: 'result',
			text: '**2070:** Ein OWL (Overwhelmingly Large Telescope) in Peru registriert mehrere unverzeichnete Asteroiden, die sich mit hoher Wahrscheinlichkeit auf Kollisionskurs mit der Erde befinden. Die Menschen messen der Meldung nur wenig Bedeutung bei, der Krieg in Afrika ist so viel näher mit seinen weit größeren Auswirkungen auf das eigene Leben.'
		},
		{
			type: 'result',
			text: '**2071:** Keine Weltraum-Agentur schließ mehr den Zusammenstoß mit den Asteroiden aus. Nach außen geben sich NASA, CNSA, Roskosmos und ESA besonnen aber im inneren herrscht Aufruhr. Die Papiere des vor zwanzig Jahren entwickelten Paladin-Satellitensystems zur Asteroidenabwehr werden erneut zur Prüfung eingereicht und mangels anderer Lösungen für gut befunden. Derweil geht das Sterben in Afrika und im Mittelmeer weiter. Die Recombination Group vermeldet immerhin einen Erfolg: Die Produktion des Serums läuft an.'
		},
		{
			type: 'result',
			text: '**2071:** Der erste der 211 Paladin-Satelliten wird von einer Ariane-Trägerrakete in den Orbit geschossen. Die restlichen folgen innerhalb eines Jahres.'
		},
		{
			type: 'result',
			text: '**2072:** Wellen an Viren legen große Teile des Streams lahm. Datenströme werden umgelenkt, um einen weitgehend reibungslosen Ablauf zu gewährleisten. Die Experten sind beunruhigt, die neusten Viren-Iterationen weisen alle eine 2 hoch 16-Signatur auf. Das Werk von Trittbrettfahrern oder die von pseudoreligiösen Technikjüngern angekündigte Immunreaktion des Streams?'
		},
		{
			type: 'result',
			text: '**2072:** Die Regierung der Schweiz vertraut nicht auf die Allmacht der Technik allein und lässt große Teile der vergessenen Alpenfestung instand setzen. Über Monate hinweg schieben sich endlose Lastwagenschlangen durch das Land der Eidgenossen, um vor den Eingängen des megalomanen Tunnelsystems ihrer Entladung zu harren: Waffen werden ebenso eingelagert wie auch Nahrung und Medizin - Anlaufhilfe für den Wiederaufbau nach einer möglichen Katastrophe.'
		},
		{
			type: 'result',
			text: '**2073:** „Clash of the giants!“ - der von den Medien hochstilisierte Kampf zwischen den Paladin-Satelliten und den Asteroiden findet nicht statt: nicht eine Sprengladungen der Satelliten zündet. Die genauen Gründe für den Ausfall bleiben mysteriös und werden nie vollständig geklärt. Der einzige Hinweis ist eine 2 hoch 16-Signatur in der Steuersoftware der Paladin-Satelliten.'
		},
		{
			type: 'result',
			text: '**2073:** Panik bricht aus, die Menschen verlassen die Städte um in den Bergen Zuflucht zu suchen.  Entsetzliche Szenen spielen sich auf den Straßen ab, Egoismus und Gewalt gehören zu der Überlebensstrategie der Verzweifelten. Polizeieinheiten und Militär sind hoffnungslos überfordert. Die eigentlich zur Raktenabwehr konstruierten Thor-Laser werden auf die Asteroiden gerichtet um die Katastrophe in letzter Minute noch abzuwenden doch ohne Erfolg. Endzeitsekten erfahren, ebenso wie Religionen im Allgemeinen, enormen Zulauf.'
		},
		{
			type: 'result',
			text: '**2073:** Das Schweizer Militär zieht sich in die Alpenfestung  zurück, ihm folgen Regierungsvertreter in die von Xenon-Strahlern erhellten Tunnel. Hinter ihnen schließt sich der Berg und lässt eine protestierende Bevölkerung zurück.'
		},
		{
			type: 'result',
			text: 'Ausgabe abgeschlossen, es sind keine weiteren Daten vorhanden. (letzte Veränderung der Daten: 13. März 2073)'
		},
		{ type: 'command', text: './listHistory.sh -search "Projekt Tannhäuser"' },
		{
			type: 'result',
			text: 'Suche fehlgeschlagen, Daten sind entweder nicht verfügbar, korrupt oder sie sind nicht berechtigt auf diese zuzugreifen.'
		},
		{ type: 'command', text: 'exit' },
		{ type: 'result', text: 'login:' }
	];
</script>

<Terminal content={pageContent} />
