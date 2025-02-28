<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Auto-questionnaire IVG</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 20px; }
        .question { margin-bottom: 15px; }
        .hidden { display: none; }
    </style>
</head>
<body>
    <h2>Auto-questionnaire pré-consultation IVG</h2>
    <p>Ce questionnaire a pour but de mieux comprendre vos besoins afin de vous proposer un accompagnement adapté. Vos réponses resteront confidentielles. Vous êtes libre de répondre uniquement aux questions avec lesquelles vous êtes à l’aise.</p>
    <p>En remplissant ce questionnaire, vous autorisez le professionnel à consulter vos données dans un but de recherche.</p>
    <h3>Objectifs de l’auto-questionnaire :</h3>
    <ul>
        <li>Proposer un dépistage orienté avec un professionnel formé aux violences (conseiller conjugal et familial, psychologue ou assistante sociale).</li>
        <li>Orienter vers des structures de soin spécialisées en violences conjugales et familiales (associations, centres de protection), en addictions (tabac, alcool, cannabis), en consultation médicales spécialisées (gynécologue, hématologue, sexologue…).</li>
        <li>Évaluer la nécessité d’une mise à l’abri immédiate ou d’un soutien juridique.</li>
        <li>Prescrire un dépistage adapté et une mise à jour des vaccinations.</li>
    </ul>

    <p>Dans le cadre de la consultation d’IVG, nous allons vous recevoir sans l’accompagnant(e), si vous le souhaitez par la suite il/elle pourra être reçu pour les informations médicales.</p>

    <form id="questionnaire">
        <!-- SECTION 1 -->
        <h3>Section 1 : Informations générales</h3>
        <div class="question">
            <label>Quels sont vos besoins pour cette consultation ?</label><br>
            <input type="checkbox" name="besoins" value="IVG médicamenteuse"> IVG médicamenteuse<br>
            <input type="checkbox" name="besoins" value="IVG chirurgicale"> IVG chirurgicale<br>
            <input type="checkbox" name="besoins" value="Echographie"> Echographie<br>
            <input type="checkbox" name="besoins" value="Informations"> Informations<br>
            <input type="checkbox" name="besoins" value="Aides"> Aides<br>
            <input type="checkbox" name="besoins" value="Autre"> Autre : <input type="text" name="besoins_autre">
        </div>
        <div class="question">
            <label>Vous sentez-vous soutenue par votre entourage ?</label><br>
            <input type="radio" name="soutien" value="Oui"> Oui
            <input type="radio" name="soutien" value="Non"> Non
        </div>
        <div class="question">
            <label>Venez-vous de votre plein gré ?</label><br>
            <input type="radio" name="volonte" value="Oui"> Oui
            <input type="radio" name="volonte" value="Non"> Non
        </div>
        <p>Nous vous proposerons un accompagnement avec une conseillère conjugale et familiale.</p>

        <!-- SECTION 2 -->
        <h3>Section 2 : Antécédents médicaux et gynécologiques</h3>
        <div class="question">
            <label>Quel est votre groupe sanguin ?</label><br>
            <input type="text" name="groupe_sanguin">
            <input type="checkbox" name="groupe_sanguin" value="Je ne sais pas"> Je ne sais pas
        </div>
        <div class="question">
            <label>Avez-vous des antécédents médicaux (troubles de la coagulation, phlébite, diabète, hypertension…) ?</label><br>
            <input type="radio" name="antecedents_medicaux" value="Oui"> Oui
            <input type="radio" name="antecedents_medicaux" value="Non"> Non
            <input type="radio" name="antecedents_medicaux" value="Je ne sais pas"> Je ne sais pas
            <input type="text" name="antecedents_medicaux_details" placeholder="Précisez si oui">
        </div>
        <div class="question">
            <label>Avez-vous des antécédents chirurgicaux ?</label><br>
            <input type="radio" name="antecedents_chirurgicaux" value="Oui"> Oui
            <input type="radio" name="antecedents_chirurgicaux" value="Non"> Non
            <input type="radio" name="antecedents_chirurgicaux" value="Je ne sais pas"> Je ne sais pas
            <input type="text" name="antecedents_chirurgicaux_details" placeholder="Précisez si oui">
        </div>
        <div class="question">
            <label>Si oui, prenez-vous des médicaments ?</label><br>
            <input type="radio" name="medicaments" value="Oui"> Oui
            <input type="radio" name="medicaments" value="Non"> Non
            <input type="text" name="medicaments_details" placeholder="Précisez si oui">
        </div>
        <div class="question">
            <label>Avez-vous des allergies non alimentaires ? (médicaments, latex, produits de contraste…)</label><br>
            <input type="radio" name="allergies" value="Oui"> Oui
            <input type="radio" name="allergies" value="Non"> Non
            <input type="radio" name="allergies" value="Je ne sais pas"> Je ne sais pas
            <input type="text" name="allergies_details" placeholder="Précisez si oui">
        </div>
        <div class="question">
            <label>Quelle est la date de vos dernières règles ?</label><br>
            <input type="text" name="dernieres_regles">
            <input type="checkbox" name="dernieres_regles" value="Inconnue"> Inconnue
        </div>
        <div class="question">
            <label>Avez-vous déjà eu des épisodes de saignements inhabituels ?</label><br>
            <input type="radio" name="saignements" value="Oui"> Oui
            <input type="radio" name="saignements" value="Non"> Non
            <input type="text" name="saignements_details" placeholder="Précisez si oui">
        </div>
        <div class="question">
            <label>Avez-vous des antécédents familiaux particuliers ?</label><br>
            <input type="radio" name="antecedents_familiaux" value="Oui"> Oui
            <input type="radio" name="antecedents_familiaux" value="Non"> Non
            <input type="radio" name="antecedents_familiaux" value="Je ne sais pas"> Je ne sais pas
            <input type="text" name="antecedents_familiaux_details" placeholder="Précisez si oui">
        </div>
        <div class="question">
            <label>Avez-vous déjà eu une grossesse ?</label><br>
            <input type="radio" name="grossesse" value="Oui"> Oui
            <input type="radio" name="grossesse" value="Non"> Non
            <input type="text" name="grossesse_details" placeholder="Précisez (nombre d’accouchements, IVG, etc.)">
        </div>
        <div class="question">
            <label>Souhaitez-vous aborder des problèmes liés à votre sexualité lors d'une autre consultation ?</label><br>
            <input type="radio" name="sexualite" value="Oui"> Oui
            <input type="radio" name="sexualite" value="Non"> Non
        </div>
    </form>

    <!-- SECTION 3 -->
    <h3>Section 3 : Consommations et habitudes</h3>
    <div class="question">
        <label>Tabac : Fumez-vous actuellement ?</label><br>
        <input type="radio" name="tabac" value="Oui"> Oui
        <input type="radio" name="tabac" value="Non"> Non
    </div>
    <div class="question">
        <label>Combien de cigarettes fumez-vous par jour ?</label><br>
        <input type="radio" name="cigarettes" value="10 ou moins"> 10 ou moins
        <input type="radio" name="cigarettes" value="11 à 20"> 11 à 20
        <input type="radio" name="cigarettes" value="21 à 30"> 21 à 30
        <input type="radio" name="cigarettes" value="31 ou plus"> 31 ou plus
    </div>
    <div class="question">
        <label>Dans quel délai après le réveil fumez-vous votre première cigarette ?</label><br>
        <input type="radio" name="delai_cigarette" value="Moins de 5 minutes"> Moins de 5 minutes
        <input type="radio" name="delai_cigarette" value="6 à 30 minutes"> 6 à 30 minutes
        <input type="radio" name="delai_cigarette" value="31 à 60 minutes"> 31 à 60 minutes
        <input type="radio" name="delai_cigarette" value="Après plus d’1 heure"> Après plus d’1 heure
    </div>
    <div class="question">
        <label>Combien de verre(s) d’alcool consommez-vous habituellement ?</label><br>
        <input type="radio" name="alcool" value="Je ne bois pas"> Je ne bois pas
        <input type="radio" name="alcool" value="< 10 verres par semaine"> < 10 verres par semaine : consommation occasionnelle
        <input type="radio" name="alcool" value="> 10 verres par semaine"> > 10 verres par semaine : consommation régulière
    </div>
    <div class="question">
        <label>Est-il arrivé que des proches, des professionnels de la santé s’inquiètent de votre consommation d’alcool ?</label><br>
        <input type="radio" name="inquietude_alcool" value="Oui"> Oui
        <input type="radio" name="inquietude_alcool" value="Non"> Non
    </div>
    <div class="question">
        <label>Drogues et substances psychoactives : Avez-vous consommé des substances au cours de la dernière année ?</label><br>
        <input type="radio" name="drogues" value="Oui"> Oui
        <input type="radio" name="drogues" value="Non"> Non
        <input type="text" name="drogues_details" placeholder="Précisez si oui (CBD, cocaïne, cannabis, etc.)">
    </div>

    <!-- SECTION 4 -->
    <h3>Section 4 : Dépistages</h3>
    <div class="question">
        <label>Avez-vous des antécédents d’infections sexuellement transmissibles (IST) ?</label><br>
        <input type="radio" name="ist" value="Oui"> Oui
        <input type="radio" name="ist" value="Non"> Non
        <input type="radio" name="ist" value="Je n’ai jamais fait de dépistage"> Je n’ai jamais fait de dépistage
        <input type="text" name="ist_details" placeholder="Précisez si oui">
    </div>
    <div class="question">
        <label>Désirez-vous bénéficier d’un dépistage des IST (VIH, hépatites, chlamydia, gonocoque…) ?</label><br>
        <input type="radio" name="depistage_ist" value="Oui"> Oui
        <input type="radio" name="depistage_ist" value="Non"> Non
    </div>
    <p>Le dépistage annuel des IST est recommandé de manière annuelle chez les moins de 25 ans ainsi qu’avant la réalisation d’une IVG médicamenteuse et chirurgicale.</p>
    <div class="question">
        <label>Quand avez-vous réalisé votre dernier frottis cervical (dépistage du cancer du col de l’utérus) ?</label><br>
        <input type="text" name="frottis_annee" placeholder="En quelle année ?">
        <input type="radio" name="frottis" value="Jamais (j’ai moins de 25 ans)"> Jamais (j’ai moins de 25 ans)
        <input type="radio" name="frottis" value="Jamais (> 25 ans)"> Jamais (> 25 ans)
        <input type="radio" name="frottis" value="Je ne sais pas"> Je ne sais pas
    </div>
    <div class="question">
        <label>Avez-vous été suivie par un gynécologue, une sage-femme ou un médecin généraliste pour votre suivi gynécologique ces 12 derniers mois ?</label><br>
        <input type="radio" name="suivi_gyn" value="Oui"> Oui
        <input type="radio" name="suivi_gyn" value="Non"> Non
    </div>
    <div class="question">
        <label>Avez-vous été vaccinée par le vaccin contre le papillomavirus (HPV) ?</label><br>
        <input type="radio" name="vaccin_hpv" value="Oui"> Oui
        <input type="radio" name="vaccin_hpv" value="Non"> Non
        <input type="radio" name="vaccin_hpv" value="Je ne sais pas"> Je ne sais pas
    </div>
    <div class="question">
        <label>Connaissez-vous l'auto-palpation mammaire ?</label><br>
        <input type="radio" name="auto_palpation" value="Oui"> Oui
        <input type="radio" name="auto_palpation" value="Non"> Non
    </div>
    <div class="question">
        <label>Si oui, la pratiquez-vous ?</label><br>
        <input type="radio" name="pratique_palpation" value="Oui"> Oui
        <input type="radio" name="pratique_palpation" value="Non"> Non
    </div>

    <!-- SECTION 5 -->
    <h3>Section 5 : Contraception/menstruations</h3>
    <div class="question">
        <label>Avez-vous des règles douloureuses ?</label><br>
        <input type="radio" name="regles_douloureuses" value="Oui"> oui
        <input type="radio" name="regles_douloureuses" value="Non"> non
    </div>
    <div class="question">
        <label>Aviez-vous une contraception ?</label><br>
        <input type="radio" name="avait_contraception" value="Oui"> Oui (précisez laquelle : <input type="text" name="contraception_details"> )<br>
        <input type="radio" name="avait_contraception" value="Non"> Non
    </div>
    <div class="question">
        <label>Aviez-vous déjà arrêté une méthode de contraception à cause des effets secondaires (modifications du poids, labilité émotionnelle, trouble de la libido, sécheresses, acné etc…) ou par souhait de non prise d’hormone ?</label><br>
        <input type="radio" name="arrete_contraception" value="Oui"> Oui, précisez lesquels : <input type="text" name="arrete_contraception_details"><br>
        <input type="radio" name="arrete_contraception" value="Non"> Non
    </div>
    <div class="question">
        <label>La question de la contraception sera abordée, avez-vous des questions ? (8)</label><br>
        <input type="radio" name="questions_contraception" value="Oui"> Oui
        <input type="radio" name="questions_contraception" value="Non"> Non
    </div>
    <div class="question">
        <label>A combien estimez-vous votre niveau de connaissances en contraception ?</label><br>
        <input type="radio" name="connaissances_contraception" value="Aucune connaissance"> Aucune connaissance<br>
        <input type="radio" name="connaissances_contraception" value="Peu de connaissances"> Peu de connaissances<br>
        <input type="radio" name="connaissances_contraception" value="Connaissances moyennes"> Connaissances moyennes<br>
        <input type="radio" name="connaissances_contraception" value="Beaucoup de connaissances"> Beaucoup de connaissances
    </div>

<!-- SECTION 6 -->
    <h3>Section 6 : État émotionnel</h3>
    <p>Au cours de la dernière année vous est-il arrivé de :</p>
    <div class="question">
        <label>Vous sentez-vous anxieuse ou inquiète sans raison apparente ?</label><br>
        <input type="radio" name="anxiete_sans_raison" value="Oui"> Oui
        <input type="radio" name="anxiete_sans_raison" value="Non"> Non
    </div>
    <div class="question">
        <label>Avoir des problèmes pour dormir ?</label><br>
        <input type="radio" name="problemes_sommeil" value="Oui"> Oui
        <input type="radio" name="problemes_sommeil" value="Non"> Non
    </div>
    <div class="question">
        <label>Vous sentir dépassée par les événements ?</label><br>
        <input type="radio" name="sentir_depassee" value="Oui"> Oui
        <input type="radio" name="sentir_depassee" value="Non"> Non
    </div>
    <div class="question">
        <label>Pensez-vous à vous faire du mal ou à vous mettre en danger ?</label><br>
        <input type="radio" name="auto_mutilation" value="Oui"> Oui
        <input type="radio" name="auto_mutilation" value="Non"> Non
    </div>
    <div class="question">
        <label>Souhaitez-vous être accompagnée par un professionnel (conseillère, psychologue, psychiatre, etc.) pour parler de vos émotions ?</label><br>
        <input type="radio" name="accompagnement_pro" value="Oui"> Oui
        <input type="radio" name="accompagnement_pro" value="Non"> Non
    </div>

<!-- SECTION 7 -->
    <h3>Section 7 : Violence et sécurité</h3>
    <p>Vous pouvez répondre aux questions sans que nous abordions le sujet si vous ne le souhaitez pas, mais sachez que nous sommes à votre écoute.</p>
    <div class="question">
        <label>Dans votre vie vous est-il déjà arrivé quelque chose qui n'aurait pas dû arriver?</label><br>
        <input type="radio" name="qqch_inapproprie" value="Oui"> Oui
        <input type="radio" name="qqch_inapproprie" value="Non"> Non
    </div>
    <div class="question">
        <label>Avez-vous déjà été victime de violences ?</label><br>
        <input type="checkbox" name="violences" value="Physiques"> Physiques<br>
        <input type="checkbox" name="violences" value="Psychologiques"> Psychologiques<br>
        <input type="checkbox" name="violences" value="Sexuelles"> Sexuelles<br>
        <input type="checkbox" name="violences" value="Non"> Non<br>
        <input type="checkbox" name="violences" value="Autres"> Autres
    </div>
    <div class="question">
        <label>Vous sentez-vous en sécurité dans votre environnement actuel ?</label><br>
        <input type="radio" name="securite_environnement" value="Oui"> Oui
        <input type="radio" name="securite_environnement" value="Non"> Non
    </div>
    <div class="question">
        <label>Souhaitez-vous parler de ces sujets avec un professionnel ? (9)</label><br>
        <input type="radio" name="parler_violences" value="Oui"> Oui
        <input type="radio" name="parler_violences" value="Non"> Non
    </div>
    <div class="question">
        <label>Vous sentez-vous en sécurité avec votre partenaire actuel, un(e) ex-partenaire ?</label><br>
        <input type="radio" name="securite_partenaire" value="Tout le temps"> Tout le temps
        <input type="radio" name="securite_partenaire" value="Pas toujours"> Pas toujours
        <input type="radio" name="securite_partenaire" value="Rarement"> Rarement
        <input type="radio" name="securite_partenaire" value="Pas de partenaire"> Pas de partenaire
    </div>

<!-- SECTION 8 -->
    <h3>Section 8 : Autres aspects psychosociaux</h3>
    <div class="question">
        <label>Disposez-vous d’une personne de confiance sur qui vous pouvez compter en cas de besoin ?</label><br>
        <input type="radio" name="personne_confiance" value="Oui"> Oui (précisez : <input type="text" name="confiance_details"> )<br>
        <input type="radio" name="personne_confiance" value="Non"> Non
    </div>
    <div class="question">
        <label>Souhaitez-vous connaître les aides financières disponibles adaptées à votre situation ?</label><br>
        <input type="radio" name="aides_financieres" value="Oui"> Oui
        <input type="radio" name="aides_financieres" value="Non"> Non
    </div>
    <div class="question">
        <label>Avez-vous des difficultés professionnelles (burn out, harcèlement…) qui influencent votre situation actuelle ?</label><br>
        <input type="radio" name="difficultes_pro" value="Oui"> Oui
        <input type="radio" name="difficultes_pro" value="Non"> Non
    </div>

<!-- SECTION 9 -->
    <h3>Section 9 : Suggestions ou préoccupations spécifiques</h3>
    <div class="question">
        <label>Y a-t-il un sujet que vous aimeriez particulièrement aborder lors de votre consultation ?</label><br>
        <input type="text" name="sujet_particulier" placeholder="Votre réponse">
    </div>

<!-- BUTTONS AT THE END OF EVERYTHING -->
    <button type="button" onclick="genererResume()">Générer Résumé</button>
    <h3>Résumé</h3>
    <pre id="resume"></pre>
    <button type="button" onclick="telechargerResume()">Télécharger Résumé</button>

    <!-- All scripts at the end -->
    <script>
        function genererResume() {
            let resume = "Résumé des réponses :\n";
            // Combine Section 1 and 2 form queries
            // Also gather Section 3 and Section 4 data
            // The easiest is to handle everything as if it's under one big form

            // If you want the code to gather from the entire document, just query body
            // or keep referencing the form if you prefer that structure.

            // We'll gather all inputs from the document, not just the single form with ID
            // Because Section 3 & 4 might be outside the form?
            let allInputs = document.querySelectorAll("input, select, textarea");

            allInputs.forEach(input => {
                // We only care if it's checked (for radio/checkbox) or a text with a value
                if ((input.type === "checkbox" || input.type === "radio") && input.checked) {
                    let questionDiv = input.closest(".question");
                    if(questionDiv) {
                        let label = questionDiv.querySelector("label");
                        if(label) {
                            resume += `${label.innerText} : ${input.value}\n`;
                        }
                    }
                } else if (input.type === "text" && input.value.trim() !== "") {
                    let questionDiv = input.closest(".question");
                    if(questionDiv) {
                        let label = questionDiv.querySelector("label");
                        if(label) {
                            resume += `${label.innerText} : ${input.value}\n`;
                        }
                    }
                }
            });

            // If no answers, show something
            if(resume === "Résumé des réponses :\n") {
                resume += "(Aucune réponse renseignée)\n";
            }

            document.getElementById("resume").innerText = resume;
        }

        function telechargerResume() {
            let texte = document.getElementById("resume").innerText;
            let blob = new Blob([texte], { type: "text/plain" });
            let link = document.createElement("a");
            link.href = URL.createObjectURL(blob);
            link.download = "resume.txt";
            link.click();
        }
    </script>
</body>
</html>

