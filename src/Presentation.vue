<template>
    <div class="container">
        <div class="text">
            <i class="fa-solid fa-arrow-left" :class="{ 'disabled': currentHistoire == 0 }" @click="decrement"></i>

            <h2>
                {{ histoire[currentHistoire].text }}
            </h2>
            <i class="fa-solid fa-arrow-right" :class="{ 'disabled': currentHistoire == histoire.length - 1 }" @click="increment"></i>
        </div>
        <img :src="histoire[currentHistoire].imageSrc" />
    </div>
</template>
<script>
export default {
    methods: {
        increment() {
            if (this.currentHistoire != this.histoire.length - 1) {
                this.currentHistoire++;
            }
        },
        decrement() {
            if (this.currentHistoire != 0) {
                this.currentHistoire--;
            }
        },
    },
    data() {
        return {
            currentHistoire: 0,
            histoire: [
                {
                    text: "Hunter x Hunter est un manga et un anime créé par Yoshihiro Togashi. L'histoire suit un jeune garçon nommé Gon Freecss, qui découvre que son père, Jin Freecss, est un Hunter - un membre d'une élite de chasseurs professionnels qui traquent des créatures dangereuses, récupèrent des artefacts rares et effectuent des missions spéciales. Gon décide alors de devenir lui aussi un Hunter pour retrouver son père et suivre ses traces.",
                    imageSrc: "gon2.png",
                },
                {
                    text: "Au cours de son voyage pour devenir un Hunter, Gon rencontre de nombreux amis et ennemis, et affronte des défis difficiles. Il se lie d'amitié avec Killua Zoldyck, un assassin prodige et héritier d'une famille de tueurs professionnels, ainsi que Leorio Paradinight, un étudiant en médecine qui veut devenir Hunter pour aider les gens. Ils sont également rejoints par Kurapika, un membre du clan Kurta, qui cherche à venger son peuple massacré pour leurs yeux écarlates uniques.",
                    imageSrc: "kindpng_2152860.png",
                },
                {
                    text: "Au fil de leur voyage, Gon et ses amis affrontent des adversaires redoutables, tels que Hisoka, un clown meurtrier qui est obsédé par le combat, la Brigade Fantôme, un groupe de criminels meurtriers, et la famille Zoldyck, une famille d'assassins redoutables et sans scrupules.",
                    imageSrc:
                        "hisoka___hunter_x_hunter___png_by_arialacava_dclu7m6-fullview.png",
                },
                {
                    text: "L'histoire de Hunter x Hunter est également centrée sur les épreuves que les Hunters doivent surmonter pour devenir des chasseurs professionnels. Ces épreuves comprennent des examens physiques et mentaux difficiles, ainsi que des missions dangereuses qui mettent leur vie en danger. Les Hunters sont également confrontés à des épreuves morales, où ils doivent faire des choix difficiles et prendre des décisions qui peuvent avoir des conséquences graves.",
                    imageSrc:
                        "215-2152806_transparent-gon-png-hunter-x-hunter-transparent-png.png",
                },
                {
                    text: "Au fur et à mesure que l'histoire progresse, Gon découvre la vérité sur la disparition de son père et doit faire face à des choix difficiles pour protéger ceux qu'il aime. La série est connue pour ses personnages intéressants et complexes, son intrigue captivante et sa violence parfois crue, mais aussi pour les longues pauses de son auteur entre les publications.",
                    imageSrc: "gon2.png",
                }
            ],
        };
    },
};
</script>
<style scoped>
h2 {
    font-family: "Manga style";
    font-size: 1.3em;
    height: 250px;
    font-family: poppins;
    font-style: italic;
}
div.container {
    padding-left: 200px;
    height: 100vh;
    background: #f6f6f6;
    transform: translateY(-2vh);
    display: flex;
    align-items: center;
}
.container div {
    width: 50%;
    display: flex;
    flex-direction: column;
    gap: 20px;
}
i {
    cursor: pointer;
    font-size: 1.5em;
    padding: 5px 15px;
    color: white;
    background-color: #0b6b37;
    border-radius: 5px;
}
i.disabled{
    background-color: #0b6b377d;
}
i.fa-arrow-left {
    align-self: flex-start;
}
i.fa-arrow-right {
    align-self: flex-end;
}
img{
    height: 90%;
    align-self: flex-end;
}
</style>
