<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);

const quotes = ref([
  {
    author: "Abu Bakr Al-Siddiq",
    text_ar: "إن الله تبارك وتعالى فاتح عليكم، فلا تأخذُن منها إلا بلاغًا.",
    text_en:
      "Allah, the Exalted, has opened a door for you, so do not take from it except what is sufficient.",
  },
  {
    author: "Umar ibn Al-Khattab",
    text_ar:
      "وإذا عرض لك أمران: أحدهما لله والآخر للدنيا، فآثر نصيبك من الآخرة على نصيبك من الدنيا، فأن الدنيا تنفد والآخرة تبقى.",
    text_en:
      "If two matters are presented to you, one for Allah and the other for the worldly life, then choose your share of the Hereafter over your share of this world, for the worldly life will perish and the Hereafter will remain.",
  },
  {
    author: "Uthman ibn Affan",
    text_ar:
      "الدنيا خضرة، قد شُهِّيَتْ إلى الناس، ومال إليها كثيرٌ منهم، فلا تركنوا إلى الدنيا، ولا تثقوا بها، فإنها ليست بثقة، واعلموا أنها غير تاركة إلَّا من تركها.",
    text_en:
      "The worldly life is attractive and appealing to people, and many are deluded by it. Do not rely on the worldly life, and do not trust it, for it is not trustworthy. Know that no one leaves it except those who abandon it.",
  },
  {
    author: "Ali ibn Abi Talib",
    text_ar:
      "ارتحلت الدنيا مدبرة، وارتحلت الآخرة مقبلة، ولكل منهما بنون، فكونوا من أبناء الآخرة، ولا تكونوا من أبناء الدنيا. فإن اليوم عمل ولا حساب، وغدًا حساب ولا عمل",
    text_en:
      "The worldly life has turned away, and the Hereafter is approaching, and each has its children. So be among the children of the Hereafter, not among the children of the worldly life. Today is for action without accountability, and tomorrow is for accountability without action.",
  },
  {
    author: "Ibn Masud",
    text_ar:
      "ليس أحد إلا وهو ضيف على الدنيا وماله عاريـة، فالضيف مرتحل والعارية مردودة.",
    text_en:
      "Everyone is but a guest in this world, and his wealth is a loan. So, the guest will depart, and the loan will be returned.",
  },
  {
    author: "Ibn Umar",
    text_ar:
      "إذا أصبحتَ فلا تنتظِرِ المساءَ، وإذا أمسيْتَ فلا تنتظِرِ الصَّباحَ، وخُذْ من صِحَّتِك لمرضِك، ومن حياتِك لموتِك.",
    text_en:
      "When you wake up, do not await the evening, and when you are in the evening, do not await the morning. Take from your health for your illness, and from your life for your death.",
  },
  {
    author: "Hasan Al-Basri",
    text_ar: "من نافسك في دينك فنافسه، ومن نافسك في دنياك فألقها في نحره.",
    text_en:
      "Compete with others in matters of your religion, and whoever competes with you in worldly matters, throw them into his own throat.",
  },
  {
    author: "Lukman the Wise",
    text_ar:
      "يا بني، بعْ دنياك بآخرتك تربحهما جميعًا، ولا تبع آخرتك بدنياك تخسرهما جميعًا.",
    text_en:
      "O my son, trade your worldly life for your Hereafter, and do not trade your Hereafter for your worldly life, for you will lose them both.",
  },
  {
    author: "Al-Shafi'i",
    text_ar:
      "من غلبت عليه شدة الشهوة لحب الحياة، ألزمته العبودية لأهلها، ومن رضي بالقنوع زال عنه الخضوع.",
    text_en:
      "Whoever is overwhelmed by the intensity of desires for the love of life, he becomes enslaved to its people. But whoever is content with sufficiency, he is liberated from subservience.",
  },
  {
    author: "Al-Fudayl ibn 'Iyad",
    text_ar:
      "لو كانت الدنيا من ذهب يفنى والآخرة من خزف يبقى، لكان ينبغي لنا أن نختار خزفًا يبقى على ذهب يفنى.",
    text_en:
      "If the world were made of gold that perishes and the Hereafter of clay that remains, it would be appropriate for us to choose that which remains over that which perishes.",
  },
  {
    author: "Ibn Taymiyyah",
    text_ar: "ليس في الدنيا نعيمٌ يشبه نعيم الآخرة إلا نعيم الإيمان.",
    text_en:
      "There is no joy in this world that resembles the joy of the Hereafter except the joy of faith.",
  },
  {
    author: "Ibn Qayyim al-Jawziyya",

    text_ar:
      "الدنيا في الحقيقة لا تُذَمُّ، وإنما يُتوجه الذمُّ إلى فعل العبد فيها، ولكن لَمَّا غلبتْ عليها الشهوات والحظوظ، والغفلة والإعراض عن الله والدار الآخرة، فصار هذا هو الغالب على أهلها وما فيها، وهو الغالب على اسمها، صار لها اسم الذم عند الإطلاق، وإلا فهي مَبْنَى الآخرةِ ومزرعتُها، وفيها اكتسبتْ النفوسُ الإيمان، ومعرفةَ الله ومحبتَه وذكرَه ابتغاء مرضاته، وخيرُ عيش ناله أهل الجنة في الجنة، إنما كان بما زرعوه فيها، وكفى بها مدحًا وفضلًا",
    text_en:
      "The world is not to be blamed in reality, but rather the blame is directed towards the actions of the servant within it. However, when desires, fortunes, neglectfulness, and turning away from Allah and the Hereafter dominate, then this becomes prevalent among its people and within it. This becomes its predominant characteristic, and it is named with disparagement. Otherwise, it is the foundation of the Hereafter and its plantation. In it, souls acquire faith, knowledge of Allah, love for Him, and remembrance of Him in seeking His pleasure. The best of living obtained by the inhabitants of Paradise in Paradise is only by what they sowed therein, and it suffices for them in praise and favor.",
  },
]);

const currentQuote = ref(quotes.value[count.value]);
const nextQuote = () => {
  count.value = Math.floor(Math.random() * quotes.value.length);
  currentQuote.value = quotes.value[count.value];
};
</script>

<template>
  <div>
    <h1>{{ msg }}</h1>
    <button type="button" @click="nextQuote" class="next-btn">Next</button>
    <div class="card">
      <blockquote v-if="currentQuote">
        <q>{{ currentQuote.text_ar }}</q>
        <br />
        <q class="read-the-docs">{{ currentQuote.text_en }}</q>
        <br />
        <cite>{{ currentQuote.author }}</cite>
      </blockquote>
    </div>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
.card {
  margin: 1em;
  padding: 1em;
  height: 100vh;
}
.card blockquote {
  font-size: 1.5em;
  line-height: 1.5em;
  border: 1px solid #ccc;
  border-radius: 0.25em;
  text-align: center;
  margin: 0;
  padding: 0;
}
.next-btn {
  padding: 0.5em 1em;
  margin: 1em;
  border: 1px solid #ccc;
  border-radius: 0.25em;
  background-color: #3d3d3d;
  color: #fff;
  cursor: pointer;
}
</style>
