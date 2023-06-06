<template>
    <div class="container">
        <div class="img-container">
            <div class="div1" @click="activePersonnage = 1">
                <img src="personnages\gon.png" alt="" />
                <img
                    class="gif"
                    src="personnages\gon-fighting-hisoka-in-hunter-x-hunter-wxvff9kw1dxfxzvu.gif"
                    alt=""
                />
            </div>
            <div class="div2" @click="activePersonnage = 2">
                <img
                    src="personnages\aniyuki-hunter-x-hunter-coloring-page-45.jpg"
                    alt=""
                />
                <img
                    class="gif"
                    src="personnages\GraveIdolizedHammerkop-max-1mb.gif"
                    alt=""
                />
            </div>
            <div class="div3" @click="activePersonnage = 3">
                <img
                    src="personnages/aniyuki-hunter-x-hunter-coloring-page-48.png"
                    alt=""
                />
                <img class="gif" src="personnages/giphy.gif" alt="" />
            </div>
            <div class="div4" @click="activePersonnage = 4">
                <img src="personnages/Leorio-Hunter-x-Hunter.png" alt="" />
                <img
                    class="gif"
                    src="personnages/DimpledLimpAplomadofalcon-size_restricted.gif"
                    alt=""
                />
            </div>
            <div class="div5" @click="activePersonnage = 5">
                <img
                    src="personnages/wonder-day-hunter-x-hunter-28.jpg"
                    alt=""
                />
                <img
                    class="gif"
                    src="personnages/BlindFlatBrahmancow-max-1mb.gif"
                    alt=""
                />
            </div>
            <div class="div6" @click="activePersonnage = 6">
                <img
                    src="personnages/aniyuki-hunter-x-hunter-coloring-page-52-803x1024.png"
                    alt=""
                />
                <img
                    class="gif"
                    src="personnages/AcceptableOrneryFlyingfox-max-1mb.gif"
                    alt=""
                />
            </div>
            <div class="div7" @click="activePersonnage = 7">
                <img
                    src="personnages/wonder-day-hunter-x-hunter-65-753x1024.png"
                    alt=""
                />
                <img
                    class="gif"
                    src="personnages/tumblr_nsq4uqQdAr1tes8zmo1_540.gif"
                    alt=""
                />
            </div>
            <div class="div8" @click="activePersonnage = 8">
                <img
                    src="personnages/wonder-day-hunter-x-hunter-52-820x1024.jpg"
                    alt=""
                />
                <img
                    class="gif"
                    src="personnages/komacine.gif"
                    alt=""
                />
            </div>
        </div>
        <div class="text">
            <div>
                <h2>{{ personnages[activePersonnage - 1].nom }}</h2>
                <p>
                    {{ personnages[activePersonnage - 1].desc }}
                </p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    mounted() {
        console.log(this.personnages);
    },
    name: "personnages",
    data() {
        return {
            activePersonnage: 1,
            personnages: [
                {
                    id: 1,
                    nom: "GON FREECS",
                    desc: `Gon Freecss est un jeune garçon provenant d'un petit village
                    aimé des animaux. Il rêve de devenir Hunter afin de
                    retrouver son père, le plus grand Hunter de tous, qu'il n'a
                    jamais vu qu'en photo. Mais pour devenir Hunter
                    professionnel, il faut passer plusieurs épreuves et tests
                    très difficiles. Pendant les épreuves, Gon fait la
                    connaissance d'amis tel que Kirua, Kurapica, Leorio mais de
                    très dangereux combattants sont également présent afin de
                    passer le test de Hunter.`,
                },
                {
                    id: 2,
                    nom: "KILLUA ZOLDYCK",
                    desc: `Killua Zoldyck est un personnage principal de Hunter x Hunter, issu d'une famille d'assassins professionnels. Il possède des compétences exceptionnelles en matière de combat, d'espionnage et de manipulation, ainsi qu'une personnalité douce et empathique. Malgré son passé sombre, Killua est un personnage sympathique et protecteur envers ses amis, en particulier Gon, avec qui il partage un lien fort tout au long de leur voyage pour devenir des Hunters. Au fil de la série, Killua doit surmonter ses propres défis personnels, trouver sa propre voie dans la vie et développer sa propre identité.`,
                },
                {
                    id: 3,
                    nom: "KURAPIKA KURTA",
                    desc: `Kurapika est un jeune homme au regard écarlate, dernier survivant du clan Kurta décimé par la Brigade Fantôme. Animé par une vengeance implacable, il devient un Hunter pour traquer les membres de la Brigade Fantôme et récupérer les yeux écarlates volés de son clan. Utilisateur du Nen, sa technique des "Chaînes Écarlates" lui permet de manipuler de puissantes chaînes pour la guérison, la protection et l'attaque. Calme et réfléchi, Kurapika est prêt à tout pour atteindre son but, mais se questionne parfois sur sa quête de vengeance. Malgré sa méfiance initiale, il se lie d'amitié avec Gon, Killua et Leorio, et développe des liens solides avec ses compagnons de chasseurs.`,
                },
                {
                    id: 4,
                    nom: "LEORIO PARADINIGHT",
                    desc: `Leorio est un membre du groupe de chasseurs formé par Gon, Kurapika et Killua dans le manga Hunter x Hunter. Il se distingue par son apparence ordinaire et son attitude généralement joviale. Bien qu'il ne possède pas les capacités spéciales du Nen comme ses compagnons, Leolio compense cela par sa force physique et son intelligence. Il est motivé par son désir de devenir un médecin pour aider les autres, et sa compétence en matière de soins est souvent mise en avant. Leolio est un personnage loyal, protecteur et dévoué envers ses amis, prêt à se battre pour les soutenir. Son tempérament impulsif et son attitude parfois colérique ajoutent une dynamique intéressante au groupe. Malgré sa nature enjouée, Leolio peut être sérieux et réfléchi lorsque la situation l'exige. Son personnage évolue au fil de l'histoire, et il se révèle être un allié précieux pour ses compagnons de chasseurs dans leurs aventures.`,
                },
                {
                    id: 5,
                    nom: "HISOKA MOROW",
                    desc: `Hisoka Morow, est un personnage complexe et intrigant de Hunter x Hunter. Il est un membre énigmatique de la Brigade Fantôme et se distingue par son apparence excentrique et son comportement sadique. Hisoka est un combattant redoutable, utilisant le Nen pour renforcer sa force et ses capacités. Il est obsédé par la recherche de puissants adversaires et éprouve un plaisir malsain lorsqu'il se mesure à des combattants compétents. Son caractère manipulateur et imprévisible le rend à la fois fascinant et effrayant. Hisoka est prêt à trahir ses alliés et à changer d'allégeance en fonction de ses propres intérêts. Sa personnalité charismatique, son humour sombre et son amour pour les combats intenses en font un personnage emblématique de la série.`,
                },
                {
                    id: 6,
                    nom: "FEITAN PORTOR",
                    desc: `Feitan Portor, est un membre redoutable de la Brigade Fantôme. Il est calme, silencieux et se démarque par son apparence sombre et son air mystérieux. Feitan est un combattant exceptionnel qui excelle dans l'utilisation du Nen, notamment avec sa technique "Pain Packer" qui lui permet de manipuler la douleur et de la convertir en une puissance destructrice. Il est reconnu pour sa cruauté impitoyable envers ses ennemis et son penchant pour les batailles sanglantes. Feitan est un personnage complexe, gardant généralement ses émotions sous contrôle, mais révélant parfois un côté sadique. Sa dévotion envers la Brigade Fantôme et son dévouement à leur cause en font un membre précieux et redoutable de l'organisation criminelle.`,
                },
                {
                    id: 7,
                    nom: "SHIZUKU MURASAKI",
                    desc: `Shizuku Murasaki, est une membre de la Brigade Fantôme. Elle se distingue par son apparence douce et sa personnalité calme. Shizuku possède une capacité spéciale appelée "Cleaner" qui lui permet de sucer des objets à l'aide d'un aspirateur magique et d'en extraire des informations précieuses. Elle est souvent perçue comme étant naïve, mais sa compétence en tant que membre de la Brigade Fantôme est incontestable. Malgré son apparence fragile, Shizuku peut se montrer impitoyable et déterminée lorsqu'il s'agit de protéger ses camarades. Son attitude bienveillante et son sens de la camaraderie font d'elle un membre apprécié de l'organisation criminelle, apportant une touche d'équilibre et de compassion au sein de la Brigade Fantôme.`,
                },
                {
                    id: 8,
                    nom: "MACHI KOMACINE",
                    desc: `Machi Komacine est un membre énigmatique de la Brigade Fantôme. Elle se distingue par son apparence élégante et son calme apparent. Machi possède une maîtrise exceptionnelle du Nen, utilisant ses fils de Nen pour diverses compétences, notamment pour la couture et pour attaquer ses ennemis avec précision. Elle est reconnue pour sa loyauté envers la Brigade Fantôme et est considérée comme l'une des membres les plus fiables de l'organisation. Bien qu'elle puisse sembler détachée et froide, Machi a montré des moments de compassion et de soutien envers ses camarades, en particulier envers Hisoka. Son aura mystérieuse et son expertise en matière de manipulation des fils de Nen en font un personnage intrigant et redoutable au sein de la Brigade Fantôme.`,
                },
            ],
        };
    },
};
</script>
<style lang="scss" scoped>
div.container {
    transform: translateY(-15vh);
    display: flex;
    background: #f6f6f6;
    gap: 20px;
}
img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    cursor: pointer;
}

.img-container {
    height: 1200px;
    background-color: rgb(52, 52, 52);
    padding: 5px;
    width: 50%;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(16, 1fr);
    gap: 5px 5px;
    grid-auto-flow: row;
    grid-template-areas:
        "div1 div2"
        "div1 div2"
        "div1 div2"
        "div1 div2"
        "div3 div2"
        "div3 div4"
        "div3 div4"
        "div5 div4"
        "div5 div4"
        "div5 div6"
        "div5 div6"
        "div7 div6"
        "div7 div8"
        "div7 div8"
        "div7 div8"
        "div7 div8";
}
.img-container div {
    .gif {
        opacity: 0;
        &:hover {
            opacity: 1;
            transition: 1.2s;
        }
    }
}
.div1 {
    grid-area: div1;
    position: relative;
    &:hover {
        body {
            background-color: aqua;
        }
    }
}
.div2 {
    grid-area: div2;
    position: relative;
}
.gif {
    position: absolute;
    top: 0;
    left: 0;
}

.div3 {
    grid-area: div3;
    position: relative;
}
.div4 {
    grid-area: div4;
    position: relative;
}
.div5 {
    grid-area: div5;
    position: relative;
}
.div6 {
    grid-area: div6;
    position: relative;
}
.div7 {
    grid-area: div7;
    position: relative;
}
.div8 {
    grid-area: div8;
    position: relative;
}

.text {
    margin-top: 100px;
    width: 50%;
    h2 {
        color: #c7213b;
    }
    p {
        font-family: poppins;
        font-style: italic;
        margin-top: 20px;
        font-size: 1.3em;
    }

    div {
        position: sticky;
        top: 20%;
    }
}
</style>
