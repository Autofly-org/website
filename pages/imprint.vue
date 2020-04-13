<template>
  <div class="imprint">
    <h1>imprint</h1>
    <h2>Betreiber</h2>
    <p>Autofly <br>
    Marienberger Strasse 60 <br>
    01279 Dresden <br>
    E-Mail info@autofly.org <br>
    Tel 17634407872</p>

    <h2>Inhaltlich Verantwortlicher
    gem. § 55 II RStV</h2>
    <p>Johann Süß <br>
    Marienberger Strasse 60 <br>
    01279 Dresden <br>
    suess@navabase.com <br>
    Tel 17634407872</p>

    <h2>Haftung für Inhalte</h2>
    <p>Die Inhalte unserer Seiten wurden mit größter Sorgfalt erstellt. Für die Richtigkeit, Vollständigkeit und Aktualität der Inhalte können wir jedoch keine Gewähr übernehmen. Als Diensteanbieter sind wir gemäß § 7 Abs.1 TMG für eigene Inhalte auf diesen Seiten nach den allgemeinen Gesetzen verantwortlich. Nach §§ 8 bis 10 TMG sind wir als Diensteanbieter jedoch nicht verpflichtet, übermittelte oder gespeicherte fremde Informationen zu überwachen oder nach Umständen zu forschen, die auf eine rechtswidrige Tätigkeit hinweisen. Verpflichtungen zur Entfernung oder Sperrung der Nutzung von Informationen nach den allgemeinen Gesetzen bleiben hiervon unberührt. Eine diesbezügliche Haftung ist jedoch erst ab dem Zeitpunkt der Kenntnis einer konkreten Rechtsverletzung möglich. Bei Bekanntwerden von entsprechenden Rechtsverletzungen werden wir diese Inhalte umgehend entfernen.</p>

    <h2>Datenschutz</h2>
    <p>Die Nutzung unserer Webseite ist in der Regel ohne eine Angabe personenbezogener Daten möglich. Soweit auf unseren Seiten personenbezogene Daten (beispielsweise Name, Anschrift oder E-Mail-Adresse) erhoben werden, erfolgt dies – soweit es möglich ist– immer auf freiwilliger Basis. Wir geben Ihre Daten ohne Ihre ausdrückliche Zustimmung nicht an Dritte weiter. Außerdem weisen wir Sie darauf hin, dass die Datenübertragung im Internet (wie beispielsweise bei der Kommunikation über E-Mail) Sicherheitslücken aufweisen kann. Denn ein lückenloser Schutz der Daten vor dem Zugriff durch Dritte ist nicht möglich. Wir widersprechen hiermit ausdrücklich der Nutzung von im Rahmen der Impressumspflicht veröffentlichten Kontaktdaten durch Dritte zur Übersendung von nicht ausdrücklich angeforderter Werbung und Informationsmaterialien. Die Betreiber dieser Seiten behalten sich ausdrücklich vor, im Fall der unverlangten Zusendung von Werbeinformationen, etwa durch Spam-Mails, rechtliche Schritte einzuleiten.</p>

    <h2>Google Analytics</h2>
    <p>Diese Website benutzt Google Analytics, einen Webanalysedienst der Google Inc. (''Google''). Google Analytics verwendet sog. ''Cookies'', Textdateien, die auf Ihrem Computer gespeichert werden und die eine Analyse der Benutzung der Website durch Sie ermöglicht. Die durch den Cookie erzeugten Informationen über Ihre Benutzung diese Website (einschließlich Ihrer IP-Adresse) wird an einen Server von Google in den USA übertragen und dort gespeichert. Google wird diese Informationen benutzen, um Ihre Nutzung der Website auszuwerten, um Reports über die Websiteaktivitäten für die Websitebetreiber zusammenzustellen und um weitere mit der Websitenutzung und der Internetnutzung verbundene Dienstleistungen zu erbringen. Auch wird Google diese Informationen gegebenenfalls an Dritte übertragen, sofern dies gesetzlich vorgeschrieben oder soweit Dritte diese Daten im Auftrag von Google verarbeiten. Google wird in keinem Fall Ihre IP-Adresse mit anderen Daten der Google in Verbindung bringen. Sie können die Installation der Cookies durch eine entsprechende Einstellung Ihrer Browser Software verhindern; wir weisen Sie jedoch darauf hin, dass Sie in diesem Fall gegebenenfalls nicht sämtliche Funktionen dieser Website voll umfänglich nutzen können. Durch die Nutzung dieser Website erklären Sie sich mit der Bearbeitung der über Sie erhobenen Daten durch Google in der zuvor beschriebenen Art und Weise und zu dem zuvor benannten Zweck einverstanden. Sie können der Erhebung und Speicherung Ihrer Daten jederzeit widersprechen.</p>
    <p>Diese Website benutzt Google Analytics mit der Zusatzfunktion „anonymizeIP()“. Dies bedeutet, dass IP-Adressen nicht vollständig, sondern nur gekürzt gespeichert und verarbeitet werden, um einen direkten Rückschluss auf die Person auszuschließen.</p>

    <p>Gratis Impressum von agb.de</p>
  </div>
</template>

<script lang="ts">

</script>

<style lang="scss" scoped>
.imprint {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  width: 80vw;
  padding-top: 50px;
  margin: 0 auto;

  h1 {
    grid-column: 1 / span 2;
    font-size: 55px;
    text-align: left;
  }

  h2 {
    grid-column: 1;
    justify-self: right;
    font-size: 18px;
  }

  p {
    grid-column: 2;
    justify-self: left;
    text-align: left;
  }
}

@media only screen and (max-width: 765px) {
  .imprint {
    grid-template-columns: 1fr 0fr;
    gap: 0;
    row-gap: 30px;

    h1, h2 {
      text-align: center !important;
      grid-column: 1 !important;
      justify-self: center !important;
    }
  
    p {
      grid-column: 1 !important;
      text-align: center !important;
      justify-self: center !important;
    }
  }
}
</style>
