<script>
import Typewriter from "typewriter-effect/dist/core";

export default {
  name: "HomePage",
  mounted() {
    const typewriter = new Typewriter(this.$refs.typewriterRef, {
      delay: 10,
      autoStart: true,
    });
    typewriter
      .typeString("Bonjour l'artiste ! ")
      .pauseFor(1000)
      .typeString(
        "Nous avons besoin de toi pour apprendre à notre IA à coder sans faire d'erreurs. <br>"
      )
      .pauseFor(1000)
      .typeString(
        "Pour ce faire, nous avons créé un jeu où il te faudra coder une calculatrice plus vite que notre IA.<br>"
      )
      .pauseFor(1000)
      .typeString("Mais Attention ! ")
      .pauseFor(1000)
      .typeString("Il faut que le code soit impéccable ! ")
      .pauseFor(1000)
      .typeString("Car coder vite, c'est bien... ")
      .pauseFor(1000)
      .typeString("Mais coder bien, c'est mieux ! <br>")
      .pauseFor(1000)
      .typeString("Tu es partant ? ")
      .pauseFor(1000)
      .typeString("Super ! <br>")
      .pauseFor(1000)
      .typeString(
        "Voici les commandes qui te permettront d'écrire le programme : <br>"
      )
      .pauseFor(1000)
      .typeString(
        "<strong>La tortue 🐢</strong> : code aléatoirement une petite quantité avec peu de chances d'introduire des bugs <br>"
      )
      .pauseFor(1000)
      .typeString(
        "<strong>L'éclair ⚡</strong> : code aléatoirement une grande quantité avec beaucoup de chances d'introduire des bugs <br>"
      )
      .pauseFor(1000)

      .typeString(
        "<strong>Le bug 🪲</strong> : retire aléatoirement une certaine quantité de bugs <br>"
      )
      .pauseFor(1000)

      .typeString("Cliques sur START quand tu es prêt(e) 🙃.")
      .pauseFor(1000)
      .start();
  },
};
</script>

<template>
  <div>
    <p><span ref="typewriterRef"></span></p>
    <v-btn elevation="9" x-large color="primary" to="/interface"> START </v-btn>
  </div>
</template>
